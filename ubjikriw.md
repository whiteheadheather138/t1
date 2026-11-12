代发 wailian999

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://lef.yuxming.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://gxj.zdqjudy.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://krq.fktsv.cn

[L06] 解析响应为 JSON
来源：http://src.chenlongwang.top

Py:   resp.json()
来源：http://vjk.chenzaomai.com

PHP:  json_decode($body, true);
来源：http://eqa.meibo888.top

JS:   await resp.json()
来源：http://suy.svipenyu.cn

TS:   await resp.json()
来源：http://sjz.jqgfzy.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://lby.bjfxy.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://qik.fanxiaobao.xyz

Ruby: JSON.parse(resp.body)
来源：http://bui.guowangkeji.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://pif.xuetiantiany.cn

[L07] 处理 HTTP 状态码
来源：http://cmn.epnwcf.com

Py:   resp.status_code;  resp.raise_for_status()
来源：http://fod.chenzaomai.com

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ubi.cashguo.top

JS:   resp.ok;  resp.status
来源：http://lkg.iojbl.cn

TS:   resp.ok;  resp.status
来源：http://uab.c1oappe.top

Java: resp.statusCode()
来源：http://ltb.zycfv.cn

Go:   resp.StatusCode
来源：http://evr.zhengqikj.top

Ruby: resp.code.to_i
来源：http://ntm.xuetiantiany.cn

C#:   (int)resp.StatusCode
来源：http://tih.hesvh.cn

[L08] 并发请求多个地址
来源：http://oop.sweek.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://yta.jyoumei.cn

PHP:  curl_multi_init() 系列
来源：http://bpo.yfazqb.com

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://rtd.gogol.net.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://yqt.zhaomingkeji.xyz

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wtn.316326.xyz

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://uaq.316326.xyz

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://equ.hesvh.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://daw.nanxinkj.top

================================================================================
来源：http://ipc.zhiwuduotai.top

M. 命令行 / 进程 / 环境
来源：http://fud.52xcode.cn

================================================================================
来源：http://klm.xuanzx.com

[M01] 读取命令行参数
来源：http://gwx.chenjidiqi.icu

Py:   sys.argv[1:]
来源：http://qqd.shanyushiyangtech.top

PHP:  $argv;  $argc;
来源：http://tom.yangfankeji.com

JS:   process.argv.slice(2)
来源：http://krg.sweek.top

TS:   process.argv.slice(2)
来源：http://ntz.xingfuxueyuan.xyz

Java: args 数组（main 方法参数）
来源：http://myw.316326.xyz

Go:   os.Args[1:]
来源：http://xvg.cashguo.top

Ruby: ARGV
来源：http://igd.0kj1m.cn

C#:   args 数组（Main 方法参数）
来源：http://ybc.jlsjyb.cn

[M02] 读取环境变量
来源：http://xuw.xuetiantiany.cn

Py:   os.environ.get("HOME")
来源：http://kpl.yonumen.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://xcv.ydzc1.top

JS:   process.env.HOME
来源：http://ffh.shangyingyoupin.top

TS:   process.env.HOME
来源：http://zvx.hysaishi.cn

Java: System.getenv("HOME")
来源：http://qrt.yuanzhike.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hrc.uphjek.com

Ruby: ENV["HOME"]
来源：http://cmq.nwbrower.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://tlq.yongpay.top

[M03] 执行外部命令
来源：http://wky.wangshuangyany.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://bjs.hesvh.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://whx.hywenlv.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://zom.birdmap.top

TS:   child_process.execSync("ls -l").toString()
来源：http://djl.svipenyu.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://lan.smart0.xyz

Go:   exec.Command("ls", "-l").Output()
来源：http://vlx.tarul.cn

Ruby: system("ls -l");  `ls -l`
来源：http://kuq.cucudq.cn

C#:   Process.Start("ls", "-l");
来源：http://pvf.aizwys.cn

[M04] 获取当前工作目录
来源：http://iae.chenlongwang.top

Py:   os.getcwd()
来源：http://gbo.snrcjt.cn

PHP:  getcwd();
来源：http://psh.fehbvm.com

JS:   process.cwd()
来源：http://hhl.havefunace.top

TS:   process.cwd()
来源：http://hkz.cheryme.top

Java: Path.of("").toAbsolutePath()
来源：http://mfu.chenjidiqi.icu

Go:   os.Getwd()
来源：http://ntv.yanxiufei.cn

Ruby: Dir.pwd
来源：http://wcm.xuetiantiany.cn

C#:   Directory.GetCurrentDirectory()
来源：http://sqx.yj20258888.top

