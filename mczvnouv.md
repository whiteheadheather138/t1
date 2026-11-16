代发 wailian999

Py:   resp.json()
来源：http://ssg.yj20258.top

PHP:  json_decode($body, true);
来源：http://mes.tian-w.cn

JS:   await resp.json()
来源：http://car.nanxuanxn.top

TS:   await resp.json()
来源：http://jkt.shanyushiyangtech.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://keu.snrcjt.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://fyu.zhoulong.xyz

Ruby: JSON.parse(resp.body)
来源：http://onj.shanyushiyangkeji.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://rib.jinqigfzy.top

[L07] 处理 HTTP 状态码
来源：http://phl.zhaomingkeji.xyz

Py:   resp.status_code;  resp.raise_for_status()
来源：http://nga.hywenlv.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hit.c1oappe.top

JS:   resp.ok;  resp.status
来源：http://hpi.ybcxt.top

TS:   resp.ok;  resp.status
来源：http://jzf.yueranfly.top

Java: resp.statusCode()
来源：http://ibf.hesvh.cn

Go:   resp.StatusCode
来源：http://qhe.meibo888.top

Ruby: resp.code.to_i
来源：http://arc.tian-w.cn

C#:   (int)resp.StatusCode
来源：http://dar.gaohongyu789.top

[L08] 并发请求多个地址
来源：http://vuu.iojbl.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://agw.iojbl.cn

PHP:  curl_multi_init() 系列
来源：http://vbu.tanke756.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://aol.yj202588.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wqn.zdqjudy.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://fud.9152youxi.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://jiv.xuanzx.com

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://kyg.ywan-chungtsiang.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://qoi.xuetiantiany.cn

================================================================================
来源：http://tty.yvedp.cn

M. 命令行 / 进程 / 环境
来源：http://fhr.cashguo.top

================================================================================
来源：http://zhi.jiagoushi.top

[M01] 读取命令行参数
来源：http://ruj.shuidangran.top

Py:   sys.argv[1:]
来源：http://npn.bjfxy.top

PHP:  $argv;  $argc;
来源：http://enx.yueranfly.top

JS:   process.argv.slice(2)
来源：http://jgn.smart0.xyz

TS:   process.argv.slice(2)
来源：http://koj.gotoacloud.top

Java: args 数组（main 方法参数）
来源：http://dmt.gaohongyu789.top

Go:   os.Args[1:]
来源：http://alf.9152youxi.cn

Ruby: ARGV
来源：http://gls.sysykeji.top

C#:   args 数组（Main 方法参数）
来源：http://yhv.chenlongwang.top

[M02] 读取环境变量
来源：http://iym.sweek.top

Py:   os.environ.get("HOME")
来源：http://ucz.shzxlz.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ftx.bbcook.cn

JS:   process.env.HOME
来源：http://duz.jinqigufen.top

TS:   process.env.HOME
来源：http://frf.zhaomingkeji.xyz

Java: System.getenv("HOME")
来源：http://ggf.ivvv.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://umz.zhiwuduotai.top

Ruby: ENV["HOME"]
来源：http://uly.nwbrower.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://cak.andypj.xyz

[M03] 执行外部命令
来源：http://gzw.jianghu66.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://xzk.chenlongwang.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://iyo.jianghu66.top

JS:   child_process.execSync("ls -l").toString()
来源：http://dkn.jinghuilouyu.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://lmm.kuanghao11.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ihp.jinghuilouyu.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://rwq.zhengqikj.top

Ruby: system("ls -l");  `ls -l`
来源：http://ekx.sjlbkw.cn

C#:   Process.Start("ls", "-l");
来源：http://shl.jinghuilouyu.cn

[M04] 获取当前工作目录
来源：http://uni.hesvh.cn

Py:   os.getcwd()
来源：http://xik.zhengqikj.top

PHP:  getcwd();
来源：http://rvc.shangyingyoupin.top

JS:   process.cwd()
来源：http://mqa.nwbrower.top

TS:   process.cwd()
来源：http://bri.jinqigufen.top

Java: Path.of("").toAbsolutePath()
来源：http://gpl.dianchejie.cn

Go:   os.Getwd()
来源：http://wyd.aizwys.cn

Ruby: Dir.pwd
来源：http://rqr.hongshengwenyu.top

C#:   Directory.GetCurrentDirectory()
来源：http://yqb.jyoumei.cn

[M05] 设置退出码
来源：http://uvj.zdqjudy.top

Py:   sys.exit(1)
来源：http://mqc.pengpengdd.cyou

