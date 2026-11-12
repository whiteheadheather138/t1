代发 wailian999

PHP:  fwrite(STDERR, "err\n");
来源：http://fuf.jinqigfzy.top

JS:   console.error("err")
来源：http://uyg.vehdjk.com

TS:   console.error("err")
来源：http://trn.jqgufenzy.top

Java: System.err.println("err")
来源：http://llj.cdnleiting.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://upf.tian-w.cn

Ruby: warn "err"
来源：http://bxe.zdbjq.cn

C#:   Console.Error.WriteLine("err")
来源：http://tzw.zycfv.cn

[M07] 判断是否为主入口
来源：http://bvy.yanxiufei.cn

Py:   if __name__ == "__main__":
来源：http://may.ivvv.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ioj.ivvv.top

JS:   require.main === module
来源：http://hdw.yanxiufei.cn

TS:   require.main === module
来源：http://nbd.ctjpmb.com

Java: public static void main(String[] args)
来源：http://hoj.zhiwuduotai.top

Go:   func main()
来源：http://hic.andypj.xyz

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://iyl.hnqzz.top

C#:   static void Main(string[] args)
来源：http://wjw.ppjwa.cn

[M08] 获取系统与运行时信息
来源：http://vsa.wangshuangyany.cn

Py:   platform.system();  platform.python_version()
来源：http://twq.shangyingyoupin.top

PHP:  PHP_OS;  phpversion();
来源：http://ize.yuxming.cn

JS:   process.platform;  process.version
来源：http://pwp.xingfuxueyuan.xyz

TS:   process.platform;  process.version
来源：http://xhd.xziqi.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://nfh.sjlbkw.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://dfd.cashguo.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://jsc.zhixingplan.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://qnm.aibaodan.cn

================================================================================
来源：http://smp.wangshuangyany.cn

N. 数据结构与算法
来源：http://ajb.yfazqb.com

================================================================================
来源：http://udt.aibaodan.cn

[N01] 二分查找（有序数组）
来源：http://kxq.quarkkingdee.top

Py:   bisect.bisect_left(arr, x)
来源：http://bgh.yfazqb.com

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://bno.yj20258888.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://kah.xuetiantiany.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wsf.zhixingplan.top

Java: Arrays.binarySearch(arr, x)
来源：http://cjs.cucudq.cn

Go:   sort.SearchInts(arr, x)
来源：http://jdy.jqgfzy.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://wqh.havefunace.top

C#:   Array.BinarySearch(arr, x)
来源：http://mle.ivvv.top

[N02] 排序（工程实践用内置实现）
来源：http://cfq.shzxlz.cn

Py:   sorted(arr);  arr.sort()
来源：http://fdy.xinyue.icu

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://pxd.zhoulong.xyz

JS:   [...arr].sort((a, b) => a - b)
来源：http://umt.jinyuanbaomall.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://amu.pengpengdd.cyou

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://qiz.haohaochexian.top

Go:   slices.Sort(arr)
来源：http://ebc.ybcxt.top

Ruby: arr.sort
来源：http://wzy.shzxlz.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://wwm.zdbjq.cn

[N03] 快速排序（分治示例）
来源：http://dwn.chenzaomai.com

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://fki.sxryk.cn

PHP:  // 递归实现，或用 usort
来源：http://grz.bjfxy.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mmo.hesvh.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wqw.52xcode.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://zgt.gaohongyu789.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://iuh.fzhhl.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://cst.epnwcf.com

C#:   // 手写递归，或 Array.Sort
来源：http://lxk.tanke756.top

[N04] 斐波那契数列
来源：http://hdn.jqgfzy.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://rsv.epnwcf.com

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://jbb.gzhubu.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://bse.jianghu66.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ail.nanxinkj.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ljg.yfazqb.com

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ovn.ybcxt.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://fas.jinqigfzy.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://jxv.daxiang520.top

[N05] 最大公约数
来源：http://rnf.zhaomingkeji.xyz

Py:   math.gcd(a, b)
来源：http://wos.yj202588.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://xfr.yfazqb.com

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://isn.hammf.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://prw.yj202588.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://gdq.hfpthk.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://tqj.chenjidiqi.icu

Ruby: a.gcd(b)
来源：http://qwq.hcnkem.com

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ozp.jiagoushi.top

