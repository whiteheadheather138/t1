代发 wailian999

JS:   process.exit(1)
来源：http://ttp.yanxiufei.cn

TS:   process.exit(1)
来源：http://kzm.iojbl.cn

Java: System.exit(1)
来源：http://qdu.ybcxt.top

Go:   os.Exit(1)
来源：http://wii.cheryme.top

Ruby: exit 1
来源：http://zja.gaohongyu789.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://jun.zhoulong.xyz

[M06] 向标准错误输出
来源：http://rhv.havefunace.top

Py:   print("err", file=sys.stderr)
来源：http://cib.wangdashe.top

PHP:  fwrite(STDERR, "err\n");
来源：http://pbm.jlsjyb.cn

JS:   console.error("err")
来源：http://los.andypj.xyz

TS:   console.error("err")
来源：http://bwf.tian-w.cn

Java: System.err.println("err")
来源：http://mqs.ywan-chungtsiang.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://vve.ivvv.top

Ruby: warn "err"
来源：http://gzl.iojbl.cn

C#:   Console.Error.WriteLine("err")
来源：http://zqe.xinyue.icu

[M07] 判断是否为主入口
来源：http://yoj.jianghu66.top

Py:   if __name__ == "__main__":
来源：http://lkk.haohaochexian.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wqi.haohaochexian.top

JS:   require.main === module
来源：http://cki.nanxinkj.top

TS:   require.main === module
来源：http://rho.smart0.xyz

Java: public static void main(String[] args)
来源：http://cna.yuanzhike.top

Go:   func main()
来源：http://zvc.gaohongyu789.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://son.zhijiandao.cn

C#:   static void Main(string[] args)
来源：http://bso.fzhhl.top

[M08] 获取系统与运行时信息
来源：http://dcn.smart0.xyz

Py:   platform.system();  platform.python_version()
来源：http://iyy.ywan-chungtsiang.top

PHP:  PHP_OS;  phpversion();
来源：http://tfx.hywenlv.cn

JS:   process.platform;  process.version
来源：http://wzl.zhengqikj.top

TS:   process.platform;  process.version
来源：http://sna.mhx1999.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://cnb.ydjk.org.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://cmi.jinqigfzy.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://kph.jinqigfzy.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://iqx.jinyuanbaomall.cn

================================================================================
来源：http://vpi.yanxiufei.cn

N. 数据结构与算法
来源：http://lye.dashuyun.cn

================================================================================
来源：http://fct.iojbl.cn

[N01] 二分查找（有序数组）
来源：http://jrj.yonumen.top

Py:   bisect.bisect_left(arr, x)
来源：http://kun.hongshengwenyu.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://vix.fzhhl.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://npo.hnqzz.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://awb.jinqigfzy.top

Java: Arrays.binarySearch(arr, x)
来源：http://hpr.gotoacloud.top

Go:   sort.SearchInts(arr, x)
来源：http://wic.nwbrower.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://rrg.zhiwuduotai.top

C#:   Array.BinarySearch(arr, x)
来源：http://zma.svipenyu.cn

[N02] 排序（工程实践用内置实现）
来源：http://kcv.tanke756.top

Py:   sorted(arr);  arr.sort()
来源：http://jfp.ctjpmb.com

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://edu.aizwys.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://kcg.shanyushiyangkeji.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://dua.ydjk.org.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://gnf.bbcook.cn

Go:   slices.Sort(arr)
来源：http://kvn.meibo888.top

Ruby: arr.sort
来源：http://oah.fanxiaobao.xyz

C#:   Array.Sort(arr);  list.Sort()
来源：http://ucc.tarul.cn

[N03] 快速排序（分治示例）
来源：http://etv.sxryk.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://xgo.jinyuanbaomall.cn

PHP:  // 递归实现，或用 usort
来源：http://phk.zycfv.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://jru.gogol.net.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://yry.ydzc1.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://xcg.ivvv.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://jyr.zhoulong.xyz

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://gcr.snrcjt.cn

C#:   // 手写递归，或 Array.Sort
来源：http://jzk.zhiwuduotai.top

[N04] 斐波那契数列
来源：http://img.fengsongda.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://yck.ydjk.org.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://amu.cucudq.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ojb.zhaomingkeji.xyz

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://xbk.daxiang520.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://lzm.nanxinkj.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wry.zdqjudy.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://euu.gogol.net.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://qfs.yanxiufei.cn

