代发 wailian999

Ruby: exit 1
来源：http://ghu.yj20258888.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://lhu.aibaodan.cn

[M06] 向标准错误输出
来源：http://ukm.kuanghao11.cn

Py:   print("err", file=sys.stderr)
来源：http://omn.hcnkem.com

PHP:  fwrite(STDERR, "err\n");
来源：http://bgx.yj20258.top

JS:   console.error("err")
来源：http://aen.yuxming.cn

TS:   console.error("err")
来源：http://oza.xuanzx.com

Java: System.err.println("err")
来源：http://iiz.jianghu66.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://van.chenjidiqi.icu

Ruby: warn "err"
来源：http://mtx.pengpengdd.cyou

C#:   Console.Error.WriteLine("err")
来源：http://mom.tian-w.cn

[M07] 判断是否为主入口
来源：http://sxx.yonumen.top

Py:   if __name__ == "__main__":
来源：http://ufy.jinyuanbaomall.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://tao.jinyuanbaomall.cn

JS:   require.main === module
来源：http://tuu.gotoacloud.top

TS:   require.main === module
来源：http://zwn.zhiwuduotai.top

Java: public static void main(String[] args)
来源：http://jxt.chenzaomai.com

Go:   func main()
来源：http://qur.tian-w.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mig.gzhubu.top

C#:   static void Main(string[] args)
来源：http://zlh.xuanzx.com

[M08] 获取系统与运行时信息
来源：http://cnc.yvedp.cn

Py:   platform.system();  platform.python_version()
来源：http://kre.ybcxt.top

PHP:  PHP_OS;  phpversion();
来源：http://jmz.quarkkingdee.top

JS:   process.platform;  process.version
来源：http://jdz.yj202588.top

TS:   process.platform;  process.version
来源：http://ski.hesvh.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://emd.wangdashe.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://fjs.yonumen.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://fxk.tarul.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://kiw.c1oappe.top

================================================================================
来源：http://ajk.zhongyouzk.top

N. 数据结构与算法
来源：http://anw.ctjpmb.com

================================================================================
来源：http://shd.hcnkem.com

[N01] 二分查找（有序数组）
来源：http://ypq.zhijiandao.cn

Py:   bisect.bisect_left(arr, x)
来源：http://zod.jqgufenzy.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ius.ctjpmb.com

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://leb.xingfuxueyuan.xyz

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://vpo.cucudq.cn

Java: Arrays.binarySearch(arr, x)
来源：http://btn.fanxiaobao.xyz

Go:   sort.SearchInts(arr, x)
来源：http://xfl.0kj1m.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://pdx.dianchejie.cn

C#:   Array.BinarySearch(arr, x)
来源：http://sle.9152youxi.cn

[N02] 排序（工程实践用内置实现）
来源：http://yzr.yfazqb.com

Py:   sorted(arr);  arr.sort()
来源：http://urm.jianghu66.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://vic.cucudq.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://naw.gzhubu.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://pou.xinyue.icu

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://zok.pycfn.com

Go:   slices.Sort(arr)
来源：http://vah.guannengcc.top

Ruby: arr.sort
来源：http://jtt.pengpengdd.cyou

C#:   Array.Sort(arr);  list.Sort()
来源：http://psy.0kj1m.cn

[N03] 快速排序（分治示例）
来源：http://czh.yanxiufei.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hea.ehwqpu.com

PHP:  // 递归实现，或用 usort
来源：http://yyq.hfpthk.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ecz.vehdjk.com

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blg.yanxiufei.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://nlv.ppjwa.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://zim.xuanzx.com

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://cya.birdmap.top

C#:   // 手写递归，或 Array.Sort
来源：http://sle.hcnkem.com

[N04] 斐波那契数列
来源：http://rhl.cheryme.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hbc.zhongyouzk.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ura.quarkkingdee.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://cjo.zhongyouzk.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://woq.wangdashe.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ufp.epnwcf.com

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://qir.shanyushiyangtech.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://twi.ehwqpu.com

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://chm.dashuyun.cn

[N05] 最大公约数
来源：http://mgq.guowangkeji.top

Py:   math.gcd(a, b)
来源：http://yhp.c1oappe.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://sqr.jinyuanbaomall.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://nvp.smart0.xyz

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ngu.hongshengwenyu.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://sbf.yj20258.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://rlk.gotoacloud.top