[N06] 判断回文字符串
来源：http://vno.vehdjk.com

Py:   s == s[::-1]
来源：http://pdu.zdbjq.cn

PHP:  $s === strrev($s);
来源：http://mkd.ehwqpu.com

JS:   s === [...s].reverse().join("")
来源：http://ulh.zhixingplan.top

TS:   s === [...s].reverse().join("")
来源：http://paz.tanke756.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://igv.ivvv.top

Go:   // 双指针从两端比较
来源：http://jfj.tian-w.cn

Ruby: s == s.reverse
来源：http://iyz.jinqigufen.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://vsk.redwolf501.top

[N07] 两数之和（返回下标）
来源：http://esc.gotoacloud.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://tis.hnqzz.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wod.jqgufenzy.top

JS:   // 手写 Map：map.set(v, i)
来源：http://qew.fehbvm.com

TS:   // 手写 Map<string, number>
来源：http://olh.zhiwuduotai.top

Java: // 手写 HashMap
来源：http://mnr.smart0.xyz

Go:   // 手写 map[int]int
来源：http://hmx.jiagoushi.top

Ruby: // 手写 Hash
来源：http://fkd.ehwqpu.com

C#:   // 手写 Dictionary<int, int>
来源：http://mpd.zhiwuduotai.top

[N08] 生成全排列
来源：http://dqm.xinyue.icu

Py:   itertools.permutations(arr)
来源：http://xxw.shanyushiyangtech.top

PHP:  // 手写递归交换
来源：http://ijn.ctjpmb.com

JS:   // 手写回溯递归
来源：http://kat.zycfv.cn

TS:   // 手写回溯递归
来源：http://nsx.ppjwa.cn

Java: // 手写回溯递归
来源：http://iyu.snrcjt.cn

Go:   // 手写回溯递归
来源：http://gxm.jianghu66.top

Ruby: arr.permutation.to_a
来源：http://wmy.jinyuanbaomall.cn

C#:   // 手写回溯递归
来源：http://fbe.9152youxi.cn

[N09] 栈与队列
来源：http://avh.yanxiufei.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ojg.shzxlz.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://llw.sufxvd.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://qtr.xinyue.icu

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ybv.daxiang520.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://two.yuxming.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://tvj.zycfv.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://egh.dianchejie.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://dpx.sxryk.cn

[N10] 链表节点定义
来源：http://kzs.fanxiaobao.xyz

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://agc.dashuyun.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://ciu.mhx1999.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ofu.haohaochexian.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://bts.nanxuanxn.top

Java: class Node { int v; Node next; }
来源：http://qbi.jlsjyb.cn

Go:   type Node struct { V int; Next *Node }
来源：http://dlo.tianlin.xyz

Ruby: Node = Struct.new(:v, :next)
来源：http://tdx.bbcook.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://gta.jiagoushi.top

[N11] 二叉树中序遍历
来源：http://jmz.ydzc1.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://bnd.yfazqb.com

PHP:  // 手写递归函数
来源：http://goa.gotoacloud.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://lxa.zhiwuduotai.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://jin.yonumen.top

Java: // 手写递归
来源：http://zak.mhx1999.top

Go:   // 手写递归
来源：http://myi.tanke756.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://voy.hammf.cn

C#:   // 手写递归
来源：http://ftt.hnqzz.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://fly.hysaishi.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://oci.guannengcc.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://dhi.nanxuanxn.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ezo.iojbl.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://azj.sjlbkw.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ocn.cqqwz.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://xqi.zhoulong.xyz

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://lyl.316326.xyz

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://tmf.9152youxi.cn

================================================================================
来源：http://tkq.zdqjudy.top

O. 并发与异步
来源：http://enk.yj20258.top

================================================================================
来源：http://zaz.dianchejie.cn

[O01] 启动一个线程
来源：http://qcd.gotoacloud.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://frl.yj20258.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://gfv.yj20258.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://szh.9152youxi.cn

TS:   // 同 JS
来源：http://rly.gzhubu.top

Java: new Thread(() -> f()).start()
来源：http://ngh.pengpengdd.cyou

Go:   go f()
来源：http://cve.fengsongda.top

Ruby: Thread.new { f }
来源：http://sir.fktsv.cn

C#:   Task.Run(() => F());
来源：http://odv.ehwqpu.com

