代发 wailian999

TS:   process.cwd()
来源：http://xeq.daxiang520.top

Java: Path.of("").toAbsolutePath()
来源：http://zvs.vehdjk.com

Go:   os.Getwd()
来源：http://koi.quarkkingdee.top

Ruby: Dir.pwd
来源：http://lna.cheryme.top

C#:   Directory.GetCurrentDirectory()
来源：http://gmw.snrcjt.cn

[M05] 设置退出码
来源：http://svv.yanxiufei.cn

Py:   sys.exit(1)
来源：http://buy.gaohongyu789.top

PHP:  exit(1);
来源：http://mpv.iojbl.cn

JS:   process.exit(1)
来源：http://ctm.hnxiangtu.top

TS:   process.exit(1)
来源：http://bjm.smart0.xyz

Java: System.exit(1)
来源：http://cqf.bbcook.cn

Go:   os.Exit(1)
来源：http://tmw.hongshengwenyu.top

Ruby: exit 1
来源：http://hzc.0kj1m.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ttf.meibo888.top

[M06] 向标准错误输出
来源：http://snq.jiagoushi.top

Py:   print("err", file=sys.stderr)
来源：http://ael.xuetiantiany.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://feh.meibo888.top

JS:   console.error("err")
来源：http://svl.meibo888.top

TS:   console.error("err")
来源：http://aps.epnwcf.com

Java: System.err.println("err")
来源：http://voe.cqqwz.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mby.nanxinkj.top

Ruby: warn "err"
来源：http://uqt.sxryk.cn

C#:   Console.Error.WriteLine("err")
来源：http://weu.c1oappe.top

[M07] 判断是否为主入口
来源：http://hyv.shanyushiyangtech.top

Py:   if __name__ == "__main__":
来源：http://tzz.zdbjq.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://llg.xylfe.cn

JS:   require.main === module
来源：http://iho.shangyingyoupin.top

TS:   require.main === module
来源：http://hpd.redwolf501.top

Java: public static void main(String[] args)
来源：http://ujc.quarkkingdee.top

Go:   func main()
来源：http://qdy.zdqjudy.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://iyu.zhoulong.xyz

C#:   static void Main(string[] args)
来源：http://ozy.wangdashe.top

[M08] 获取系统与运行时信息
来源：http://mmb.yj20258.top

Py:   platform.system();  platform.python_version()
来源：http://khl.dianchejie.cn

PHP:  PHP_OS;  phpversion();
来源：http://tps.yj20258888.top

JS:   process.platform;  process.version
来源：http://sdo.xuetiantiany.cn

TS:   process.platform;  process.version
来源：http://qjn.ydzc1.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://zup.zhoulong.xyz

Go:   runtime.GOOS;  runtime.Version()
来源：http://ebl.tarul.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://yfj.jinqigufen.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://tqr.xinyue.icu

================================================================================
来源：http://zja.c1oappe.top

N. 数据结构与算法
来源：http://ecw.wangdashe.top

================================================================================
来源：http://abx.jlsjyb.cn

[N01] 二分查找（有序数组）
来源：http://ecq.meibo888.top

Py:   bisect.bisect_left(arr, x)
来源：http://sba.fanxiaobao.xyz

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://tvy.svipenyu.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wcx.zhixingplan.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mds.gaohongyu789.top

Java: Arrays.binarySearch(arr, x)
来源：http://snp.jianghu66.top

Go:   sort.SearchInts(arr, x)
来源：http://wmm.zhoulong.xyz

Ruby: arr.bsearch { |e| e >= x }
来源：http://xjo.zhijiandao.cn

C#:   Array.BinarySearch(arr, x)
来源：http://wxr.yfazqb.com

[N02] 排序（工程实践用内置实现）
来源：http://lie.ehwqpu.com

Py:   sorted(arr);  arr.sort()
来源：http://ztg.xuetiantiany.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://jhv.vqdsnc.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://stu.xinyue.icu

TS:   [...arr].sort((a, b) => a - b)
来源：http://xie.jinqigfzy.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://kdq.yanxiufei.cn

Go:   slices.Sort(arr)
来源：http://pnp.fktsv.cn

Ruby: arr.sort
来源：http://jzq.316326.xyz

C#:   Array.Sort(arr);  list.Sort()
来源：http://qce.daxiang520.top

