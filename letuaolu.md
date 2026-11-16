代发 wailian999

Ruby: exit 1
来源：http://hpi.shzxlz.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://uns.xinyue.icu

[M06] 向标准错误输出
来源：http://reu.nanxinkj.top

Py:   print("err", file=sys.stderr)
来源：http://jws.nanxuanxn.top

PHP:  fwrite(STDERR, "err\n");
来源：http://ikl.mhx1999.top

JS:   console.error("err")
来源：http://xrn.ydjk.org.cn

TS:   console.error("err")
来源：http://fsl.jinqigufen.top

Java: System.err.println("err")
来源：http://stg.jinqigfzy.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://rro.tianlin.xyz

Ruby: warn "err"
来源：http://ogd.ehwqpu.com

C#:   Console.Error.WriteLine("err")
来源：http://nba.zhengqikj.top

[M07] 判断是否为主入口
来源：http://tqj.ydzc1.top

Py:   if __name__ == "__main__":
来源：http://dcz.daria6918.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://dox.jinyuanbaomall.cn

JS:   require.main === module
来源：http://fes.yj20258.top

TS:   require.main === module
来源：http://aza.vehdjk.com

Java: public static void main(String[] args)
来源：http://cdb.zhongyouzk.top

Go:   func main()
来源：http://hms.zhongyouzk.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://yjv.yuxming.cn

C#:   static void Main(string[] args)
来源：http://ccf.ctjpmb.com

[M08] 获取系统与运行时信息
来源：http://prc.jqgfzy.top

Py:   platform.system();  platform.python_version()
来源：http://tna.hfpthk.cn

PHP:  PHP_OS;  phpversion();
来源：http://fcn.zhiwuduotai.top

JS:   process.platform;  process.version
来源：http://mlg.gzhubu.top

TS:   process.platform;  process.version
来源：http://yiv.cdnleiting.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://zbg.cashguo.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://cob.guannengcc.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://yks.sxryk.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://jii.jinghuilouyu.cn

================================================================================
来源：http://pxw.fktsv.cn

N. 数据结构与算法
来源：http://lgu.shanyushiyangkeji.top

================================================================================
来源：http://txc.redwolf501.top

[N01] 二分查找（有序数组）
来源：http://gnh.shanyushiyangtech.top

Py:   bisect.bisect_left(arr, x)
来源：http://cqw.xziqi.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://izn.tian-w.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ypi.zhaomingkeji.xyz

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://jdu.yuanzhike.top

Java: Arrays.binarySearch(arr, x)
来源：http://wia.zhengqikj.top

Go:   sort.SearchInts(arr, x)
来源：http://vmo.fzhhl.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://cpx.ehwqpu.com

C#:   Array.BinarySearch(arr, x)
来源：http://ukb.wangshuangyany.cn

[N02] 排序（工程实践用内置实现）
来源：http://jao.ydzc1.top

Py:   sorted(arr);  arr.sort()
来源：http://cmw.birdmap.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://pqd.yvedp.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://dfv.bjfxy.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://lvc.zhongyouzk.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ran.haohaochexian.top

Go:   slices.Sort(arr)
来源：http://wiy.hywenlv.cn

Ruby: arr.sort
来源：http://aqt.fehbvm.com

C#:   Array.Sort(arr);  list.Sort()
来源：http://bbk.cucudq.cn

[N03] 快速排序（分治示例）
来源：http://fka.0kj1m.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://lnr.kuanghao11.cn

PHP:  // 递归实现，或用 usort
来源：http://wnw.xingfuxueyuan.xyz

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://kfc.0kj1m.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://vcl.zhongyouzk.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mju.fehbvm.com

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://knv.yfazqb.com

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://fwi.bbcook.cn

C#:   // 手写递归，或 Array.Sort
来源：http://piw.shangyingyoupin.top

[N04] 斐波那契数列
来源：http://nyo.chenzaomai.com

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://yij.52xcode.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://fum.gaohongyu789.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://lef.hcnkem.com

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://zwj.zhoulong.xyz

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://tuj.yuanzhike.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://rcp.zdqjudy.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://epy.shanyushiyangkeji.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://azd.pengpengdd.cyou

[N05] 最大公约数
来源：http://cny.yanxiufei.cn

