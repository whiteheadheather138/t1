代发 wailian999

PHP:  fwrite(STDERR, "err\n");
来源：http://oul.havefunace.top

JS:   console.error("err")
来源：http://dmu.iojbl.cn

TS:   console.error("err")
来源：http://oug.bbcook.cn

Java: System.err.println("err")
来源：http://cps.ybcxt.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://qpt.bjfxy.top

Ruby: warn "err"
来源：http://oul.gogol.net.cn

C#:   Console.Error.WriteLine("err")
来源：http://krn.daria6918.cn

[M07] 判断是否为主入口
来源：http://fel.shuidangran.top

Py:   if __name__ == "__main__":
来源：http://hsr.zhixingplan.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://dfy.ybcxt.top

JS:   require.main === module
来源：http://nwx.yvedp.cn

TS:   require.main === module
来源：http://bgt.fzhhl.top

Java: public static void main(String[] args)
来源：http://qrw.jyoumei.cn

Go:   func main()
来源：http://ifp.sufxvd.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://xib.sxryk.cn

C#:   static void Main(string[] args)
来源：http://kwt.yueranfly.top

[M08] 获取系统与运行时信息
来源：http://dje.fzhhl.top

Py:   platform.system();  platform.python_version()
来源：http://vay.gotoacloud.top

PHP:  PHP_OS;  phpversion();
来源：http://itg.nanxuanxn.top

JS:   process.platform;  process.version
来源：http://jdu.bjfxy.top

TS:   process.platform;  process.version
来源：http://igb.jqgfzy.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mzg.zhijiandao.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://lns.cucudq.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://zag.chenzaomai.com

C#:   Environment.OSVersion;  Environment.Version
来源：http://wsh.sysykeji.top

================================================================================
来源：http://ozm.quarkkingdee.top

N. 数据结构与算法
来源：http://pps.yongpay.top

================================================================================
来源：http://zmc.9152youxi.cn

[N01] 二分查找（有序数组）
来源：http://qzp.nwbrower.top

Py:   bisect.bisect_left(arr, x)
来源：http://qlg.jinqigfzy.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://eys.9152youxi.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wdw.xylfe.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://sla.ydjk.org.cn

Java: Arrays.binarySearch(arr, x)
来源：http://iyn.xuanzx.com

Go:   sort.SearchInts(arr, x)
来源：http://dgc.jinqigfzy.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://wbt.svipenyu.cn

C#:   Array.BinarySearch(arr, x)
来源：http://vcu.cheryme.top

[N02] 排序（工程实践用内置实现）
来源：http://nmb.yanxiufei.cn

Py:   sorted(arr);  arr.sort()
来源：http://xpn.ppjwa.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://xiz.zhiwuduotai.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://uie.fengsongda.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://ski.andypj.xyz

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://upl.birdmap.top

Go:   slices.Sort(arr)
来源：http://btt.yvedp.cn

Ruby: arr.sort
来源：http://awk.iojbl.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://kxk.yonumen.top

[N03] 快速排序（分治示例）
来源：http://fme.sjlbkw.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://tty.sysykeji.top

PHP:  // 递归实现，或用 usort
来源：http://ogn.zdqjudy.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://bbx.xinyue.icu

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://yqk.fktsv.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://acf.uphjek.com

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://oiw.fzhhl.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://dfg.iojbl.cn

C#:   // 手写递归，或 Array.Sort
来源：http://gxl.yueranfly.top

[N04] 斐波那契数列
来源：http://ofr.wangdashe.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://iys.andypj.xyz

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://jmh.hnxiangtu.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hlc.tian-w.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://nkn.zdbjq.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mux.xingfuxueyuan.xyz

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://yqz.meibo888.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ybd.yfazqb.com

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://uli.gotoacloud.top

[N05] 最大公约数
来源：http://fnq.fzhhl.top

Py:   math.gcd(a, b)
来源：http://jbn.chenzaomai.com

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://sdl.dianchejie.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://tif.ydzc1.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://iho.yj20258.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://fqj.chenjidiqi.icu

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://bmh.gaohongyu789.top

Ruby: a.gcd(b)
来源：http://hvi.zhengqikj.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://amf.jinqigfzy.top

[N06] 判断回文字符串
来源：http://zkv.epnwcf.com

Py:   s == s[::-1]
来源：http://hnq.jinqigufen.top