Ruby: a.gcd(b)
来源：http://cdl.shuidangran.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ibh.cdnleiting.top

[N06] 判断回文字符串
来源：http://dut.pycfn.com

Py:   s == s[::-1]
来源：http://cnb.gzhubu.top

PHP:  $s === strrev($s);
来源：http://uiq.hnqzz.top

JS:   s === [...s].reverse().join("")
来源：http://osh.pengpengdd.cyou

TS:   s === [...s].reverse().join("")
来源：http://jjw.guowangkeji.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://lsf.zhijiandao.cn

Go:   // 双指针从两端比较
来源：http://urz.fanxiaobao.xyz

Ruby: s == s.reverse
来源：http://wih.zhiwuduotai.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://ils.snrcjt.cn

[N07] 两数之和（返回下标）
来源：http://hya.svipenyu.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://fuw.shangyingyoupin.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://fnn.birdmap.top

JS:   // 手写 Map：map.set(v, i)
来源：http://zyk.sjlbkw.cn

TS:   // 手写 Map<string, number>
来源：http://vwr.fzhhl.top

Java: // 手写 HashMap
来源：http://pjz.316326.xyz

Go:   // 手写 map[int]int
来源：http://jrk.hongshengwenyu.top

Ruby: // 手写 Hash
来源：http://nlk.guowangkeji.top

C#:   // 手写 Dictionary<int, int>
来源：http://pba.9152youxi.cn

[N08] 生成全排列
来源：http://cdf.jlsjyb.cn

Py:   itertools.permutations(arr)
来源：http://yho.sufxvd.cn

PHP:  // 手写递归交换
来源：http://njg.zhiwuduotai.top

JS:   // 手写回溯递归
来源：http://gbm.0kj1m.cn

TS:   // 手写回溯递归
来源：http://smv.svipenyu.cn

Java: // 手写回溯递归
来源：http://qap.sufxvd.cn

Go:   // 手写回溯递归
来源：http://soq.redwolf501.top

Ruby: arr.permutation.to_a
来源：http://fko.yueranfly.top

C#:   // 手写回溯递归
来源：http://zpf.jlsjyb.cn

[N09] 栈与队列
来源：http://wve.chenjidiqi.icu

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://yjf.gzhubu.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://enw.jiagoushi.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://snv.chenlongwang.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://eur.cashguo.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://tpm.tianlin.xyz

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://rxc.gogol.net.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://gbi.xuetiantiany.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://cdx.wangshuangyany.cn

[N10] 链表节点定义
来源：http://idb.jyoumei.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://tkk.hnxiangtu.top

PHP:  class Node { public $v; public $next = null; }
来源：http://vuu.zhengqikj.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://npm.yongpay.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://nvb.shuidangran.top

Java: class Node { int v; Node next; }
来源：http://qmm.yongpay.top

Go:   type Node struct { V int; Next *Node }
来源：http://prv.chenlongwang.top

Ruby: Node = Struct.new(:v, :next)
来源：http://nav.redwolf501.top

C#:   class Node { public int V; public Node? Next; }
来源：http://sbb.yonumen.top

[N11] 二叉树中序遍历
来源：http://xbn.yanxiufei.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://jmg.shzxlz.cn

PHP:  // 手写递归函数
来源：http://moo.jlsjyb.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://pul.yuxming.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://emh.ywan-chungtsiang.top

Java: // 手写递归
来源：http://cjl.jinqigfzy.top

Go:   // 手写递归
来源：http://uia.zhaomingkeji.xyz

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mww.vehdjk.com

C#:   // 手写递归
来源：http://vfi.daria6918.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://dhz.pengpengdd.cyou

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://tqe.ybcxt.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://stg.yangfankeji.com

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mxr.cashguo.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://siy.zycfv.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://muc.birdmap.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://yuv.yuxming.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://qpi.andypj.xyz

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mpk.fehbvm.com

================================================================================
来源：http://hbl.zhixingplan.top

O. 并发与异步
来源：http://uds.daria6918.cn

================================================================================
来源：http://aly.kuanghao11.cn

[O01] 启动一个线程
来源：http://lam.ywan-chungtsiang.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://lww.chenjidiqi.icu

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ign.fengsongda.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://iby.redwolf501.top

TS:   // 同 JS
来源：http://xap.yonumen.top

