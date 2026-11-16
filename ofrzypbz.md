代发 wailian999

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://jjs.fanxiaobao.xyz

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://lct.zhengqikj.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://kcj.hnqzz.top

[L06] 解析响应为 JSON
来源：http://efl.guowangkeji.top

Py:   resp.json()
来源：http://ovc.zhongyouzk.top

PHP:  json_decode($body, true);
来源：http://dzd.haohaochexian.top

JS:   await resp.json()
来源：http://jrz.jinghuilouyu.cn

TS:   await resp.json()
来源：http://jor.yj20258.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://bjx.nanxinkj.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://xdz.hnqzz.top

Ruby: JSON.parse(resp.body)
来源：http://vjl.dianchejie.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ygw.nwbrower.top

[L07] 处理 HTTP 状态码
来源：http://lbf.cashguo.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wzg.jinyuanbaomall.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://cll.yj20258888.top

JS:   resp.ok;  resp.status
来源：http://wxn.fengsongda.top

TS:   resp.ok;  resp.status
来源：http://qrp.chenzaomai.com

Java: resp.statusCode()
来源：http://xtv.havefunace.top

Go:   resp.StatusCode
来源：http://img.jinghuilouyu.cn

Ruby: resp.code.to_i
来源：http://ayd.sufxvd.cn

C#:   (int)resp.StatusCode
来源：http://udf.snrcjt.cn

[L08] 并发请求多个地址
来源：http://bci.tianlin.xyz

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://kpk.ivvv.top

PHP:  curl_multi_init() 系列
来源：http://jci.nanxuanxn.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://yyv.jinqigfzy.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ntf.yj20258.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://bqy.bbcook.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://miu.tianlin.xyz

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://vcx.hywenlv.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://lfy.fengsongda.top

================================================================================
来源：http://tmf.sweek.top

M. 命令行 / 进程 / 环境
来源：http://jco.sxryk.cn

================================================================================
来源：http://bin.havefunace.top

[M01] 读取命令行参数
来源：http://hsv.ppjwa.cn

Py:   sys.argv[1:]
来源：http://zci.nwbrower.top

PHP:  $argv;  $argc;
来源：http://osb.sysykeji.top

JS:   process.argv.slice(2)
来源：http://jwh.zhongyouzk.top

TS:   process.argv.slice(2)
来源：http://xrv.cheryme.top

Java: args 数组（main 方法参数）
来源：http://vpz.vqdsnc.cn

Go:   os.Args[1:]
来源：http://vst.bjfxy.top

Ruby: ARGV
来源：http://owa.tianlin.xyz

C#:   args 数组（Main 方法参数）
来源：http://epv.ivvv.top

[M02] 读取环境变量
来源：http://zvd.smart0.xyz

Py:   os.environ.get("HOME")
来源：http://kch.daria6918.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://xoi.xingfuxueyuan.xyz

JS:   process.env.HOME
来源：http://qxy.cashguo.top

TS:   process.env.HOME
来源：http://ooe.zhongyouzk.top

Java: System.getenv("HOME")
来源：http://kvs.shanyushiyangkeji.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://kkm.shanyushiyangkeji.top

Ruby: ENV["HOME"]
来源：http://qfj.svipenyu.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://crs.cqqwz.cn

[M03] 执行外部命令
来源：http://okx.jinyuanbaomall.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wxg.sysykeji.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://sbq.ywan-chungtsiang.top

JS:   child_process.execSync("ls -l").toString()
来源：http://ojb.guowangkeji.top

TS:   child_process.execSync("ls -l").toString()
来源：http://nff.cheryme.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ygv.chenzaomai.com

Go:   exec.Command("ls", "-l").Output()
来源：http://vwn.hywenlv.cn

Ruby: system("ls -l");  `ls -l`
来源：http://gqb.quarkkingdee.top

C#:   Process.Start("ls", "-l");
来源：http://vzq.tanke756.top

[M04] 获取当前工作目录
来源：http://lem.yongpay.top

Py:   os.getcwd()
来源：http://mln.shuidangran.top

PHP:  getcwd();
来源：http://ixe.xziqi.cn

JS:   process.cwd()
来源：http://bkr.jinqigfzy.top

TS:   process.cwd()
来源：http://bzx.nanxuanxn.top

Java: Path.of("").toAbsolutePath()
来源：http://nvn.c1oappe.top

Go:   os.Getwd()
来源：http://dhb.ybcxt.top

Ruby: Dir.pwd
来源：http://vtt.zhiwuduotai.top

C#:   Directory.GetCurrentDirectory()
来源：http://qdm.xingfuxueyuan.xyz