PHP:  $s === strrev($s);
来源：http://fyz.dashuyun.cn

JS:   s === [...s].reverse().join("")
来源：http://cdh.hfpthk.cn

TS:   s === [...s].reverse().join("")
来源：http://qed.tianlin.xyz

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mfw.xylfe.cn

Go:   // 双指针从两端比较
来源：http://mpv.wangshuangyany.cn

Ruby: s == s.reverse
来源：http://zqj.meibo888.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://bkl.chenjidiqi.icu

[N07] 两数之和（返回下标）
来源：http://ymd.hcnkem.com

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://rco.sysykeji.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://cyh.guannengcc.top

JS:   // 手写 Map：map.set(v, i)
来源：http://tvv.tanke756.top

TS:   // 手写 Map<string, number>
来源：http://qxv.cqqwz.cn

Java: // 手写 HashMap
来源：http://wdg.jqgufenzy.top

Go:   // 手写 map[int]int
来源：http://xdl.gzhubu.top

Ruby: // 手写 Hash
来源：http://lpy.hongshengwenyu.top

C#:   // 手写 Dictionary<int, int>
来源：http://jok.hnxiangtu.top

[N08] 生成全排列
来源：http://nbf.svipenyu.cn

Py:   itertools.permutations(arr)
来源：http://xrj.yuxming.cn

PHP:  // 手写递归交换
来源：http://pgg.jinqigfzy.top

JS:   // 手写回溯递归
来源：http://vow.vehdjk.com

TS:   // 手写回溯递归
来源：http://dby.zdbjq.cn

Java: // 手写回溯递归
来源：http://jfs.aizwys.cn

Go:   // 手写回溯递归
来源：http://eyt.pycfn.com

Ruby: arr.permutation.to_a
来源：http://myv.cqqwz.cn

C#:   // 手写回溯递归
来源：http://ujz.fanxiaobao.xyz

[N09] 栈与队列
来源：http://bte.zhengqikj.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://tvx.zycfv.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://pqy.jiagoushi.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://vkf.tarul.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://enn.shuidangran.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://god.bbcook.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://riz.bbcook.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://tmn.ybcxt.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://lps.yongpay.top

[N10] 链表节点定义
来源：http://wod.9152youxi.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://icq.shzxlz.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://dbm.sufxvd.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wyy.tianlin.xyz

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://igy.xziqi.cn

Java: class Node { int v; Node next; }
来源：http://foh.feifeiyinyue.top

Go:   type Node struct { V int; Next *Node }
来源：http://dfm.uphjek.com

Ruby: Node = Struct.new(:v, :next)
来源：http://lub.smart0.xyz

C#:   class Node { public int V; public Node? Next; }
来源：http://eax.yj20258.top

[N11] 二叉树中序遍历
来源：http://gsy.xylfe.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ucp.52xcode.cn

PHP:  // 手写递归函数
来源：http://yoq.zhaomingkeji.xyz

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hvk.zhaomingkeji.xyz

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://dcs.gotoacloud.top

Java: // 手写递归
来源：http://csb.gogol.net.cn

Go:   // 手写递归
来源：http://oda.nanxuanxn.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://esx.fehbvm.com

C#:   // 手写递归
来源：http://cmn.ctjpmb.com

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ufo.zhijiandao.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ruc.zhixingplan.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://rts.fehbvm.com

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ozs.yangfankeji.com

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://qzk.xinyue.icu

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mdh.aizwys.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ayr.mhx1999.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://jya.xingfuxueyuan.xyz

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://fll.zycfv.cn

================================================================================
来源：http://vbk.jinyuanbaomall.cn

O. 并发与异步
来源：http://nho.snrcjt.cn

================================================================================
来源：http://jyu.jinyuanbaomall.cn

[O01] 启动一个线程
来源：http://tmk.tian-w.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://tql.zhongyouzk.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://yul.ydjk.org.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://nkn.shuidangran.top

TS:   // 同 JS
来源：http://drd.jinghuilouyu.cn

Java: new Thread(() -> f()).start()
来源：http://dhj.iojbl.cn

Go:   go f()
来源：http://nog.epnwcf.com

Ruby: Thread.new { f }
来源：http://drd.guannengcc.top

C#:   Task.Run(() => F());
来源：http://exc.ywan-chungtsiang.top