Py:   math.gcd(a, b)
来源：http://cng.dianchejie.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://bod.gaohongyu789.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://lav.hysaishi.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://itz.guowangkeji.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://dxn.aizwys.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://xqh.shuidangran.top

Ruby: a.gcd(b)
来源：http://mld.ppjwa.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://qzt.0kj1m.cn

[N06] 判断回文字符串
来源：http://lid.jlsjyb.cn

Py:   s == s[::-1]
来源：http://tur.vqdsnc.cn

PHP:  $s === strrev($s);
来源：http://kxo.meibo888.top

JS:   s === [...s].reverse().join("")
来源：http://edr.bbcook.cn

TS:   s === [...s].reverse().join("")
来源：http://eso.pycfn.com

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://buw.xuanzx.com

Go:   // 双指针从两端比较
来源：http://xps.zhijiandao.cn

Ruby: s == s.reverse
来源：http://rqc.fengsongda.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://dqf.aibaodan.cn

[N07] 两数之和（返回下标）
来源：http://vuh.yuanzhike.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://lih.ctjpmb.com

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ixt.yanxiufei.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://okq.jinqigfzy.top

TS:   // 手写 Map<string, number>
来源：http://lpd.xuanzx.com

Java: // 手写 HashMap
来源：http://ble.yongpay.top

Go:   // 手写 map[int]int
来源：http://nmn.ctjpmb.com

Ruby: // 手写 Hash
来源：http://ryi.ehwqpu.com

C#:   // 手写 Dictionary<int, int>
来源：http://xjz.sweek.top

[N08] 生成全排列
来源：http://mjq.wangshuangyany.cn

Py:   itertools.permutations(arr)
来源：http://sbb.yonumen.top

PHP:  // 手写递归交换
来源：http://zjc.guannengcc.top

JS:   // 手写回溯递归
来源：http://wsn.fengsongda.top

TS:   // 手写回溯递归
来源：http://uvl.zhoulong.xyz

Java: // 手写回溯递归
来源：http://wsk.jiagoushi.top

Go:   // 手写回溯递归
来源：http://epq.meibo888.top

Ruby: arr.permutation.to_a
来源：http://epw.hnxiangtu.top

C#:   // 手写回溯递归
来源：http://efs.yueranfly.top

[N09] 栈与队列
来源：http://pbo.zhaomingkeji.xyz

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://bmm.c1oappe.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://gur.zhijiandao.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://gkd.zycfv.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://upy.jyoumei.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://fis.yj20258.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://bal.sweek.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://bgl.xuanzx.com

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://lpp.xuetiantiany.cn

[N10] 链表节点定义
来源：http://cns.guowangkeji.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://aiv.bbcook.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://una.hysaishi.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://kdv.yuxming.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://maw.c1oappe.top

Java: class Node { int v; Node next; }
来源：http://tzh.gotoacloud.top

Go:   type Node struct { V int; Next *Node }
来源：http://fku.meibo888.top

Ruby: Node = Struct.new(:v, :next)
来源：http://mps.zhengqikj.top

C#:   class Node { public int V; public Node? Next; }
来源：http://tge.xuetiantiany.cn

[N11] 二叉树中序遍历
来源：http://ppx.zdqjudy.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://lwp.bjfxy.top

PHP:  // 手写递归函数
来源：http://dkk.c1oappe.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ope.tanke756.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://qjw.redwolf501.top

Java: // 手写递归
来源：http://rdb.shzxlz.cn

Go:   // 手写递归
来源：http://lqy.chenjidiqi.icu

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://sgf.fehbvm.com

C#:   // 手写递归
来源：http://tmb.chenlongwang.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://bjg.hnqzz.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://oxl.fktsv.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://dgv.yvedp.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://nnu.gotoacloud.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://see.yvedp.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://etv.yj20258.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://tqk.zhixingplan.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://qjy.xylfe.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://aec.smart0.xyz

================================================================================
来源：http://crt.mhx1999.top

O. 并发与异步
来源：http://aqh.ehwqpu.com

================================================================================
来源：http://owj.zhongyouzk.top

[O01] 启动一个线程
来源：http://yxi.epnwcf.com

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://nyh.fktsv.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://yfm.yongpay.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://dkz.ywan-chungtsiang.top

TS:   // 同 JS
来源：http://kgo.sysykeji.top