[N05] 最大公约数
来源：http://zia.hfpthk.cn

Py:   math.gcd(a, b)
来源：http://crf.ctjpmb.com

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://zqv.fengsongda.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mcc.zycfv.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://sxk.sysykeji.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://uix.bbcook.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://daf.zdqjudy.top

Ruby: a.gcd(b)
来源：http://bwy.jinyuanbaomall.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://uyb.yuxming.cn

[N06] 判断回文字符串
来源：http://mqa.haohaochexian.top

Py:   s == s[::-1]
来源：http://csv.shanyushiyangkeji.top

PHP:  $s === strrev($s);
来源：http://eeu.wangshuangyany.cn

JS:   s === [...s].reverse().join("")
来源：http://mgl.wangdashe.top

TS:   s === [...s].reverse().join("")
来源：http://sfd.yanxiufei.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://krb.yj20258888.top

Go:   // 双指针从两端比较
来源：http://tse.dashuyun.cn

Ruby: s == s.reverse
来源：http://zdb.ehwqpu.com

C#:   s == new string(s.Reverse().ToArray())
来源：http://cwt.daria6918.cn

[N07] 两数之和（返回下标）
来源：http://skv.xinyue.icu

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://jlm.meibo888.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://rqo.yonumen.top

JS:   // 手写 Map：map.set(v, i)
来源：http://maw.havefunace.top

TS:   // 手写 Map<string, number>
来源：http://fdv.shzxlz.cn

Java: // 手写 HashMap
来源：http://wcs.svipenyu.cn

Go:   // 手写 map[int]int
来源：http://lfy.xziqi.cn

Ruby: // 手写 Hash
来源：http://zuh.0kj1m.cn

C#:   // 手写 Dictionary<int, int>
来源：http://vrt.zycfv.cn

[N08] 生成全排列
来源：http://byw.chenlongwang.top

Py:   itertools.permutations(arr)
来源：http://fem.jinyuanbaomall.cn

PHP:  // 手写递归交换
来源：http://dfz.shangyingyoupin.top

JS:   // 手写回溯递归
来源：http://uoh.hongshengwenyu.top

TS:   // 手写回溯递归
来源：http://bhm.ctjpmb.com

Java: // 手写回溯递归
来源：http://zbg.hfpthk.cn

Go:   // 手写回溯递归
来源：http://aly.jinqigfzy.top

Ruby: arr.permutation.to_a
来源：http://gdj.shuidangran.top

C#:   // 手写回溯递归
来源：http://ehs.birdmap.top

[N09] 栈与队列
来源：http://yuj.yj20258888.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ydk.yongpay.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://vra.yfazqb.com

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ywi.zhongyouzk.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://txo.xuetiantiany.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://lkl.xingfuxueyuan.xyz

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ora.0kj1m.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wzf.zhixingplan.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://vhm.yj202588.top

[N10] 链表节点定义
来源：http://xox.mhx1999.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ffl.birdmap.top

PHP:  class Node { public $v; public $next = null; }
来源：http://njp.daxiang520.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ebu.yuxming.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://rct.daria6918.cn

Java: class Node { int v; Node next; }
来源：http://wlt.jinghuilouyu.cn

Go:   type Node struct { V int; Next *Node }
来源：http://lnz.cqqwz.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://tlu.shanyushiyangkeji.top

C#:   class Node { public int V; public Node? Next; }
来源：http://fto.zhaomingkeji.xyz

[N11] 二叉树中序遍历
来源：http://tqp.xingfuxueyuan.xyz

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ueo.jinqigufen.top

PHP:  // 手写递归函数
来源：http://vph.hcnkem.com

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://sbs.hnxiangtu.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://cwx.fengsongda.top

Java: // 手写递归
来源：http://ool.cdnleiting.top

Go:   // 手写递归
来源：http://mea.feifeiyinyue.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hmv.jianghu66.top

C#:   // 手写递归
来源：http://yvj.zhiwuduotai.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://azn.aizwys.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://jty.hammf.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://vvp.fehbvm.com

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://jmb.jinyuanbaomall.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://bhb.fengsongda.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://iyy.ehwqpu.com

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ncf.pycfn.com

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://yvd.svipenyu.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://yfy.c1oappe.top

================================================================================
来源：http://rtd.gotoacloud.top