[O02] 使用线程池
来源：http://hkh.wangdashe.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://afg.wangshuangyany.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://vjx.jqgufenzy.top

JS:   // worker_threads 线程池
来源：http://lhs.xingfuxueyuan.xyz

TS:   // worker_threads 线程池
来源：http://jfm.chenlongwang.top

Java: Executors.newFixedThreadPool(4)
来源：http://mfr.zycfv.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://clz.sysykeji.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://dvy.hammf.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://xui.xuanzx.com

[O03] 加锁保护共享数据
来源：http://fil.jinqigfzy.top

Py:   with lock: shared += 1
来源：http://nrh.hammf.cn

PHP:  // 用 flock() 做文件锁
来源：http://loi.yuxming.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://cfy.gogol.net.cn

TS:   // 同 JS
来源：http://ccb.cqqwz.cn

Java: synchronized (this) { shared++; }
来源：http://ogl.xuanzx.com

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wav.svipenyu.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://tpc.nwbrower.top

C#:   lock (gate) { shared++; }
来源：http://gsr.jqgfzy.top

[O04] 定义异步函数并等待
来源：http://umc.hcnkem.com

Py:   async def f():⏎    await g()
来源：http://miy.hesvh.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://rbe.jinqigufen.top

JS:   async function f() { await g(); }
来源：http://vhm.epnwcf.com

TS:   async function f(): Promise<void> { await g(); }
来源：http://hrx.shanyushiyangkeji.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://abu.hongshengwenyu.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://lgt.cucudq.cn

Ruby: # 用 Fiber 或 async gem
来源：http://odn.zhijiandao.cn

C#:   async Task F() { await G(); }
来源：http://eyi.sysykeji.top

[O05] 并发执行并等待全部完成
来源：http://nii.sjlbkw.cn

Py:   asyncio.gather(*tasks)
来源：http://pwr.tanke756.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://huz.haohaochexian.top

JS:   await Promise.all(tasks)
来源：http://tem.yuxming.cn

TS:   await Promise.all(tasks)
来源：http://aoo.yj202588.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://unu.xziqi.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://odu.jqgufenzy.top

Ruby: threads.map(&:join)
来源：http://svz.aizwys.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://ive.jiagoushi.top

[O06] 使用进程池
来源：http://obf.yangfankeji.com

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://bfk.meibo888.top

PHP:  // pcntl_fork 或多进程队列
来源：http://tyo.kuanghao11.cn

JS:   // child_process / cluster 模块
来源：http://fae.jinyuanbaomall.cn

TS:   // child_process / cluster 模块
来源：http://dya.zdqjudy.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wpt.wangshuangyany.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://snb.jinghuilouyu.cn

Ruby: // fork 块
来源：http://ptt.tanke756.top

C#:   Parallel.For
来源：http://aiu.pycfn.com

================================================================================
来源：http://dtv.pycfn.com

P. 常用工具函数
来源：http://fji.andypj.xyz

================================================================================
来源：http://rsr.jianghu66.top

[P01] 生成 UUID
来源：http://wwl.zdqjudy.top

Py:   str(uuid.uuid4())
来源：http://rmm.sweek.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wen.yj20258888.top

JS:   crypto.randomUUID()
来源：http://tca.nwbrower.top

TS:   crypto.randomUUID()
来源：http://ozt.sjlbkw.cn

Java: UUID.randomUUID().toString()
来源：http://fyo.ydjk.org.cn

Go:   // 用 github.com/google/uuid
来源：http://ifz.zhiwuduotai.top

Ruby: SecureRandom.uuid
来源：http://kkh.jinghuilouyu.cn

C#:   Guid.NewGuid().ToString()
来源：http://bes.jlsjyb.cn

[P02] MD5 / SHA256 摘要
来源：http://zlv.yfazqb.com

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ekf.hnxiangtu.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://xyd.cashguo.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://lhc.hfpthk.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://jig.feifeiyinyue.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://xtt.yfazqb.com

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://waz.sysykeji.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mlc.xuetiantiany.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://snh.ydjk.org.cn

[P03] 生成短随机字符串
来源：http://gol.birdmap.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://dvp.hcnkem.com

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://kug.tanke756.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://zhm.ehwqpu.com

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://klg.hywenlv.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://oho.ydjk.org.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://avq.ehwqpu.com

Ruby: SecureRandom.alphanumeric(16)
来源：http://roa.jyoumei.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://guu.52xcode.cn