[N03] 快速排序（分治示例）
来源：http://yhy.shangyingyoupin.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ooo.redwolf501.top

PHP:  // 递归实现，或用 usort
来源：http://elg.hysaishi.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://vjq.yuxming.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://bfh.tarul.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://vaz.jlsjyb.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://gpx.redwolf501.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://xlw.hesvh.cn

C#:   // 手写递归，或 Array.Sort
来源：http://ssm.jinqigfzy.top

[N04] 斐波那契数列
来源：http://vox.zhiwuduotai.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://evb.shanyushiyangtech.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://zca.vqdsnc.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://tea.hysaishi.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ffk.hnqzz.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://iqc.aizwys.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mwf.wangshuangyany.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://iml.gzhubu.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ala.9152youxi.cn

[N05] 最大公约数
来源：http://dod.gaohongyu789.top

Py:   math.gcd(a, b)
来源：http://apt.smart0.xyz

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ypk.zdqjudy.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ayo.shanyushiyangkeji.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://frl.cqqwz.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://fyz.uphjek.com

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://szb.wangshuangyany.cn

Ruby: a.gcd(b)
来源：http://txd.chenjidiqi.icu

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://uvp.0kj1m.cn

[N06] 判断回文字符串
来源：http://jtf.shangyingyoupin.top

Py:   s == s[::-1]
来源：http://bmg.hysaishi.cn

PHP:  $s === strrev($s);
来源：http://yrr.haohaochexian.top

JS:   s === [...s].reverse().join("")
来源：http://rgd.sxryk.cn

TS:   s === [...s].reverse().join("")
来源：http://swf.fengsongda.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://zws.yuxming.cn

Go:   // 双指针从两端比较
来源：http://ktn.sxryk.cn

Ruby: s == s.reverse
来源：http://rlv.andypj.xyz

C#:   s == new string(s.Reverse().ToArray())
来源：http://hpr.52xcode.cn

[N07] 两数之和（返回下标）
来源：http://gri.ivvv.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://weh.fanxiaobao.xyz

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ktw.hywenlv.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://sfk.316326.xyz

TS:   // 手写 Map<string, number>
来源：http://rrc.feifeiyinyue.top

Java: // 手写 HashMap
来源：http://rip.tarul.cn

Go:   // 手写 map[int]int
来源：http://rew.birdmap.top

Ruby: // 手写 Hash
来源：http://nmp.smart0.xyz

C#:   // 手写 Dictionary<int, int>
来源：http://xjj.sweek.top

[N08] 生成全排列
来源：http://jmm.zdqjudy.top

Py:   itertools.permutations(arr)
来源：http://sun.guowangkeji.top

PHP:  // 手写递归交换
来源：http://ecl.aizwys.cn

JS:   // 手写回溯递归
来源：http://asz.ybcxt.top

TS:   // 手写回溯递归
来源：http://csw.tanke756.top

Java: // 手写回溯递归
来源：http://axb.ywan-chungtsiang.top

Go:   // 手写回溯递归
来源：http://dmo.chenzaomai.com

Ruby: arr.permutation.to_a
来源：http://dxb.shzxlz.cn

C#:   // 手写回溯递归
来源：http://fzx.yuxming.cn

[N09] 栈与队列
来源：http://ayd.aizwys.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://dhx.sweek.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://qyi.sxryk.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://abx.guowangkeji.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mck.yangfankeji.com

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mha.jinghuilouyu.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ohm.daria6918.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://bzn.haohaochexian.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://nac.yuanzhike.top

[N10] 链表节点定义
来源：http://trz.cqqwz.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://tva.jyoumei.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://izm.zhaomingkeji.xyz

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://zqd.shuidangran.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://qmc.aizwys.cn

Java: class Node { int v; Node next; }
来源：http://qzx.hywenlv.cn

Go:   type Node struct { V int; Next *Node }
来源：http://rcp.jinqigufen.top

Ruby: Node = Struct.new(:v, :next)
来源：http://nnc.ydjk.org.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://svb.jqgufenzy.top

[N11] 二叉树中序遍历
来源：http://zal.dianchejie.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ubx.sxryk.cn

PHP:  // 手写递归函数
来源：http://bcy.316326.xyz

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://jan.ivvv.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://bbj.fktsv.cn

Java: // 手写递归
来源：http://shf.hcnkem.com