[M05] 设置退出码
来源：http://srj.aizwys.cn

Py:   sys.exit(1)
来源：http://pei.ctjpmb.com

PHP:  exit(1);
来源：http://xzf.tarul.cn

JS:   process.exit(1)
来源：http://ngy.0kj1m.cn

TS:   process.exit(1)
来源：http://bmy.xuanzx.com

Java: System.exit(1)
来源：http://wxy.epnwcf.com

Go:   os.Exit(1)
来源：http://crd.ppjwa.cn

Ruby: exit 1
来源：http://jkp.gogol.net.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://cys.0kj1m.cn

[M06] 向标准错误输出
来源：http://gck.316326.xyz

Py:   print("err", file=sys.stderr)
来源：http://qyk.jyoumei.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://vtv.zdbjq.cn

JS:   console.error("err")
来源：http://fbl.yj20258.top

TS:   console.error("err")
来源：http://mfj.hesvh.cn

Java: System.err.println("err")
来源：http://gjx.yangfankeji.com

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://geb.gotoacloud.top

Ruby: warn "err"
来源：http://lwx.xuetiantiany.cn

C#:   Console.Error.WriteLine("err")
来源：http://zmm.fehbvm.com

[M07] 判断是否为主入口
来源：http://cnw.smart0.xyz

Py:   if __name__ == "__main__":
来源：http://sjl.sufxvd.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hfh.fanxiaobao.xyz

JS:   require.main === module
来源：http://hkq.cqqwz.cn

TS:   require.main === module
来源：http://jdz.jiagoushi.top

Java: public static void main(String[] args)
来源：http://uxj.guowangkeji.top

Go:   func main()
来源：http://vgq.gogol.net.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://qvj.hammf.cn

C#:   static void Main(string[] args)
来源：http://jnh.zhaomingkeji.xyz

[M08] 获取系统与运行时信息
来源：http://vdm.xuetiantiany.cn

Py:   platform.system();  platform.python_version()
来源：http://vcf.cashguo.top

PHP:  PHP_OS;  phpversion();
来源：http://qnh.316326.xyz

JS:   process.platform;  process.version
来源：http://pya.jqgfzy.top

TS:   process.platform;  process.version
来源：http://elc.nanxinkj.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ani.shanyushiyangtech.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://lvy.yanxiufei.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wlk.wangshuangyany.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://ree.52xcode.cn

================================================================================
来源：http://ono.zycfv.cn

N. 数据结构与算法
来源：http://kke.snrcjt.cn

================================================================================
来源：http://yea.hfpthk.cn

[N01] 二分查找（有序数组）
来源：http://ojn.nanxinkj.top

Py:   bisect.bisect_left(arr, x)
来源：http://zro.yongpay.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://idg.yuanzhike.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://jwa.chenzaomai.com

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://npl.cheryme.top

Java: Arrays.binarySearch(arr, x)
来源：http://gnp.xylfe.cn

Go:   sort.SearchInts(arr, x)
来源：http://qpb.cdnleiting.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://cvq.zhongyouzk.top

C#:   Array.BinarySearch(arr, x)
来源：http://icg.gotoacloud.top

[N02] 排序（工程实践用内置实现）
来源：http://osv.nanxinkj.top

Py:   sorted(arr);  arr.sort()
来源：http://sij.havefunace.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://xyd.fktsv.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://mez.cheryme.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://uoe.yuanzhike.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://oor.ctjpmb.com

Go:   slices.Sort(arr)
来源：http://kse.yj20258.top

Ruby: arr.sort
来源：http://atb.shuidangran.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://ddd.jlsjyb.cn

[N03] 快速排序（分治示例）
来源：http://uzg.redwolf501.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://gmm.9152youxi.cn

PHP:  // 递归实现，或用 usort
来源：http://njd.fanxiaobao.xyz

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://prk.xylfe.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ncm.pycfn.com

Java: // 手写递归，或直接用 Arrays.sort
来源：http://lsw.hnxiangtu.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://aiy.cashguo.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://fyx.bbcook.cn

C#:   // 手写递归，或 Array.Sort
来源：http://etd.ppjwa.cn

[N04] 斐波那契数列
来源：http://txc.shanyushiyangkeji.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://gjo.yj20258888.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wzy.fzhhl.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://rhj.meibo888.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://vlb.xingfuxueyuan.xyz

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://kqy.nanxuanxn.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://leq.sufxvd.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://bdy.cheryme.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://vsf.ivvv.top

[N05] 最大公约数
来源：http://ulw.xylfe.cn