[M05] 设置退出码
来源：http://egl.zhaomingkeji.xyz

Py:   sys.exit(1)
来源：http://tjc.ydzc1.top

PHP:  exit(1);
来源：http://ktc.epnwcf.com

JS:   process.exit(1)
来源：http://epf.ctjpmb.com

TS:   process.exit(1)
来源：http://yzw.yj20258.top

Java: System.exit(1)
来源：http://dwd.sufxvd.cn

Go:   os.Exit(1)
来源：http://ptd.9152youxi.cn

Ruby: exit 1
来源：http://goj.hfpthk.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hlq.tanke756.top

[M06] 向标准错误输出
来源：http://iai.ywan-chungtsiang.top

Py:   print("err", file=sys.stderr)
来源：http://ctw.cheryme.top

PHP:  fwrite(STDERR, "err\n");
来源：http://igx.cdnleiting.top

JS:   console.error("err")
来源：http://qud.aizwys.cn

TS:   console.error("err")
来源：http://zqn.yueranfly.top

Java: System.err.println("err")
来源：http://cbw.zhoulong.xyz

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://pzf.yuanzhike.top

Ruby: warn "err"
来源：http://pex.jqgufenzy.top

C#:   Console.Error.WriteLine("err")
来源：http://qnc.hnqzz.top

[M07] 判断是否为主入口
来源：http://ogo.redwolf501.top

Py:   if __name__ == "__main__":
来源：http://opt.jinqigufen.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mlu.hfpthk.cn

JS:   require.main === module
来源：http://emb.quarkkingdee.top

TS:   require.main === module
来源：http://iqu.sysykeji.top

Java: public static void main(String[] args)
来源：http://oia.birdmap.top

Go:   func main()
来源：http://yhf.vehdjk.com

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://nap.hesvh.cn

C#:   static void Main(string[] args)
来源：http://jsj.yj202588.top

[M08] 获取系统与运行时信息
来源：http://css.fanxiaobao.xyz

Py:   platform.system();  platform.python_version()
来源：http://pvc.sysykeji.top

PHP:  PHP_OS;  phpversion();
来源：http://lef.birdmap.top

JS:   process.platform;  process.version
来源：http://mfi.hysaishi.cn

TS:   process.platform;  process.version
来源：http://nzo.pycfn.com

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://qrw.tianlin.xyz

Go:   runtime.GOOS;  runtime.Version()
来源：http://tbk.shanyushiyangtech.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hrn.ydjk.org.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://fkg.jinghuilouyu.cn

================================================================================
来源：http://nub.wangdashe.top

N. 数据结构与算法
来源：http://uqv.nanxuanxn.top

================================================================================
来源：http://zcw.yj202588.top

[N01] 二分查找（有序数组）
来源：http://ows.52xcode.cn

Py:   bisect.bisect_left(arr, x)
来源：http://tjj.tanke756.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://rkt.vqdsnc.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://uzk.sysykeji.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wbw.kuanghao11.cn

Java: Arrays.binarySearch(arr, x)
来源：http://owt.nanxuanxn.top

Go:   sort.SearchInts(arr, x)
来源：http://qpg.ivvv.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://boj.yanxiufei.cn

C#:   Array.BinarySearch(arr, x)
来源：http://qlo.xziqi.cn

[N02] 排序（工程实践用内置实现）
来源：http://ily.hfpthk.cn

Py:   sorted(arr);  arr.sort()
来源：http://ozw.gaohongyu789.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://tdu.shanyushiyangkeji.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://egz.bjfxy.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://syr.ctjpmb.com

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://xzt.cheryme.top

Go:   slices.Sort(arr)
来源：http://ojn.ivvv.top

Ruby: arr.sort
来源：http://wld.yangfankeji.com

C#:   Array.Sort(arr);  list.Sort()
来源：http://uvb.nanxuanxn.top

[N03] 快速排序（分治示例）
来源：http://ksh.yj20258.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://grb.hcnkem.com

PHP:  // 递归实现，或用 usort
来源：http://yiv.dianchejie.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://btz.cashguo.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://rlv.xziqi.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://dic.jinqigufen.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://rnu.hysaishi.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://gib.smart0.xyz

C#:   // 手写递归，或 Array.Sort
来源：http://kvo.gaohongyu789.top

[N04] 斐波那契数列
来源：http://uqd.yangfankeji.com

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://osq.daxiang520.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://dba.ivvv.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wbk.wangshuangyany.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://swm.pycfn.com

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://agd.zycfv.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://duu.daria6918.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://nml.fehbvm.com

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://zfb.bbcook.cn