Java: new Thread(() -> f()).start()
来源：http://ihv.guannengcc.top

Go:   go f()
来源：http://ipx.zhoulong.xyz

Ruby: Thread.new { f }
来源：http://yly.guannengcc.top

C#:   Task.Run(() => F());
来源：http://bdl.chenjidiqi.icu

[O02] 使用线程池
来源：http://cso.bjfxy.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wbw.jqgufenzy.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://zdu.tanke756.top

JS:   // worker_threads 线程池
来源：http://vap.yj20258.top

TS:   // worker_threads 线程池
来源：http://lvy.xziqi.cn

Java: Executors.newFixedThreadPool(4)
来源：http://qdc.xinyue.icu

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://lct.9152youxi.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wat.yueranfly.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mxj.bbcook.cn

[O03] 加锁保护共享数据
来源：http://vqo.pengpengdd.cyou

Py:   with lock: shared += 1
来源：http://bfw.daxiang520.top

PHP:  // 用 flock() 做文件锁
来源：http://zso.zycfv.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://sop.zycfv.cn

TS:   // 同 JS
来源：http://xac.aizwys.cn

Java: synchronized (this) { shared++; }
来源：http://cou.zdqjudy.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://buo.ywan-chungtsiang.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://dvz.epnwcf.com

C#:   lock (gate) { shared++; }
来源：http://wlm.xuetiantiany.cn

[O04] 定义异步函数并等待
来源：http://hir.yanxiufei.cn

Py:   async def f():⏎    await g()
来源：http://ggo.yj20258.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://jxv.hfpthk.cn

JS:   async function f() { await g(); }
来源：http://kjs.epnwcf.com

TS:   async function f(): Promise<void> { await g(); }
来源：http://nwi.zhoulong.xyz

Java: // 用 CompletableFuture 或虚拟线程
来源：http://pvb.pycfn.com

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ozu.hfpthk.cn

Ruby: # 用 Fiber 或 async gem
来源：http://lcp.daria6918.cn

C#:   async Task F() { await G(); }
来源：http://qvk.andypj.xyz

[O05] 并发执行并等待全部完成
来源：http://viu.mhx1999.top

Py:   asyncio.gather(*tasks)
来源：http://ans.shuidangran.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://gpz.vehdjk.com

JS:   await Promise.all(tasks)
来源：http://drw.ppjwa.cn

TS:   await Promise.all(tasks)
来源：http://fce.pengpengdd.cyou

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://qcp.yangfankeji.com

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://dou.cdnleiting.top

Ruby: threads.map(&:join)
来源：http://ghy.yonumen.top

C#:   await Task.WhenAll(t1, t2)
来源：http://ddx.hywenlv.cn

[O06] 使用进程池
来源：http://dfa.birdmap.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ohr.sufxvd.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://qmm.sufxvd.cn

JS:   // child_process / cluster 模块
来源：http://gyw.52xcode.cn

TS:   // child_process / cluster 模块
来源：http://ees.redwolf501.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://nwk.jianghu66.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://yex.haohaochexian.top

Ruby: // fork 块
来源：http://vki.tian-w.cn

C#:   Parallel.For
来源：http://ctg.ehwqpu.com

================================================================================
来源：http://ngz.52xcode.cn

P. 常用工具函数
来源：http://ppm.pengpengdd.cyou

================================================================================
来源：http://ugz.xziqi.cn

[P01] 生成 UUID
来源：http://wxp.cqqwz.cn

Py:   str(uuid.uuid4())
来源：http://eea.ctjpmb.com

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://vav.cashguo.top

JS:   crypto.randomUUID()
来源：http://pvb.guowangkeji.top

TS:   crypto.randomUUID()
来源：http://ika.redwolf501.top

Java: UUID.randomUUID().toString()
来源：http://qrw.yanxiufei.cn

Go:   // 用 github.com/google/uuid
来源：http://duc.xinyue.icu

Ruby: SecureRandom.uuid
来源：http://vxi.yuxming.cn

C#:   Guid.NewGuid().ToString()
来源：http://wzb.ppjwa.cn

[P02] MD5 / SHA256 摘要
来源：http://zit.yongpay.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://dbg.sjlbkw.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://lxo.dashuyun.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://xkz.tianlin.xyz

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://suj.ybcxt.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://yrp.meibo888.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ije.jinqigufen.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://dik.nanxuanxn.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://izi.zhijiandao.cn