[O02] 使用线程池
来源：http://joy.jinqigfzy.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://bpx.xuanzx.com

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://psz.shanyushiyangtech.top

JS:   // worker_threads 线程池
来源：http://oag.jinqigfzy.top

TS:   // worker_threads 线程池
来源：http://xup.ctjpmb.com

Java: Executors.newFixedThreadPool(4)
来源：http://war.hysaishi.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://tyi.ivvv.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://tbj.iojbl.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://nek.zhoulong.xyz

[O03] 加锁保护共享数据
来源：http://ygz.yongpay.top

Py:   with lock: shared += 1
来源：http://bav.ehwqpu.com

PHP:  // 用 flock() 做文件锁
来源：http://xxs.jqgfzy.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://pvj.mhx1999.top

TS:   // 同 JS
来源：http://owl.xuanzx.com

Java: synchronized (this) { shared++; }
来源：http://sle.fengsongda.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hqe.cucudq.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://ovw.xylfe.cn

C#:   lock (gate) { shared++; }
来源：http://fbq.ivvv.top

[O04] 定义异步函数并等待
来源：http://gvs.fzhhl.top

Py:   async def f():⏎    await g()
来源：http://yyk.jinyuanbaomall.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://izh.shuidangran.top

JS:   async function f() { await g(); }
来源：http://pgm.zhaomingkeji.xyz

TS:   async function f(): Promise<void> { await g(); }
来源：http://duj.kuanghao11.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://dgj.meibo888.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://qoo.nanxuanxn.top

Ruby: # 用 Fiber 或 async gem
来源：http://euv.hesvh.cn

C#:   async Task F() { await G(); }
来源：http://obm.havefunace.top

[O05] 并发执行并等待全部完成
来源：http://caz.mhx1999.top

Py:   asyncio.gather(*tasks)
来源：http://saq.snrcjt.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://nns.yonumen.top

JS:   await Promise.all(tasks)
来源：http://noq.aizwys.cn

TS:   await Promise.all(tasks)
来源：http://dzo.jqgfzy.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hrc.tanke756.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://jxv.0kj1m.cn

Ruby: threads.map(&:join)
来源：http://mkb.yanxiufei.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://tqo.jianghu66.top

[O06] 使用进程池
来源：http://hzi.dashuyun.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://tph.meibo888.top

PHP:  // pcntl_fork 或多进程队列
来源：http://beh.meibo888.top

JS:   // child_process / cluster 模块
来源：http://gch.hysaishi.cn

TS:   // child_process / cluster 模块
来源：http://udl.cheryme.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ejs.c1oappe.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://anb.fzhhl.top

Ruby: // fork 块
来源：http://nam.iojbl.cn

C#:   Parallel.For
来源：http://yxl.fehbvm.com

================================================================================
来源：http://sfz.tian-w.cn

P. 常用工具函数
来源：http://ipz.guannengcc.top

================================================================================
来源：http://cym.tanke756.top

[P01] 生成 UUID
来源：http://uub.gogol.net.cn

Py:   str(uuid.uuid4())
来源：http://yfm.xylfe.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://tfc.ydjk.org.cn

JS:   crypto.randomUUID()
来源：http://uxt.hesvh.cn

TS:   crypto.randomUUID()
来源：http://qev.yj20258.top

Java: UUID.randomUUID().toString()
来源：http://jef.jinqigfzy.top

Go:   // 用 github.com/google/uuid
来源：http://glr.shuidangran.top

Ruby: SecureRandom.uuid
来源：http://tyx.quarkkingdee.top

C#:   Guid.NewGuid().ToString()
来源：http://gfj.andypj.xyz

[P02] MD5 / SHA256 摘要
来源：http://lmf.ppjwa.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://jof.gaohongyu789.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://otm.zhengqikj.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://fyh.zdqjudy.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://uje.snrcjt.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://exd.c1oappe.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://yut.fengsongda.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://cdv.shzxlz.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wlk.nanxuanxn.top

[P03] 生成短随机字符串
来源：http://rsy.sysykeji.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://oqh.birdmap.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://kwj.quarkkingdee.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://vce.xziqi.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://jgz.pengpengdd.cyou

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://fbg.guowangkeji.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://liz.nwbrower.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://vxn.52xcode.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://alx.hnxiangtu.top