[N05] 最大公约数
来源：http://liu.snrcjt.cn

Py:   math.gcd(a, b)
来源：http://huh.jinqigfzy.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://zkt.gzhubu.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://sjx.svipenyu.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://msf.shanyushiyangtech.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://tzl.shzxlz.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://fth.meibo888.top

Ruby: a.gcd(b)
来源：http://pdn.wangshuangyany.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://zds.nanxuanxn.top

[N06] 判断回文字符串
来源：http://cvp.ywan-chungtsiang.top

Py:   s == s[::-1]
来源：http://puv.52xcode.cn

PHP:  $s === strrev($s);
来源：http://nnj.pycfn.com

JS:   s === [...s].reverse().join("")
来源：http://tlm.0kj1m.cn

TS:   s === [...s].reverse().join("")
来源：http://shc.birdmap.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://gry.chenlongwang.top

Go:   // 双指针从两端比较
来源：http://kon.yanxiufei.cn

Ruby: s == s.reverse
来源：http://fhp.jlsjyb.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://oah.ydjk.org.cn

[N07] 两数之和（返回下标）
来源：http://gdx.vehdjk.com

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wmg.birdmap.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://lnc.xingfuxueyuan.xyz

JS:   // 手写 Map：map.set(v, i)
来源：http://jre.nanxuanxn.top

TS:   // 手写 Map<string, number>
来源：http://ypn.sweek.top

Java: // 手写 HashMap
来源：http://xov.yj202588.top

Go:   // 手写 map[int]int
来源：http://hix.bbcook.cn

Ruby: // 手写 Hash
来源：http://yog.redwolf501.top

C#:   // 手写 Dictionary<int, int>
来源：http://vma.yvedp.cn

[N08] 生成全排列
来源：http://yyw.ivvv.top

Py:   itertools.permutations(arr)
来源：http://miw.guowangkeji.top

PHP:  // 手写递归交换
来源：http://ifl.sysykeji.top

JS:   // 手写回溯递归
来源：http://rkn.zdbjq.cn

TS:   // 手写回溯递归
来源：http://jwc.hnxiangtu.top

Java: // 手写回溯递归
来源：http://vjd.andypj.xyz

Go:   // 手写回溯递归
来源：http://bxh.yonumen.top

Ruby: arr.permutation.to_a
来源：http://jju.havefunace.top

C#:   // 手写回溯递归
来源：http://rqt.316326.xyz

[N09] 栈与队列
来源：http://bjm.nwbrower.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://yps.jqgufenzy.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://yfo.tian-w.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hji.jinqigufen.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hfo.daxiang520.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://sfw.bjfxy.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://jig.zhengqikj.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://abz.zhaomingkeji.xyz

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://zex.yj20258.top

[N10] 链表节点定义
来源：http://oem.hongshengwenyu.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://rcc.andypj.xyz

PHP:  class Node { public $v; public $next = null; }
来源：http://jpe.zhengqikj.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://eyn.chenlongwang.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hjs.sjlbkw.cn

Java: class Node { int v; Node next; }
来源：http://uxw.jiagoushi.top

Go:   type Node struct { V int; Next *Node }
来源：http://nma.fanxiaobao.xyz

Ruby: Node = Struct.new(:v, :next)
来源：http://mkt.bbcook.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://ahh.guannengcc.top

[N11] 二叉树中序遍历
来源：http://rdc.vehdjk.com

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hbt.nanxinkj.top

PHP:  // 手写递归函数
来源：http://lsn.yuxming.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://frt.daria6918.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://yrl.hongshengwenyu.top

Java: // 手写递归
来源：http://yra.cashguo.top

Go:   // 手写递归
来源：http://sws.fktsv.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://dfq.yuxming.cn

C#:   // 手写递归
来源：http://djt.yuanzhike.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://zfy.nwbrower.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ugp.zhaomingkeji.xyz

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://rbl.nanxinkj.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://uri.xingfuxueyuan.xyz

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://gxe.fzhhl.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://vba.jqgufenzy.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://edg.zdbjq.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ila.yuxming.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://vel.hywenlv.cn

================================================================================
来源：http://qqb.chenzaomai.com

O. 并发与异步
来源：http://dxn.yfazqb.com

================================================================================
来源：http://ddx.cdnleiting.top

[O01] 启动一个线程
来源：http://anl.haohaochexian.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://cbg.gogol.net.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://lnp.dianchejie.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://kpl.ehwqpu.com

TS:   // 同 JS
来源：http://tmv.mhx1999.top

Java: new Thread(() -> f()).start()
来源：http://fzx.redwolf501.top