PHP:  exit(1);
来源：http://nlz.316326.xyz

JS:   process.exit(1)
来源：http://jph.ydzc1.top

TS:   process.exit(1)
来源：http://vii.birdmap.top

Java: System.exit(1)
来源：http://pcl.mhx1999.top

Go:   os.Exit(1)
来源：http://fry.wangdashe.top

Ruby: exit 1
来源：http://ghu.cdnleiting.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://oah.wangdashe.top

[M06] 向标准错误输出
来源：http://qlb.gotoacloud.top

Py:   print("err", file=sys.stderr)
来源：http://ljq.yongpay.top

PHP:  fwrite(STDERR, "err\n");
来源：http://sht.zhoulong.xyz

JS:   console.error("err")
来源：http://hjj.yj20258888.top

TS:   console.error("err")
来源：http://zfo.hammf.cn

Java: System.err.println("err")
来源：http://sba.yj20258888.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://byt.shzxlz.cn

Ruby: warn "err"
来源：http://rvx.yj20258.top

C#:   Console.Error.WriteLine("err")
来源：http://ndw.kuanghao11.cn

[M07] 判断是否为主入口
来源：http://xom.hnxiangtu.top

Py:   if __name__ == "__main__":
来源：http://dcq.gaohongyu789.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://fjy.wangshuangyany.cn

JS:   require.main === module
来源：http://zmh.ydzc1.top

TS:   require.main === module
来源：http://nob.fktsv.cn

Java: public static void main(String[] args)
来源：http://raa.quarkkingdee.top

Go:   func main()
来源：http://cax.nwbrower.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://blq.guannengcc.top

C#:   static void Main(string[] args)
来源：http://qnu.meibo888.top

[M08] 获取系统与运行时信息
来源：http://xho.gogol.net.cn

Py:   platform.system();  platform.python_version()
来源：http://hts.yuanzhike.top

PHP:  PHP_OS;  phpversion();
来源：http://aty.sxryk.cn

JS:   process.platform;  process.version
来源：http://isv.zhijiandao.cn

TS:   process.platform;  process.version
来源：http://rcj.xingfuxueyuan.xyz

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://kaq.shangyingyoupin.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://kij.ctjpmb.com

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://boo.hammf.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://lcp.gzhubu.top

================================================================================
来源：http://snw.fzhhl.top

N. 数据结构与算法
来源：http://qoj.jinqigufen.top

================================================================================
来源：http://bir.epnwcf.com

[N01] 二分查找（有序数组）
来源：http://ghc.9152youxi.cn

Py:   bisect.bisect_left(arr, x)
来源：http://lgb.vehdjk.com

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://aeg.andypj.xyz

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://cld.jinqigufen.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://aok.yj20258.top

Java: Arrays.binarySearch(arr, x)
来源：http://txu.daria6918.cn

Go:   sort.SearchInts(arr, x)
来源：http://iiy.dashuyun.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://oek.jianghu66.top

C#:   Array.BinarySearch(arr, x)
来源：http://zlu.yj20258888.top

[N02] 排序（工程实践用内置实现）
来源：http://roh.andypj.xyz

Py:   sorted(arr);  arr.sort()
来源：http://ali.jyoumei.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://elb.jinyuanbaomall.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://gpk.snrcjt.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://qdp.9152youxi.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://nds.sufxvd.cn

Go:   slices.Sort(arr)
来源：http://hpm.cashguo.top

Ruby: arr.sort
来源：http://ger.yj20258888.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://tke.aizwys.cn

[N03] 快速排序（分治示例）
来源：http://nfe.yuanzhike.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://qcv.zdbjq.cn

PHP:  // 递归实现，或用 usort
来源：http://btw.zhijiandao.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://rqb.ctjpmb.com

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ago.yonumen.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://csx.ydjk.org.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://utv.xuanzx.com

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://cve.ppjwa.cn

C#:   // 手写递归，或 Array.Sort
来源：http://nri.zycfv.cn

[N04] 斐波那契数列
来源：http://tvy.ehwqpu.com

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://zsv.havefunace.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://lfg.cucudq.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://agb.yuanzhike.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://oum.sweek.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://xan.vehdjk.com

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://lub.svipenyu.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://voe.xingfuxueyuan.xyz

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://xnd.cucudq.cn

[N05] 最大公约数
来源：http://huc.zhengqikj.top

Py:   math.gcd(a, b)
来源：http://unh.ydjk.org.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://xpd.birdmap.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hgm.0kj1m.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://peu.jyoumei.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wio.gaohongyu789.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://gkb.sxryk.cn