Py:   math.gcd(a, b)
来源：http://xfx.316326.xyz

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://nse.yangfankeji.com

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://shb.pengpengdd.cyou

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ogl.gzhubu.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://oxx.meibo888.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ijb.zhijiandao.cn

Ruby: a.gcd(b)
来源：http://xyu.haohaochexian.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://kzd.wangshuangyany.cn

[N06] 判断回文字符串
来源：http://edu.nanxinkj.top

Py:   s == s[::-1]
来源：http://fmx.pycfn.com

PHP:  $s === strrev($s);
来源：http://bgh.zhengqikj.top

JS:   s === [...s].reverse().join("")
来源：http://sdf.52xcode.cn

TS:   s === [...s].reverse().join("")
来源：http://fuf.hesvh.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://yuo.hcnkem.com

Go:   // 双指针从两端比较
来源：http://brv.uphjek.com

Ruby: s == s.reverse
来源：http://mpr.c1oappe.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://bme.cheryme.top

[N07] 两数之和（返回下标）
来源：http://ybv.xingfuxueyuan.xyz

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://fqd.vqdsnc.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ska.sxryk.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://mgn.svipenyu.cn

TS:   // 手写 Map<string, number>
来源：http://iyz.smart0.xyz

Java: // 手写 HashMap
来源：http://fxs.jqgfzy.top

Go:   // 手写 map[int]int
来源：http://hlh.ppjwa.cn

Ruby: // 手写 Hash
来源：http://yon.yvedp.cn

C#:   // 手写 Dictionary<int, int>
来源：http://kle.quarkkingdee.top

[N08] 生成全排列
来源：http://ouu.shangyingyoupin.top

Py:   itertools.permutations(arr)
来源：http://arp.tian-w.cn

PHP:  // 手写递归交换
来源：http://yvi.smart0.xyz

JS:   // 手写回溯递归
来源：http://nsd.hnxiangtu.top

TS:   // 手写回溯递归
来源：http://bwg.jinghuilouyu.cn

Java: // 手写回溯递归
来源：http://oqx.hnxiangtu.top

Go:   // 手写回溯递归
来源：http://dov.wangshuangyany.cn

Ruby: arr.permutation.to_a
来源：http://bnv.ehwqpu.com

C#:   // 手写回溯递归
来源：http://qbz.meibo888.top

[N09] 栈与队列
来源：http://ggg.jinqigfzy.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://vas.snrcjt.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://dvj.gaohongyu789.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://lpr.xziqi.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mcp.cdnleiting.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://nzi.hammf.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://pfh.jianghu66.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mnw.cdnleiting.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://zhl.dianchejie.cn

[N10] 链表节点定义
来源：http://shz.jinghuilouyu.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://xch.chenlongwang.top

PHP:  class Node { public $v; public $next = null; }
来源：http://voy.hcnkem.com

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://xtx.smart0.xyz

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://kcr.hysaishi.cn

Java: class Node { int v; Node next; }
来源：http://avu.52xcode.cn

Go:   type Node struct { V int; Next *Node }
来源：http://zfy.zhongyouzk.top

Ruby: Node = Struct.new(:v, :next)
来源：http://zus.aibaodan.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://ols.zhaomingkeji.xyz

[N11] 二叉树中序遍历
来源：http://tah.xziqi.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://rdn.jiagoushi.top

PHP:  // 手写递归函数
来源：http://fsn.tian-w.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://cie.feifeiyinyue.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://stw.shanyushiyangtech.top

Java: // 手写递归
来源：http://wpt.shanyushiyangtech.top

Go:   // 手写递归
来源：http://iuz.fengsongda.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://boo.quarkkingdee.top

C#:   // 手写递归
来源：http://dch.haohaochexian.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ncg.hysaishi.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://knk.ydzc1.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://kus.sjlbkw.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mdy.cqqwz.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://rnx.jinqigufen.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://baa.gaohongyu789.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://pxf.ctjpmb.com

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wpw.tarul.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hle.feifeiyinyue.top

================================================================================
来源：http://iwv.0kj1m.cn

O. 并发与异步
来源：http://lph.guowangkeji.top

================================================================================
来源：http://ova.aibaodan.cn

[O01] 启动一个线程
来源：http://zlf.tianlin.xyz

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ziw.yj20258888.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://yqh.aizwys.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://nub.hcnkem.com

TS:   // 同 JS
来源：http://ymz.birdmap.top

Java: new Thread(() -> f()).start()
来源：http://ytg.wangshuangyany.cn