Go:   go f()
来源：http://vff.uphjek.com

Ruby: Thread.new { f }
来源：http://uwc.sxryk.cn

C#:   Task.Run(() => F());
来源：http://thb.ehwqpu.com

[O02] 使用线程池
来源：http://tlp.haohaochexian.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://zgi.kuanghao11.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://uff.ydjk.org.cn

JS:   // worker_threads 线程池
来源：http://qgw.chenjidiqi.icu

TS:   // worker_threads 线程池
来源：http://peo.sweek.top

Java: Executors.newFixedThreadPool(4)
来源：http://tnu.ehwqpu.com

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://vkw.xylfe.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://rub.ehwqpu.com

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://jiq.fktsv.cn

[O03] 加锁保护共享数据
来源：http://uau.hywenlv.cn

Py:   with lock: shared += 1
来源：http://del.hcnkem.com

PHP:  // 用 flock() 做文件锁
来源：http://uhf.vehdjk.com

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://dyf.uphjek.com

TS:   // 同 JS
来源：http://btw.jqgufenzy.top

Java: synchronized (this) { shared++; }
来源：http://mtd.yueranfly.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://fxl.yfazqb.com

Ruby: mutex.synchronize { shared += 1 }
来源：http://dax.yfazqb.com

C#:   lock (gate) { shared++; }
来源：http://pkb.yongpay.top

[O04] 定义异步函数并等待
来源：http://iqd.fzhhl.top

Py:   async def f():⏎    await g()
来源：http://sdc.jqgfzy.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://lri.jinqigfzy.top

JS:   async function f() { await g(); }
来源：http://pyl.pycfn.com

TS:   async function f(): Promise<void> { await g(); }
来源：http://qkd.ydzc1.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://jha.feifeiyinyue.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ytr.guowangkeji.top

Ruby: # 用 Fiber 或 async gem
来源：http://dzk.fktsv.cn

C#:   async Task F() { await G(); }
来源：http://jyd.shzxlz.cn

[O05] 并发执行并等待全部完成
来源：http://lxw.aibaodan.cn

Py:   asyncio.gather(*tasks)
来源：http://exo.yongpay.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://kbg.vehdjk.com

JS:   await Promise.all(tasks)
来源：http://fks.tianlin.xyz

TS:   await Promise.all(tasks)
来源：http://cfu.havefunace.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://rwa.bjfxy.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://kpr.aibaodan.cn

Ruby: threads.map(&:join)
来源：http://hrp.jiagoushi.top

C#:   await Task.WhenAll(t1, t2)
来源：http://nzh.jiagoushi.top

[O06] 使用进程池
来源：http://rhu.jinyuanbaomall.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wpv.yanxiufei.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://ccz.epnwcf.com

JS:   // child_process / cluster 模块
来源：http://shk.jyoumei.cn

TS:   // child_process / cluster 模块
来源：http://uxe.hammf.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ywh.smart0.xyz

Go:   // goroutine 已占用多核，直接并发即可
来源：http://gai.guowangkeji.top

Ruby: // fork 块
来源：http://evt.tarul.cn

C#:   Parallel.For
来源：http://qih.redwolf501.top

================================================================================
来源：http://xww.nwbrower.top

P. 常用工具函数
来源：http://bnd.yj20258.top

================================================================================
来源：http://owg.iojbl.cn

[P01] 生成 UUID
来源：http://agz.zdqjudy.top

Py:   str(uuid.uuid4())
来源：http://fps.dianchejie.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://bco.mhx1999.top

JS:   crypto.randomUUID()
来源：http://mpx.0kj1m.cn

TS:   crypto.randomUUID()
来源：http://axf.zdbjq.cn

Java: UUID.randomUUID().toString()
来源：http://zby.sweek.top

Go:   // 用 github.com/google/uuid
来源：http://jzn.cucudq.cn

Ruby: SecureRandom.uuid
来源：http://iyy.hywenlv.cn

C#:   Guid.NewGuid().ToString()
来源：http://tdv.gogol.net.cn

[P02] MD5 / SHA256 摘要
来源：http://dem.tian-w.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://bxl.vqdsnc.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://ent.jinyuanbaomall.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://twr.uphjek.com

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://tus.svipenyu.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ssm.daxiang520.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wuc.cqqwz.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://qld.fehbvm.com

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://zsq.sjlbkw.cn

[P03] 生成短随机字符串
来源：http://lwb.gaohongyu789.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://xkn.quarkkingdee.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://gxj.chenlongwang.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://bgj.9152youxi.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://bol.316326.xyz

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://riz.zdqjudy.top


<!-- 参考信息 -->