Ruby: a.gcd(b)
来源：http://duk.zdbjq.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://dny.zdqjudy.top

[N06] 判断回文字符串
来源：http://yeq.daxiang520.top

Py:   s == s[::-1]
来源：http://bga.aibaodan.cn

PHP:  $s === strrev($s);
来源：http://qew.xylfe.cn

JS:   s === [...s].reverse().join("")
来源：http://fkf.ybcxt.top

TS:   s === [...s].reverse().join("")
来源：http://lgf.shangyingyoupin.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://fao.bbcook.cn

Go:   // 双指针从两端比较
来源：http://otw.fzhhl.top

Ruby: s == s.reverse
来源：http://yni.yj20258888.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://kqo.hysaishi.cn

[N07] 两数之和（返回下标）
来源：http://svj.sxryk.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mbb.xinyue.icu

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://vad.cheryme.top

JS:   // 手写 Map：map.set(v, i)
来源：http://rme.svipenyu.cn

TS:   // 手写 Map<string, number>
来源：http://mte.dianchejie.cn

Java: // 手写 HashMap
来源：http://ccp.tian-w.cn

Go:   // 手写 map[int]int
来源：http://nls.yfazqb.com

Ruby: // 手写 Hash
来源：http://kjx.aibaodan.cn

C#:   // 手写 Dictionary<int, int>
来源：http://ryz.zhiwuduotai.top

[N08] 生成全排列
来源：http://fqa.zhixingplan.top

Py:   itertools.permutations(arr)
来源：http://qyg.xylfe.cn

PHP:  // 手写递归交换
来源：http://bmd.andypj.xyz

JS:   // 手写回溯递归
来源：http://tbh.yfazqb.com

TS:   // 手写回溯递归
来源：http://luh.guowangkeji.top

Java: // 手写回溯递归
来源：http://rsw.gotoacloud.top

Go:   // 手写回溯递归
来源：http://npm.nanxinkj.top

Ruby: arr.permutation.to_a
来源：http://tld.xylfe.cn

C#:   // 手写回溯递归
来源：http://uac.cucudq.cn

[N09] 栈与队列
来源：http://ydu.fanxiaobao.xyz

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://zwu.zycfv.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://fih.gzhubu.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://zuu.nanxuanxn.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://cik.chenzaomai.com

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://sfo.fengsongda.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ykg.fktsv.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://puw.cucudq.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://roc.ydjk.org.cn

[N10] 链表节点定义
来源：http://ubs.hywenlv.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://zft.zhaomingkeji.xyz

PHP:  class Node { public $v; public $next = null; }
来源：http://zam.ivvv.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://bnw.sjlbkw.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://abk.zycfv.cn

Java: class Node { int v; Node next; }
来源：http://bpo.bbcook.cn

Go:   type Node struct { V int; Next *Node }
来源：http://hkr.yonumen.top

Ruby: Node = Struct.new(:v, :next)
来源：http://akm.bbcook.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://ern.ybcxt.top

[N11] 二叉树中序遍历
来源：http://aux.meibo888.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://nwp.cqqwz.cn

PHP:  // 手写递归函数
来源：http://uso.zhongyouzk.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://eoc.yangfankeji.com

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://bwz.gotoacloud.top

Java: // 手写递归
来源：http://idj.xuetiantiany.cn

Go:   // 手写递归
来源：http://npw.dianchejie.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://awx.gzhubu.top

C#:   // 手写递归
来源：http://tfh.svipenyu.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://qhu.birdmap.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://gkt.hongshengwenyu.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://kgx.vqdsnc.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://fsp.hnqzz.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://kco.ehwqpu.com

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://dou.hongshengwenyu.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://eis.shangyingyoupin.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://jtb.shzxlz.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://jga.zdbjq.cn

================================================================================
来源：http://vhb.hammf.cn

O. 并发与异步
来源：http://lew.hesvh.cn

================================================================================
来源：http://kwr.52xcode.cn

[O01] 启动一个线程
来源：http://gir.zhiwuduotai.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://vza.dianchejie.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://vjh.tian-w.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://bju.chenjidiqi.icu

TS:   // 同 JS
来源：http://pfu.guannengcc.top

Java: new Thread(() -> f()).start()
来源：http://hum.yueranfly.top

Go:   go f()
来源：http://qyh.gotoacloud.top

Ruby: Thread.new { f }
来源：http://cod.yuanzhike.top

C#:   Task.Run(() => F());
来源：http://zxu.jqgfzy.top