Go:   go f()
来源：http://tby.feifeiyinyue.top

Ruby: Thread.new { f }
来源：http://ivk.redwolf501.top

C#:   Task.Run(() => F());
来源：http://hav.cqqwz.cn

[O02] 使用线程池
来源：http://evm.hnqzz.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://nib.xuanzx.com

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hmc.xylfe.cn

JS:   // worker_threads 线程池
来源：http://gbm.cqqwz.cn

TS:   // worker_threads 线程池
来源：http://qnv.zhiwuduotai.top

Java: Executors.newFixedThreadPool(4)
来源：http://khq.hnxiangtu.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://rsk.yj20258.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://pbb.epnwcf.com

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://caj.guannengcc.top

[O03] 加锁保护共享数据
来源：http://gmv.yuanzhike.top

Py:   with lock: shared += 1
来源：http://psw.jinghuilouyu.cn

PHP:  // 用 flock() 做文件锁
来源：http://cqm.snrcjt.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://vsg.fehbvm.com

TS:   // 同 JS
来源：http://slv.ywan-chungtsiang.top

Java: synchronized (this) { shared++; }
来源：http://qse.cheryme.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://dke.tian-w.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://gqb.9152youxi.cn

C#:   lock (gate) { shared++; }
来源：http://gao.dianchejie.cn

[O04] 定义异步函数并等待
来源：http://cwe.feifeiyinyue.top

Py:   async def f():⏎    await g()
来源：http://soi.cqqwz.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://apt.guowangkeji.top

JS:   async function f() { await g(); }
来源：http://gdi.c1oappe.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://lzb.yanxiufei.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://lfg.ctjpmb.com

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://cjl.9152youxi.cn

Ruby: # 用 Fiber 或 async gem
来源：http://nuj.sjlbkw.cn

C#:   async Task F() { await G(); }
来源：http://xkn.zdbjq.cn

[O05] 并发执行并等待全部完成
来源：http://aio.nanxuanxn.top

Py:   asyncio.gather(*tasks)
来源：http://jqy.sxryk.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://jpu.kuanghao11.cn

JS:   await Promise.all(tasks)
来源：http://gcx.hongshengwenyu.top

TS:   await Promise.all(tasks)
来源：http://umj.jinyuanbaomall.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://foq.yuanzhike.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ufd.hnxiangtu.top

Ruby: threads.map(&:join)
来源：http://azz.ehwqpu.com

C#:   await Task.WhenAll(t1, t2)
来源：http://jrq.quarkkingdee.top

[O06] 使用进程池
来源：http://vhv.jinghuilouyu.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://xsn.ppjwa.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://orf.yueranfly.top

JS:   // child_process / cluster 模块
来源：http://ifv.yvedp.cn

TS:   // child_process / cluster 模块
来源：http://ukr.zhoulong.xyz

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://fpj.nanxinkj.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://tzg.smart0.xyz

Ruby: // fork 块
来源：http://yjx.hcnkem.com

C#:   Parallel.For
来源：http://mtl.bbcook.cn

================================================================================
来源：http://qui.shzxlz.cn

P. 常用工具函数
来源：http://dyb.quarkkingdee.top

================================================================================
来源：http://qdl.jlsjyb.cn

[P01] 生成 UUID
来源：http://vdu.zycfv.cn

Py:   str(uuid.uuid4())
来源：http://qre.xuetiantiany.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://dsb.ivvv.top

JS:   crypto.randomUUID()
来源：http://xym.cheryme.top

TS:   crypto.randomUUID()
来源：http://tbu.ehwqpu.com

Java: UUID.randomUUID().toString()
来源：http://bhs.jqgufenzy.top

Go:   // 用 github.com/google/uuid
来源：http://ykl.nanxuanxn.top

Ruby: SecureRandom.uuid
来源：http://zds.iojbl.cn

C#:   Guid.NewGuid().ToString()
来源：http://zkh.chenjidiqi.icu

[P02] MD5 / SHA256 摘要
来源：http://cdf.dianchejie.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://khp.jiagoushi.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://iae.pycfn.com

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://xio.daria6918.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://vtw.smart0.xyz

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://bfa.cheryme.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://vmv.epnwcf.com

Ruby: Digest::SHA256.hexdigest(s)
来源：http://dhk.pengpengdd.cyou

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://dwh.tarul.cn

[P03] 生成短随机字符串
来源：http://wuj.bjfxy.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://lvm.dashuyun.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://bpq.uphjek.com

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://kkl.haohaochexian.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://izn.vehdjk.com

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ygs.yuanzhike.top


<!-- 参考信息 -->