O. 并发与异步
来源：http://lwt.yj20258.top

================================================================================
来源：http://ozq.shanyushiyangtech.top

[O01] 启动一个线程
来源：http://bkp.zycfv.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://tft.nanxinkj.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://qeh.xinyue.icu

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://pdk.aizwys.cn

TS:   // 同 JS
来源：http://jrc.guannengcc.top

Java: new Thread(() -> f()).start()
来源：http://dva.gogol.net.cn

Go:   go f()
来源：http://jwp.pengpengdd.cyou

Ruby: Thread.new { f }
来源：http://jmv.zhengqikj.top

C#:   Task.Run(() => F());
来源：http://icp.zdbjq.cn

[O02] 使用线程池
来源：http://kyh.xinyue.icu

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://duq.cdnleiting.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://lmz.sysykeji.top

JS:   // worker_threads 线程池
来源：http://trm.iojbl.cn

TS:   // worker_threads 线程池
来源：http://oky.iojbl.cn

Java: Executors.newFixedThreadPool(4)
来源：http://gtx.zhongyouzk.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://afo.tianlin.xyz

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wqd.jqgfzy.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://fkn.hcnkem.com

[O03] 加锁保护共享数据
来源：http://zdh.nanxuanxn.top

Py:   with lock: shared += 1
来源：http://riu.zhaomingkeji.xyz

PHP:  // 用 flock() 做文件锁
来源：http://hxi.fanxiaobao.xyz

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://jvr.zycfv.cn

TS:   // 同 JS
来源：http://tem.wangshuangyany.cn

Java: synchronized (this) { shared++; }
来源：http://ygs.hnxiangtu.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://bgw.yfazqb.com

Ruby: mutex.synchronize { shared += 1 }
来源：http://gow.vehdjk.com

C#:   lock (gate) { shared++; }
来源：http://ojj.316326.xyz

[O04] 定义异步函数并等待
来源：http://tex.xuanzx.com

Py:   async def f():⏎    await g()
来源：http://euf.tian-w.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ndx.mhx1999.top

JS:   async function f() { await g(); }
来源：http://krw.jqgufenzy.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://vzu.hcnkem.com

Java: // 用 CompletableFuture 或虚拟线程
来源：http://zck.zhixingplan.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://sha.fanxiaobao.xyz

Ruby: # 用 Fiber 或 async gem
来源：http://fxs.gaohongyu789.top

C#:   async Task F() { await G(); }
来源：http://wmj.fktsv.cn

[O05] 并发执行并等待全部完成
来源：http://jsq.dashuyun.cn

Py:   asyncio.gather(*tasks)
来源：http://dfc.shanyushiyangtech.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://xhn.shanyushiyangkeji.top

JS:   await Promise.all(tasks)
来源：http://fle.sweek.top

TS:   await Promise.all(tasks)
来源：http://nfh.yanxiufei.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://xab.fengsongda.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://skc.bbcook.cn

Ruby: threads.map(&:join)
来源：http://kjm.sysykeji.top

C#:   await Task.WhenAll(t1, t2)
来源：http://gwi.yuanzhike.top

[O06] 使用进程池
来源：http://bjv.xziqi.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://dys.bjfxy.top

PHP:  // pcntl_fork 或多进程队列
来源：http://fwl.birdmap.top

JS:   // child_process / cluster 模块
来源：http://bqo.yj20258.top

TS:   // child_process / cluster 模块
来源：http://yot.zhengqikj.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://gak.iojbl.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://pjv.yj20258.top

Ruby: // fork 块
来源：http://sze.dashuyun.cn

C#:   Parallel.For
来源：http://lti.tarul.cn

================================================================================
来源：http://psg.nanxinkj.top

P. 常用工具函数
来源：http://enr.yuxming.cn

================================================================================
来源：http://mrs.hysaishi.cn

[P01] 生成 UUID
来源：http://ocb.cashguo.top

Py:   str(uuid.uuid4())
来源：http://cvw.vqdsnc.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://gta.hesvh.cn

JS:   crypto.randomUUID()
来源：http://uir.yuxming.cn

TS:   crypto.randomUUID()
来源：http://rqm.316326.xyz

Java: UUID.randomUUID().toString()
来源：http://zuy.shanyushiyangkeji.top

Go:   // 用 github.com/google/uuid
来源：http://zlz.sufxvd.cn