[P03] 生成短随机字符串
来源：http://guz.yj20258.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://uyo.jqgfzy.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://xqd.snrcjt.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ajx.zhijiandao.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ims.zhengqikj.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ube.dianchejie.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://jgp.yanxiufei.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://ggu.dashuyun.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://nyn.fktsv.cn

[P04] 求长度
来源：http://dsm.svipenyu.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://tqt.chenjidiqi.icu

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ojz.ctjpmb.com

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://fwt.bbcook.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://bmk.vqdsnc.cn

Java: list.size();  map.size();  s.length()
来源：http://eif.ppjwa.cn

Go:   len(arr);  len(m)
来源：http://obx.hnxiangtu.top

Ruby: x.length;  x.size
来源：http://sty.52xcode.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://psu.0kj1m.cn

[P05] 判断两个对象内容是否相等
来源：http://bud.tianlin.xyz

Py:   a == b              # 列表与字典递归比较内容
来源：http://txq.xylfe.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ulg.gzhubu.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://sme.hfpthk.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://rje.iojbl.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://zvr.hesvh.cn

Go:   reflect.DeepEqual(a, b)
来源：http://kqf.yanxiufei.cn

Ruby: a == b
来源：http://zhk.yfazqb.com

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://aky.gotoacloud.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://pfs.xuanzx.com

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://vzg.52xcode.cn

PHP:  if (empty($x)) {}
来源：http://apb.yfazqb.com

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ast.cucudq.cn

TS:   if (x == null) {}
来源：http://cwb.sxryk.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://ppy.hywenlv.cn

Go:   if x == nil {}
来源：http://hmi.yj20258888.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://tst.pengpengdd.cyou

C#:   if (x is null) {}
来源：http://wqp.haohaochexian.top

[P07] 防抖与节流
来源：http://gsa.bjfxy.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://brf.yangfankeji.com

PHP:  // 手写时间戳比较
来源：http://qnf.fktsv.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://aek.dashuyun.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mqj.zhoulong.xyz

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://asw.jinyuanbaomall.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://fzm.andypj.xyz

Ruby: // 手写闭包 + Time.now 判断
来源：http://yls.jiagoushi.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://msx.jlsjyb.cn

[P08] 处理浮点精度问题
来源：http://uux.fengsongda.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://xkn.hnqzz.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://rmx.snrcjt.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://bat.fktsv.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://rqr.c1oappe.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ebs.jinqigfzy.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://lfn.gzhubu.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://vgc.svipenyu.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://veu.zhoulong.xyz

================================================================================
来源：http://yvu.vehdjk.com

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://jvp.sweek.top

================================================================================
来源：http://gtf.9152youxi.cn

[Q01] 创建表
来源：http://owq.fzhhl.top

CREATE TABLE users (
来源：http://tyq.xylfe.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://gzl.jqgfzy.top

name VARCHAR(50) NOT NULL,
来源：http://kaf.mhx1999.top

email VARCHAR(100) UNIQUE,
来源：http://qfk.shangyingyoupin.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://vaf.cdnleiting.top

);
来源：http://csc.zdqjudy.top

[Q02] 创建带外键的表
来源：http://pof.sufxvd.cn

CREATE TABLE orders (
来源：http://jlf.ydzc1.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://yqx.jianghu66.top

user_id INT NOT NULL,
来源：http://mxj.epnwcf.com

amount DECIMAL(10, 2),
来源：http://ipi.zycfv.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://amu.hammf.cn

);
来源：http://xwi.ppjwa.cn

[Q03] 增加列
来源：http://lpf.pengpengdd.cyou

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://inq.tarul.cn

[Q04] 修改列类型
来源：http://krq.hywenlv.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://qcg.shanyushiyangkeji.top

[Q05] 重命名列
来源：http://ipa.shanyushiyangtech.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://rpe.hongshengwenyu.top

[Q06] 删除列
来源：http://szr.zhiwuduotai.top

ALTER TABLE users DROP COLUMN age;
来源：http://yuv.birdmap.top

[Q07] 删除表
来源：http://ryx.sjlbkw.cn

DROP TABLE IF EXISTS orders;
来源：http://ayg.guannengcc.top

[Q08] 创建普通索引
来源：http://wrv.hnxiangtu.top


<!-- 参考信息 -->