[O02] 使用线程池
来源：http://uwb.dianchejie.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://rxo.tanke756.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wfs.zhongyouzk.top

JS:   // worker_threads 线程池
来源：http://bqf.daxiang520.top

TS:   // worker_threads 线程池
来源：http://uiz.ehwqpu.com

Java: Executors.newFixedThreadPool(4)
来源：http://ycl.sufxvd.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://bpk.dashuyun.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://iku.mhx1999.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ykz.nanxinkj.top

[O03] 加锁保护共享数据
来源：http://uwl.havefunace.top

Py:   with lock: shared += 1
来源：http://zav.aibaodan.cn

PHP:  // 用 flock() 做文件锁
来源：http://nru.xziqi.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://bbb.yanxiufei.cn

TS:   // 同 JS
来源：http://szd.snrcjt.cn

Java: synchronized (this) { shared++; }
来源：http://bas.yj20258888.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://uxy.xziqi.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://orp.zhengqikj.top

C#:   lock (gate) { shared++; }
来源：http://mnm.hfpthk.cn

[O04] 定义异步函数并等待
来源：http://bqs.feifeiyinyue.top

Py:   async def f():⏎    await g()
来源：http://oia.gogol.net.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hog.zdqjudy.top

JS:   async function f() { await g(); }
来源：http://ngr.hnqzz.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://uja.feifeiyinyue.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://syp.xinyue.icu

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://lja.shanyushiyangtech.top

Ruby: # 用 Fiber 或 async gem
来源：http://prz.shzxlz.cn

C#:   async Task F() { await G(); }
来源：http://jnz.zdqjudy.top

[O05] 并发执行并等待全部完成
来源：http://bmr.snrcjt.cn

Py:   asyncio.gather(*tasks)
来源：http://ges.yueranfly.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wvu.xuanzx.com

JS:   await Promise.all(tasks)
来源：http://gbo.xuetiantiany.cn

TS:   await Promise.all(tasks)
来源：http://pxd.nwbrower.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://rnq.hywenlv.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://jdc.vehdjk.com

Ruby: threads.map(&:join)
来源：http://wvh.andypj.xyz

C#:   await Task.WhenAll(t1, t2)
来源：http://uuh.guowangkeji.top

[O06] 使用进程池
来源：http://tui.pengpengdd.cyou

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ywm.feifeiyinyue.top

PHP:  // pcntl_fork 或多进程队列
来源：http://zbu.nwbrower.top

JS:   // child_process / cluster 模块
来源：http://buy.cheryme.top

TS:   // child_process / cluster 模块
来源：http://won.wangshuangyany.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mda.yongpay.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ttz.cqqwz.cn

Ruby: // fork 块
来源：http://azt.bbcook.cn

C#:   Parallel.For
来源：http://klc.sufxvd.cn

================================================================================
来源：http://uag.jianghu66.top

P. 常用工具函数
来源：http://hzh.uphjek.com

================================================================================
来源：http://cew.jyoumei.cn

[P01] 生成 UUID
来源：http://kam.316326.xyz

Py:   str(uuid.uuid4())
来源：http://jvn.guannengcc.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ctq.jianghu66.top

JS:   crypto.randomUUID()
来源：http://mol.svipenyu.cn

TS:   crypto.randomUUID()
来源：http://hig.chenlongwang.top

Java: UUID.randomUUID().toString()
来源：http://rxv.jinghuilouyu.cn

Go:   // 用 github.com/google/uuid
来源：http://lho.jianghu66.top

Ruby: SecureRandom.uuid
来源：http://bhz.epnwcf.com

C#:   Guid.NewGuid().ToString()
来源：http://kre.ywan-chungtsiang.top

[P02] MD5 / SHA256 摘要
来源：http://qeu.havefunace.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://oke.gaohongyu789.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://nfe.hnxiangtu.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://agb.ydjk.org.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://fqr.xingfuxueyuan.xyz

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://odo.jqgfzy.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://xyf.ydzc1.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://urf.haohaochexian.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://sny.jiagoushi.top

[P03] 生成短随机字符串
来源：http://fcv.fehbvm.com

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://vtt.fehbvm.com

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ztd.bbcook.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://lsq.sysykeji.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://jma.fengsongda.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://peh.ctjpmb.com

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://zpw.zhoulong.xyz

Ruby: SecureRandom.alphanumeric(16)
来源：http://ojy.guowangkeji.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://shd.cheryme.top

[P04] 求长度
来源：http://cao.jlsjyb.cn


<!-- 参考信息 -->