Java: new Thread(() -> f()).start()
来源：http://keq.vqdsnc.cn

Go:   go f()
来源：http://utm.xuanzx.com

Ruby: Thread.new { f }
来源：http://yyu.yfazqb.com

C#:   Task.Run(() => F());
来源：http://zsk.jianghu66.top

[O02] 使用线程池
来源：http://vzu.zhijiandao.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://jdg.gzhubu.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://lan.hesvh.cn

JS:   // worker_threads 线程池
来源：http://hth.jinyuanbaomall.cn

TS:   // worker_threads 线程池
来源：http://flk.birdmap.top

Java: Executors.newFixedThreadPool(4)
来源：http://gii.jyoumei.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://kph.yuanzhike.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://daa.nwbrower.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mur.feifeiyinyue.top

[O03] 加锁保护共享数据
来源：http://vus.52xcode.cn

Py:   with lock: shared += 1
来源：http://iox.fehbvm.com

PHP:  // 用 flock() 做文件锁
来源：http://yln.wangdashe.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ihw.c1oappe.top

TS:   // 同 JS
来源：http://myt.0kj1m.cn

Java: synchronized (this) { shared++; }
来源：http://rmk.jyoumei.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://kdn.gaohongyu789.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://nbg.andypj.xyz

C#:   lock (gate) { shared++; }
来源：http://bba.snrcjt.cn

[O04] 定义异步函数并等待
来源：http://mbf.fehbvm.com

Py:   async def f():⏎    await g()
来源：http://ubc.hcnkem.com

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://zsb.bbcook.cn

JS:   async function f() { await g(); }
来源：http://lnr.epnwcf.com

TS:   async function f(): Promise<void> { await g(); }
来源：http://vdi.tianlin.xyz

Java: // 用 CompletableFuture 或虚拟线程
来源：http://qlw.9152youxi.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://dwa.haohaochexian.top

Ruby: # 用 Fiber 或 async gem
来源：http://wev.tanke756.top

C#:   async Task F() { await G(); }
来源：http://fgx.jinghuilouyu.cn

[O05] 并发执行并等待全部完成
来源：http://alo.cashguo.top

Py:   asyncio.gather(*tasks)
来源：http://zhj.guowangkeji.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://dry.hcnkem.com

JS:   await Promise.all(tasks)
来源：http://big.uphjek.com

TS:   await Promise.all(tasks)
来源：http://mdn.svipenyu.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://vjz.yj202588.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://rlo.zdbjq.cn

Ruby: threads.map(&:join)
来源：http://ctd.yvedp.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://puu.tianlin.xyz

[O06] 使用进程池
来源：http://jbd.meibo888.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://vpf.hfpthk.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://fos.sufxvd.cn

JS:   // child_process / cluster 模块
来源：http://mqe.316326.xyz

TS:   // child_process / cluster 模块
来源：http://krk.hesvh.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://cwl.redwolf501.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://vds.ivvv.top

Ruby: // fork 块
来源：http://gta.uphjek.com

C#:   Parallel.For
来源：http://ple.52xcode.cn

================================================================================
来源：http://kna.ydjk.org.cn

P. 常用工具函数
来源：http://yid.zhaomingkeji.xyz

================================================================================
来源：http://zyj.jqgufenzy.top

[P01] 生成 UUID
来源：http://yln.dianchejie.cn

Py:   str(uuid.uuid4())
来源：http://tjg.gogol.net.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://cvq.chenlongwang.top

JS:   crypto.randomUUID()
来源：http://clk.yj20258.top

TS:   crypto.randomUUID()
来源：http://kxn.vqdsnc.cn

Java: UUID.randomUUID().toString()
来源：http://gbm.hfpthk.cn

Go:   // 用 github.com/google/uuid
来源：http://tah.hfpthk.cn

Ruby: SecureRandom.uuid
来源：http://cuf.fktsv.cn

C#:   Guid.NewGuid().ToString()
来源：http://wok.yj202588.top

[P02] MD5 / SHA256 摘要
来源：http://vcr.shanyushiyangkeji.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://tin.sweek.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://wqg.zdbjq.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://rrh.zdbjq.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mcp.nwbrower.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ngt.zhijiandao.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://kwx.yanxiufei.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://afg.xylfe.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://crh.jiagoushi.top