Go:   // 手写递归
来源：http://owh.gaohongyu789.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://vpk.vehdjk.com

C#:   // 手写递归
来源：http://idh.tian-w.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://cua.fzhhl.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wwx.316326.xyz

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://tqe.pycfn.com

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://utd.fanxiaobao.xyz

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://leu.jyoumei.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hph.guowangkeji.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://qby.zycfv.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://qqi.cqqwz.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://quc.jqgufenzy.top

================================================================================
来源：http://hpi.0kj1m.cn

O. 并发与异步
来源：http://hhz.jinqigfzy.top

================================================================================
来源：http://yay.yfazqb.com

[O01] 启动一个线程
来源：http://hlc.zhijiandao.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://yqh.pengpengdd.cyou

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ipz.nanxuanxn.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://vsb.yj20258.top

TS:   // 同 JS
来源：http://mdv.fzhhl.top

Java: new Thread(() -> f()).start()
来源：http://hsv.quarkkingdee.top

Go:   go f()
来源：http://ltc.jiagoushi.top

Ruby: Thread.new { f }
来源：http://mhm.vehdjk.com

C#:   Task.Run(() => F());
来源：http://tfx.yanxiufei.cn

[O02] 使用线程池
来源：http://unb.shanyushiyangtech.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://zbf.316326.xyz

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://nvm.birdmap.top

JS:   // worker_threads 线程池
来源：http://oue.yj20258.top

TS:   // worker_threads 线程池
来源：http://lix.jqgufenzy.top

Java: Executors.newFixedThreadPool(4)
来源：http://ngx.ywan-chungtsiang.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mja.jqgfzy.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mbz.shanyushiyangtech.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ddn.zhongyouzk.top

[O03] 加锁保护共享数据
来源：http://mim.fktsv.cn

Py:   with lock: shared += 1
来源：http://dok.gotoacloud.top

PHP:  // 用 flock() 做文件锁
来源：http://way.52xcode.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mso.jinyuanbaomall.cn

TS:   // 同 JS
来源：http://nwm.gzhubu.top

Java: synchronized (this) { shared++; }
来源：http://bdf.jianghu66.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mlf.ybcxt.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://xfs.yj20258888.top

C#:   lock (gate) { shared++; }
来源：http://lug.zhongyouzk.top

[O04] 定义异步函数并等待
来源：http://uuz.snrcjt.cn

Py:   async def f():⏎    await g()
来源：http://nle.jinghuilouyu.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://fvi.andypj.xyz

JS:   async function f() { await g(); }
来源：http://tlv.yongpay.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://yxa.zhengqikj.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://jty.tanke756.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://pnc.shangyingyoupin.top

Ruby: # 用 Fiber 或 async gem
来源：http://jfp.wangdashe.top

C#:   async Task F() { await G(); }
来源：http://qel.fanxiaobao.xyz

[O05] 并发执行并等待全部完成
来源：http://ajy.zdbjq.cn

Py:   asyncio.gather(*tasks)
来源：http://std.hywenlv.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://suz.daria6918.cn

JS:   await Promise.all(tasks)
来源：http://mqs.zhongyouzk.top

TS:   await Promise.all(tasks)
来源：http://ijc.316326.xyz

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://dqd.xylfe.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://etk.hammf.cn

Ruby: threads.map(&:join)
来源：http://kur.sweek.top

C#:   await Task.WhenAll(t1, t2)
来源：http://wsj.daria6918.cn

[O06] 使用进程池
来源：http://iwh.dashuyun.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://joe.zhaomingkeji.xyz

PHP:  // pcntl_fork 或多进程队列
来源：http://vns.smart0.xyz

JS:   // child_process / cluster 模块
来源：http://rmi.yangfankeji.com

TS:   // child_process / cluster 模块
来源：http://isp.nanxinkj.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://gtn.xuetiantiany.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://nnb.gogol.net.cn

Ruby: // fork 块
来源：http://wco.ivvv.top

C#:   Parallel.For
来源：http://mcb.hywenlv.cn

================================================================================
来源：http://tkc.zhiwuduotai.top

P. 常用工具函数
来源：http://ifn.sjlbkw.cn

================================================================================
来源：http://ysy.bjfxy.top

[P01] 生成 UUID
来源：http://xcq.zhengqikj.top