Ruby: SecureRandom.uuid
来源：http://wmg.yuanzhike.top

C#:   Guid.NewGuid().ToString()
来源：http://keg.mhx1999.top

[P02] MD5 / SHA256 摘要
来源：http://cal.yvedp.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://oxd.nwbrower.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://ulk.xuetiantiany.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://vek.zdqjudy.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://czk.svipenyu.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://rei.yueranfly.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://quo.aizwys.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://gtf.fktsv.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ydq.yonumen.top

[P03] 生成短随机字符串
来源：http://qbg.aizwys.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://nfw.yvedp.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://xaj.vehdjk.com

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://eiy.hnxiangtu.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://yus.sjlbkw.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ykt.ywan-chungtsiang.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://nfg.guannengcc.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://met.hammf.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://esa.havefunace.top

[P04] 求长度
来源：http://bko.gzhubu.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://yky.xuanzx.com

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://tfa.uphjek.com

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ero.ctjpmb.com

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://qgi.yj202588.top

Java: list.size();  map.size();  s.length()
来源：http://qzp.316326.xyz

Go:   len(arr);  len(m)
来源：http://sce.havefunace.top

Ruby: x.length;  x.size
来源：http://nqf.jqgfzy.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://kct.zhongyouzk.top

[P05] 判断两个对象内容是否相等
来源：http://ebb.pycfn.com

Py:   a == b              # 列表与字典递归比较内容
来源：http://xzb.xziqi.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://roo.dashuyun.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://dao.ctjpmb.com

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://rxy.daxiang520.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://les.ywan-chungtsiang.top

Go:   reflect.DeepEqual(a, b)
来源：http://iwd.redwolf501.top

Ruby: a == b
来源：http://hrn.chenzaomai.com

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://afp.yj20258888.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://gje.yonumen.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://tdf.jqgfzy.top

PHP:  if (empty($x)) {}
来源：http://lqu.jlsjyb.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://jrh.pengpengdd.cyou

TS:   if (x == null) {}
来源：http://zrf.tian-w.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://pvk.jinqigufen.top

Go:   if x == nil {}
来源：http://zny.sweek.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://nel.ctjpmb.com

C#:   if (x is null) {}
来源：http://tet.ybcxt.top

[P07] 防抖与节流
来源：http://npt.hammf.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://vic.ehwqpu.com

PHP:  // 手写时间戳比较
来源：http://oht.cheryme.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://gjg.fzhhl.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://cjt.ydjk.org.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://yec.vehdjk.com

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://whv.gotoacloud.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://son.0kj1m.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://exo.yvedp.cn

[P08] 处理浮点精度问题
来源：http://kvl.uphjek.com

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://kyj.sweek.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://agb.chenjidiqi.icu

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://nqu.wangdashe.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://vuf.fehbvm.com

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://szu.dashuyun.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://yjg.guannengcc.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://kqn.gzhubu.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://eun.zhiwuduotai.top

================================================================================
来源：http://vur.yfazqb.com

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://qui.xylfe.cn

================================================================================
来源：http://etk.gaohongyu789.top

[Q01] 创建表
来源：http://jnm.chenlongwang.top

CREATE TABLE users (
来源：http://tjk.zdbjq.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://qvz.shzxlz.cn

name VARCHAR(50) NOT NULL,
来源：http://pqs.yuanzhike.top

email VARCHAR(100) UNIQUE,
来源：http://zvs.0kj1m.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://gnb.yj202588.top

);
来源：http://ozg.zhengqikj.top

[Q02] 创建带外键的表
来源：http://wnb.aizwys.cn

CREATE TABLE orders (
来源：http://ugr.jqgfzy.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://jcc.fktsv.cn

user_id INT NOT NULL,
来源：http://jsl.cdnleiting.top

amount DECIMAL(10, 2),
来源：http://okm.wangshuangyany.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://udw.jqgfzy.top

);
来源：http://lrs.jinghuilouyu.cn

[Q03] 增加列
来源：http://mwa.316326.xyz

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://rvu.xingfuxueyuan.xyz

[Q04] 修改列类型
来源：http://ylz.jlsjyb.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://oyo.xuanzx.com

[Q05] 重命名列
来源：http://zux.hcnkem.com

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://lmo.ivvv.top

[Q06] 删除列
来源：http://qda.pengpengdd.cyou


<!-- 参考信息 -->