[P03] 生成短随机字符串
来源：http://pbk.zhaomingkeji.xyz

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://xyb.hesvh.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://sns.chenlongwang.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://dxn.cqqwz.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://obp.chenzaomai.com

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://nbg.hongshengwenyu.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://jxr.dashuyun.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://bqz.nwbrower.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://zhr.shanyushiyangtech.top

[P04] 求长度
来源：http://fgz.havefunace.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://dto.pycfn.com

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://jsp.shanyushiyangkeji.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ibo.sjlbkw.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://loz.jinyuanbaomall.cn

Java: list.size();  map.size();  s.length()
来源：http://iyo.daxiang520.top

Go:   len(arr);  len(m)
来源：http://rlq.jqgufenzy.top

Ruby: x.length;  x.size
来源：http://zns.xinyue.icu

C#:   list.Count;  dict.Count;  s.Length
来源：http://loa.xingfuxueyuan.xyz

[P05] 判断两个对象内容是否相等
来源：http://abt.daxiang520.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://rgu.jinyuanbaomall.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ngw.jinqigfzy.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://pex.uphjek.com

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://pdi.yueranfly.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ubk.yvedp.cn

Go:   reflect.DeepEqual(a, b)
来源：http://pjo.zhongyouzk.top

Ruby: a == b
来源：http://vis.cashguo.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://evd.tanke756.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://paa.hnxiangtu.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://jin.ehwqpu.com

PHP:  if (empty($x)) {}
来源：http://hqc.jinqigufen.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://jzo.meibo888.top

TS:   if (x == null) {}
来源：http://bhj.aizwys.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://juy.xylfe.cn

Go:   if x == nil {}
来源：http://eqv.xylfe.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://jdb.sxryk.cn

C#:   if (x is null) {}
来源：http://zdf.sjlbkw.cn

[P07] 防抖与节流
来源：http://wxg.9152youxi.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ubg.tarul.cn

PHP:  // 手写时间戳比较
来源：http://cpa.zhoulong.xyz

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://oaz.uphjek.com

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://thh.cucudq.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://lqd.chenjidiqi.icu

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hvp.zhixingplan.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://cpi.9152youxi.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://zvx.tianlin.xyz

[P08] 处理浮点精度问题
来源：http://yvy.vqdsnc.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://cgx.guowangkeji.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://nsx.zdqjudy.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ynl.jiagoushi.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://jfg.hammf.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://dxy.vqdsnc.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wme.fehbvm.com

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ndf.yvedp.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://nxq.chenzaomai.com

================================================================================
来源：http://ect.feifeiyinyue.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://xku.shzxlz.cn

================================================================================
来源：http://jew.shzxlz.cn

[Q01] 创建表
来源：http://acy.ppjwa.cn

CREATE TABLE users (
来源：http://tau.yvedp.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hyh.pycfn.com

name VARCHAR(50) NOT NULL,
来源：http://kwe.sxryk.cn

email VARCHAR(100) UNIQUE,
来源：http://kjm.nanxinkj.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://tnx.cdnleiting.top

);
来源：http://hfd.shanyushiyangtech.top

[Q02] 创建带外键的表
来源：http://cwp.cheryme.top

CREATE TABLE orders (
来源：http://icl.daria6918.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ird.tianlin.xyz

user_id INT NOT NULL,
来源：http://geh.yj20258888.top

amount DECIMAL(10, 2),
来源：http://uwr.xylfe.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://omz.ehwqpu.com

);
来源：http://yml.52xcode.cn

[Q03] 增加列
来源：http://szq.gzhubu.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://nwa.tian-w.cn

[Q04] 修改列类型
来源：http://jje.tarul.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://sih.fengsongda.top

[Q05] 重命名列
来源：http://gqd.zhongyouzk.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ila.vqdsnc.cn

[Q06] 删除列
来源：http://xtb.zhijiandao.cn

ALTER TABLE users DROP COLUMN age;
来源：http://dxn.ywan-chungtsiang.top

[Q07] 删除表
来源：http://tpu.9152youxi.cn

DROP TABLE IF EXISTS orders;
来源：http://aat.zdbjq.cn

[Q08] 创建普通索引
来源：http://sak.sxryk.cn


<!-- 参考信息 -->