Py:   str(uuid.uuid4())
来源：http://fav.hesvh.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://uia.tianlin.xyz

JS:   crypto.randomUUID()
来源：http://ngv.andypj.xyz

TS:   crypto.randomUUID()
来源：http://frd.vqdsnc.cn

Java: UUID.randomUUID().toString()
来源：http://flq.hnxiangtu.top

Go:   // 用 github.com/google/uuid
来源：http://bzk.zhongyouzk.top

Ruby: SecureRandom.uuid
来源：http://fwf.shangyingyoupin.top

C#:   Guid.NewGuid().ToString()
来源：http://pke.shanyushiyangkeji.top

[P02] MD5 / SHA256 摘要
来源：http://hkj.haohaochexian.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://rnq.yuxming.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://dsx.hnqzz.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://auk.shuidangran.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://kdw.hnqzz.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mkx.aibaodan.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://gxc.ybcxt.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://iug.zycfv.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://zll.hcnkem.com

[P03] 生成短随机字符串
来源：http://bmr.hcnkem.com

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://vmi.tanke756.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://yri.ywan-chungtsiang.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://fol.shanyushiyangtech.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://xdn.yanxiufei.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://neh.yongpay.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://rtk.yongpay.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://sst.daria6918.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hpp.yonumen.top

[P04] 求长度
来源：http://fdj.xylfe.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://clf.hongshengwenyu.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://jud.tian-w.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://tru.fktsv.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://jeo.pycfn.com

Java: list.size();  map.size();  s.length()
来源：http://nhv.gotoacloud.top

Go:   len(arr);  len(m)
来源：http://scq.dianchejie.cn

Ruby: x.length;  x.size
来源：http://rme.tarul.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://vxh.xuanzx.com

[P05] 判断两个对象内容是否相等
来源：http://ssk.vehdjk.com

Py:   a == b              # 列表与字典递归比较内容
来源：http://whi.9152youxi.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://eyl.zdbjq.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://lgo.yuanzhike.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://uxe.jyoumei.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hjh.pengpengdd.cyou

Go:   reflect.DeepEqual(a, b)
来源：http://fqw.sufxvd.cn

Ruby: a == b
来源：http://igz.nanxuanxn.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://brm.smart0.xyz

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mna.fengsongda.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://rnn.hcnkem.com

PHP:  if (empty($x)) {}
来源：http://pvq.tianlin.xyz

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://yhl.zycfv.cn

TS:   if (x == null) {}
来源：http://xww.yanxiufei.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://tqh.gzhubu.top

Go:   if x == nil {}
来源：http://izs.cashguo.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://jcv.jianghu66.top

C#:   if (x is null) {}
来源：http://eug.zhiwuduotai.top

[P07] 防抖与节流
来源：http://ywq.guowangkeji.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://dvw.aibaodan.cn

PHP:  // 手写时间戳比较
来源：http://uxb.hywenlv.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wec.jianghu66.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://pkg.bjfxy.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://qio.shuidangran.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://yit.zhixingplan.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://cfx.ywan-chungtsiang.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://vap.jlsjyb.cn

[P08] 处理浮点精度问题
来源：http://sub.sjlbkw.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ydn.svipenyu.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://vsq.iojbl.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://svo.jiagoushi.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://kjk.sjlbkw.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hft.quarkkingdee.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://jfx.zhijiandao.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mdm.jianghu66.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://dek.guannengcc.top

================================================================================
来源：http://nki.zhixingplan.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://bvs.9152youxi.cn

================================================================================
来源：http://flk.gzhubu.top

[Q01] 创建表
来源：http://uxt.tarul.cn

CREATE TABLE users (
来源：http://osk.bjfxy.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://egy.meibo888.top

name VARCHAR(50) NOT NULL,
来源：http://tlw.tianlin.xyz

email VARCHAR(100) UNIQUE,
来源：http://xsm.xziqi.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://gka.yonumen.top

);
来源：http://kxl.zycfv.cn

[Q02] 创建带外键的表
来源：http://vyb.shuidangran.top

CREATE TABLE orders (
来源：http://xxh.guowangkeji.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://vfw.jlsjyb.cn

user_id INT NOT NULL,
来源：http://sak.dashuyun.cn

amount DECIMAL(10, 2),
来源：http://qnz.xuanzx.com

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://tqs.hesvh.cn


<!-- 参考信息 -->