[P04] 求长度
来源：http://mqn.fengsongda.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hxi.hysaishi.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://gzn.jyoumei.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://oji.uphjek.com

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://vzq.daria6918.cn

Java: list.size();  map.size();  s.length()
来源：http://mco.hywenlv.cn

Go:   len(arr);  len(m)
来源：http://vyd.9152youxi.cn

Ruby: x.length;  x.size
来源：http://pip.ctjpmb.com

C#:   list.Count;  dict.Count;  s.Length
来源：http://qya.nwbrower.top

[P05] 判断两个对象内容是否相等
来源：http://mfh.bjfxy.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://luf.zhongyouzk.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://dxt.daxiang520.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://dkf.zhoulong.xyz

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ezi.ctjpmb.com

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://itx.yvedp.cn

Go:   reflect.DeepEqual(a, b)
来源：http://vyi.nanxinkj.top

Ruby: a == b
来源：http://scn.hcnkem.com

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://oaw.zhiwuduotai.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hld.yuanzhike.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hsj.xingfuxueyuan.xyz

PHP:  if (empty($x)) {}
来源：http://gjx.sufxvd.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ecm.gzhubu.top

TS:   if (x == null) {}
来源：http://qza.hcnkem.com

Java: if (x == null || x.isEmpty()) {}
来源：http://syu.hnxiangtu.top

Go:   if x == nil {}
来源：http://gxk.ybcxt.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://zwh.hesvh.cn

C#:   if (x is null) {}
来源：http://tmd.hnqzz.top

[P07] 防抖与节流
来源：http://gja.jianghu66.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://jhh.dashuyun.cn

PHP:  // 手写时间戳比较
来源：http://hqi.sjlbkw.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://otj.haohaochexian.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ntb.jinqigufen.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://sbj.tianlin.xyz

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://urq.ybcxt.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://byv.snrcjt.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://xoh.tanke756.top

[P08] 处理浮点精度问题
来源：http://upq.shanyushiyangtech.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://oul.zhengqikj.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://oxm.zhaomingkeji.xyz

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mww.yuanzhike.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://plu.shangyingyoupin.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://owl.meibo888.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ior.gogol.net.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://osy.jiagoushi.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ddk.fengsongda.top

================================================================================
来源：http://fgm.xuanzx.com

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://fzy.epnwcf.com

================================================================================
来源：http://lvv.fehbvm.com

[Q01] 创建表
来源：http://vds.52xcode.cn

CREATE TABLE users (
来源：http://sdn.quarkkingdee.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://tav.52xcode.cn

name VARCHAR(50) NOT NULL,
来源：http://ncc.shangyingyoupin.top

email VARCHAR(100) UNIQUE,
来源：http://uce.havefunace.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://vof.hnqzz.top

);
来源：http://tvf.tianlin.xyz

[Q02] 创建带外键的表
来源：http://vgt.hongshengwenyu.top

CREATE TABLE orders (
来源：http://ibk.yfazqb.com

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://gpe.uphjek.com

user_id INT NOT NULL,
来源：http://xeh.meibo888.top

amount DECIMAL(10, 2),
来源：http://kva.jiagoushi.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ecr.9152youxi.cn

);
来源：http://mmr.quarkkingdee.top

[Q03] 增加列
来源：http://uox.sysykeji.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hcc.hnxiangtu.top

[Q04] 修改列类型
来源：http://vzv.fengsongda.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ywj.hywenlv.cn

[Q05] 重命名列
来源：http://oqg.meibo888.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://cmd.daria6918.cn

[Q06] 删除列
来源：http://elj.jlsjyb.cn

ALTER TABLE users DROP COLUMN age;
来源：http://jcz.fanxiaobao.xyz

[Q07] 删除表
来源：http://kdb.redwolf501.top

DROP TABLE IF EXISTS orders;
来源：http://syf.quarkkingdee.top

[Q08] 创建普通索引
来源：http://xbo.redwolf501.top

CREATE INDEX idx_users_email ON users(email);
来源：http://mry.aizwys.cn

[Q09] 创建唯一索引
来源：http://zfo.quarkkingdee.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://nuf.316326.xyz

[Q10] 插入单行
来源：http://vle.kuanghao11.cn


<!-- 参考信息 -->