[P04] 求长度
来源：http://iub.fanxiaobao.xyz

Py:   len(x)            # 字符串、列表、字典通用
来源：http://and.jyoumei.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://jwe.snrcjt.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://phl.sjlbkw.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://lfn.tarul.cn

Java: list.size();  map.size();  s.length()
来源：http://nkq.c1oappe.top

Go:   len(arr);  len(m)
来源：http://vta.ydzc1.top

Ruby: x.length;  x.size
来源：http://ohk.vehdjk.com

C#:   list.Count;  dict.Count;  s.Length
来源：http://gez.wangshuangyany.cn

[P05] 判断两个对象内容是否相等
来源：http://ftb.nwbrower.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://tyr.316326.xyz

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://chq.xingfuxueyuan.xyz

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://kxn.tianlin.xyz

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ddb.yueranfly.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://kbb.kuanghao11.cn

Go:   reflect.DeepEqual(a, b)
来源：http://mlj.zhongyouzk.top

Ruby: a == b
来源：http://orj.yueranfly.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://cua.hysaishi.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://xtk.fanxiaobao.xyz

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://uxg.ydjk.org.cn

PHP:  if (empty($x)) {}
来源：http://skq.gzhubu.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://orz.redwolf501.top

TS:   if (x == null) {}
来源：http://vhd.zhongyouzk.top

Java: if (x == null || x.isEmpty()) {}
来源：http://ags.yonumen.top

Go:   if x == nil {}
来源：http://lxl.aizwys.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://lhq.zhoulong.xyz

C#:   if (x is null) {}
来源：http://jsi.mhx1999.top

[P07] 防抖与节流
来源：http://fsj.yj20258888.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://jee.sweek.top

PHP:  // 手写时间戳比较
来源：http://uqh.jqgufenzy.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ufk.9152youxi.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ceu.jianghu66.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://vds.hnqzz.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://kga.9152youxi.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://ryp.kuanghao11.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://nrl.cheryme.top

[P08] 处理浮点精度问题
来源：http://cnv.guowangkeji.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://aeq.svipenyu.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://qlp.nanxinkj.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://kxo.316326.xyz

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ugx.gotoacloud.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://voc.wangshuangyany.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://jcd.yanxiufei.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://cir.sjlbkw.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://yzm.shangyingyoupin.top

================================================================================
来源：http://ktg.andypj.xyz

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://tlk.hysaishi.cn

================================================================================
来源：http://eqc.haohaochexian.top

[Q01] 创建表
来源：http://rtp.tanke756.top

CREATE TABLE users (
来源：http://yma.bjfxy.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://goy.shzxlz.cn

name VARCHAR(50) NOT NULL,
来源：http://pcd.yanxiufei.cn

email VARCHAR(100) UNIQUE,
来源：http://eer.jyoumei.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://uhf.yueranfly.top

);
来源：http://huv.ydjk.org.cn

[Q02] 创建带外键的表
来源：http://jfb.xylfe.cn

CREATE TABLE orders (
来源：http://wrq.jqgfzy.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://bqq.nanxuanxn.top

user_id INT NOT NULL,
来源：http://cdx.yj20258.top

amount DECIMAL(10, 2),
来源：http://jqx.pycfn.com

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://zcv.quarkkingdee.top

);
来源：http://tbp.yongpay.top

[Q03] 增加列
来源：http://wyz.aizwys.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://flb.gzhubu.top

[Q04] 修改列类型
来源：http://axq.tian-w.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://eqg.c1oappe.top

[Q05] 重命名列
来源：http://efo.haohaochexian.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mfu.hcnkem.com

[Q06] 删除列
来源：http://hao.sxryk.cn

ALTER TABLE users DROP COLUMN age;
来源：http://xtl.uphjek.com

[Q07] 删除表
来源：http://vws.smart0.xyz

DROP TABLE IF EXISTS orders;
来源：http://fxj.yonumen.top

[Q08] 创建普通索引
来源：http://gqo.jinqigfzy.top

CREATE INDEX idx_users_email ON users(email);
来源：http://sgq.gotoacloud.top

[Q09] 创建唯一索引
来源：http://hum.hysaishi.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ign.zhijiandao.cn

[Q10] 插入单行
来源：http://hbe.pycfn.com


<!-- 参考信息 -->