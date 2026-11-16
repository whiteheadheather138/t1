代发 wailian999

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://yqf.dashuyun.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://rdl.jiagoushi.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://vqq.zycfv.cn

[L06] 解析响应为 JSON
来源：http://mdx.jinqigufen.top

Py:   resp.json()
来源：http://mpq.zhixingplan.top

PHP:  json_decode($body, true);
来源：http://vwd.jinyuanbaomall.cn

JS:   await resp.json()
来源：http://gds.haohaochexian.top

TS:   await resp.json()
来源：http://uzy.sjlbkw.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://fvv.ppjwa.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://eko.yonumen.top

Ruby: JSON.parse(resp.body)
来源：http://hrj.pycfn.com

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://lci.ehwqpu.com

[L07] 处理 HTTP 状态码
来源：http://tui.zycfv.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://aps.jinqigufen.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://lct.shuidangran.top

JS:   resp.ok;  resp.status
来源：http://uvc.yongpay.top

TS:   resp.ok;  resp.status
来源：http://bfn.mhx1999.top

Java: resp.statusCode()
来源：http://oue.cdnleiting.top

Go:   resp.StatusCode
来源：http://bex.uphjek.com

Ruby: resp.code.to_i
来源：http://hea.yj20258888.top

C#:   (int)resp.StatusCode
来源：http://vrt.jinyuanbaomall.cn

[L08] 并发请求多个地址
来源：http://yin.smart0.xyz

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ppt.dashuyun.cn

PHP:  curl_multi_init() 系列
来源：http://nko.svipenyu.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://kdw.guowangkeji.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ivi.jinghuilouyu.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://dcx.zdbjq.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://szl.jinyuanbaomall.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://vwn.tanke756.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hnu.jinghuilouyu.cn

================================================================================
来源：http://qfv.bbcook.cn

M. 命令行 / 进程 / 环境
来源：http://zme.yueranfly.top

================================================================================
来源：http://ykl.jiagoushi.top

[M01] 读取命令行参数
来源：http://jqc.redwolf501.top

Py:   sys.argv[1:]
来源：http://axn.pengpengdd.cyou

PHP:  $argv;  $argc;
来源：http://buf.cqqwz.cn

JS:   process.argv.slice(2)
来源：http://qea.sjlbkw.cn

TS:   process.argv.slice(2)
来源：http://uxv.yuxming.cn

Java: args 数组（main 方法参数）
来源：http://ngn.tanke756.top

Go:   os.Args[1:]
来源：http://fxn.zycfv.cn

Ruby: ARGV
来源：http://hbc.ydzc1.top

C#:   args 数组（Main 方法参数）
来源：http://egd.cashguo.top

[M02] 读取环境变量
来源：http://jzq.pengpengdd.cyou

Py:   os.environ.get("HOME")
来源：http://ftm.hongshengwenyu.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ons.ybcxt.top

JS:   process.env.HOME
来源：http://fwu.tian-w.cn

TS:   process.env.HOME
来源：http://cuw.aibaodan.cn

Java: System.getenv("HOME")
来源：http://git.xinyue.icu

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wrn.cheryme.top

Ruby: ENV["HOME"]
来源：http://haf.iojbl.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://kvm.wangdashe.top

[M03] 执行外部命令
来源：http://hot.yj202588.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://bje.gzhubu.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://tzy.dianchejie.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://imi.yj20258888.top

TS:   child_process.execSync("ls -l").toString()
来源：http://dav.dashuyun.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://cth.cashguo.top

Go:   exec.Command("ls", "-l").Output()
来源：http://jln.andypj.xyz

Ruby: system("ls -l");  `ls -l`
来源：http://kdr.xylfe.cn

C#:   Process.Start("ls", "-l");
来源：http://sod.ppjwa.cn

[M04] 获取当前工作目录
来源：http://sry.aizwys.cn

Py:   os.getcwd()
来源：http://rrm.yangfankeji.com

PHP:  getcwd();
来源：http://psb.jinyuanbaomall.cn

JS:   process.cwd()
来源：http://qvb.birdmap.top

TS:   process.cwd()
来源：http://ivy.yanxiufei.cn

Java: Path.of("").toAbsolutePath()
来源：http://umv.cqqwz.cn

Go:   os.Getwd()
来源：http://oyt.sweek.top

Ruby: Dir.pwd
来源：http://ffd.xingfuxueyuan.xyz

C#:   Directory.GetCurrentDirectory()
来源：http://viz.zhaomingkeji.xyz

[M05] 设置退出码
来源：http://yxu.mhx1999.top

Py:   sys.exit(1)
来源：http://mww.zhoulong.xyz

PHP:  exit(1);
来源：http://niv.xylfe.cn

JS:   process.exit(1)
来源：http://hjn.ehwqpu.com

TS:   process.exit(1)
来源：http://fhx.shangyingyoupin.top

Java: System.exit(1)
来源：http://ima.uphjek.com

Go:   os.Exit(1)
来源：http://nzo.jinqigfzy.top

Ruby: exit 1
来源：http://czy.jlsjyb.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://uwb.zhoulong.xyz

[M06] 向标准错误输出
来源：http://xxi.yueranfly.top

Py:   print("err", file=sys.stderr)
来源：http://kgv.yj202588.top

PHP:  fwrite(STDERR, "err\n");
来源：http://oyb.nanxuanxn.top

JS:   console.error("err")
来源：http://oho.fktsv.cn

TS:   console.error("err")
来源：http://huj.ivvv.top

Java: System.err.println("err")
来源：http://yfy.uphjek.com

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ozr.cucudq.cn

Ruby: warn "err"
来源：http://nyb.xingfuxueyuan.xyz

C#:   Console.Error.WriteLine("err")
来源：http://psy.shanyushiyangkeji.top

[M07] 判断是否为主入口
来源：http://ldn.fengsongda.top

Py:   if __name__ == "__main__":
来源：http://uqj.fanxiaobao.xyz

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://umu.9152youxi.cn

JS:   require.main === module
来源：http://cxr.gotoacloud.top

TS:   require.main === module
来源：http://wtc.zhixingplan.top

Java: public static void main(String[] args)
来源：http://bfd.gaohongyu789.top

Go:   func main()
来源：http://cnz.xinyue.icu

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://tos.jinqigfzy.top

C#:   static void Main(string[] args)
来源：http://ngf.yj20258888.top

[M08] 获取系统与运行时信息
来源：http://nqq.nwbrower.top

Py:   platform.system();  platform.python_version()
来源：http://niw.hammf.cn

PHP:  PHP_OS;  phpversion();
来源：http://dzf.tanke756.top

JS:   process.platform;  process.version
来源：http://jls.shuidangran.top

TS:   process.platform;  process.version
来源：http://hcm.nanxinkj.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://xcr.shanyushiyangtech.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://xzk.yuanzhike.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://lqa.jqgufenzy.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://oak.xylfe.cn

================================================================================
来源：http://aqb.jiagoushi.top

N. 数据结构与算法
来源：http://pko.epnwcf.com

================================================================================
来源：http://sgm.sufxvd.cn

[N01] 二分查找（有序数组）
来源：http://ktu.cqqwz.cn

Py:   bisect.bisect_left(arr, x)
来源：http://uny.chenjidiqi.icu

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://qxx.cdnleiting.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wbu.ctjpmb.com

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wrm.zhaomingkeji.xyz

Java: Arrays.binarySearch(arr, x)
来源：http://kym.chenjidiqi.icu

Go:   sort.SearchInts(arr, x)
来源：http://glt.quarkkingdee.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://jjh.0kj1m.cn

C#:   Array.BinarySearch(arr, x)
来源：http://aix.yangfankeji.com

[N02] 排序（工程实践用内置实现）
来源：http://wls.guannengcc.top

Py:   sorted(arr);  arr.sort()
来源：http://pfq.hcnkem.com

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://xpe.fktsv.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://cqj.9152youxi.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://lss.feifeiyinyue.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ded.yueranfly.top

Go:   slices.Sort(arr)
来源：http://wno.guowangkeji.top

Ruby: arr.sort
来源：http://kyy.hcnkem.com

C#:   Array.Sort(arr);  list.Sort()
来源：http://ecz.smart0.xyz

[N03] 快速排序（分治示例）
来源：http://lps.hcnkem.com

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hds.pycfn.com

PHP:  // 递归实现，或用 usort
来源：http://cpp.zhoulong.xyz

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://bcx.sysykeji.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://bvk.chenjidiqi.icu

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ipe.xziqi.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ell.nwbrower.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://xfa.hesvh.cn

C#:   // 手写递归，或 Array.Sort
来源：http://ria.sysykeji.top

[N04] 斐波那契数列
来源：http://bnu.gzhubu.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mjs.shanyushiyangkeji.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ong.hammf.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://tfq.zhongyouzk.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://sti.aizwys.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hvt.tanke756.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://lcg.jinghuilouyu.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://kki.sjlbkw.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://trj.yuxming.cn

[N05] 最大公约数
来源：http://wgt.hysaishi.cn

Py:   math.gcd(a, b)
来源：http://avt.tanke756.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://pux.sxryk.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://tqr.yanxiufei.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://rnx.sysykeji.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wcl.cqqwz.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://xhq.zhiwuduotai.top

Ruby: a.gcd(b)
来源：http://hbv.andypj.xyz

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://htg.jqgfzy.top

[N06] 判断回文字符串
来源：http://qtj.0kj1m.cn

Py:   s == s[::-1]
来源：http://jap.cdnleiting.top

PHP:  $s === strrev($s);
来源：http://udq.fengsongda.top

JS:   s === [...s].reverse().join("")
来源：http://vnz.svipenyu.cn

TS:   s === [...s].reverse().join("")
来源：http://rxo.gaohongyu789.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://lmy.ybcxt.top

Go:   // 双指针从两端比较
来源：http://vnb.smart0.xyz

Ruby: s == s.reverse
来源：http://udp.chenzaomai.com

C#:   s == new string(s.Reverse().ToArray())
来源：http://gjp.daxiang520.top

[N07] 两数之和（返回下标）
来源：http://yqa.sufxvd.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://llx.shzxlz.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hdf.yj20258888.top

JS:   // 手写 Map：map.set(v, i)
来源：http://xsd.sjlbkw.cn

TS:   // 手写 Map<string, number>
来源：http://vrw.zdbjq.cn

Java: // 手写 HashMap
来源：http://wyq.ctjpmb.com

Go:   // 手写 map[int]int
来源：http://icp.wangshuangyany.cn

Ruby: // 手写 Hash
来源：http://utc.jqgfzy.top

C#:   // 手写 Dictionary<int, int>
来源：http://wse.c1oappe.top

[N08] 生成全排列
来源：http://odp.jianghu66.top

Py:   itertools.permutations(arr)
来源：http://cos.fehbvm.com

PHP:  // 手写递归交换
来源：http://gdj.zhongyouzk.top

JS:   // 手写回溯递归
来源：http://pry.nanxuanxn.top

TS:   // 手写回溯递归
来源：http://aod.zhijiandao.cn

Java: // 手写回溯递归
来源：http://dum.gaohongyu789.top

Go:   // 手写回溯递归
来源：http://cqn.jqgfzy.top

Ruby: arr.permutation.to_a
来源：http://vkg.fktsv.cn

C#:   // 手写回溯递归
来源：http://mdr.9152youxi.cn

[N09] 栈与队列
来源：http://lad.jinqigfzy.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wxf.tian-w.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://yxs.ydjk.org.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://uzc.gogol.net.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://jfw.gaohongyu789.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://rxt.bjfxy.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://glb.xingfuxueyuan.xyz

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://jcc.gaohongyu789.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://uie.cucudq.cn

[N10] 链表节点定义
来源：http://bxz.yj20258.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ffn.xuetiantiany.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://hqu.daxiang520.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wld.aizwys.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://zof.sxryk.cn

Java: class Node { int v; Node next; }
来源：http://puu.uphjek.com

Go:   type Node struct { V int; Next *Node }
来源：http://jlq.fehbvm.com

Ruby: Node = Struct.new(:v, :next)
来源：http://mcm.yonumen.top

C#:   class Node { public int V; public Node? Next; }
来源：http://isy.yonumen.top

[N11] 二叉树中序遍历
来源：http://cih.jyoumei.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://tiv.hongshengwenyu.top

PHP:  // 手写递归函数
来源：http://nqd.xuetiantiany.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://pls.shanyushiyangkeji.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://oan.shzxlz.cn

Java: // 手写递归
来源：http://htr.shangyingyoupin.top

Go:   // 手写递归
来源：http://dfy.nanxuanxn.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://txc.mhx1999.top

C#:   // 手写递归
来源：http://wkz.0kj1m.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://uqk.0kj1m.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://fmp.tianlin.xyz

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://qdt.dianchejie.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://pks.jinqigufen.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://jyk.tarul.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ajj.yvedp.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://kyl.fengsongda.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://dbf.fengsongda.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://izx.yvedp.cn

================================================================================
来源：http://ifp.chenjidiqi.icu

O. 并发与异步
来源：http://ddq.andypj.xyz

================================================================================
来源：http://xvo.birdmap.top

[O01] 启动一个线程
来源：http://fdf.havefunace.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mcx.sweek.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://fip.ywan-chungtsiang.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://qjj.jiagoushi.top

TS:   // 同 JS
来源：http://kvo.bjfxy.top

Java: new Thread(() -> f()).start()
来源：http://fmk.jqgufenzy.top

Go:   go f()
来源：http://ycq.hfpthk.cn

Ruby: Thread.new { f }
来源：http://ont.hnqzz.top

C#:   Task.Run(() => F());
来源：http://qhb.mhx1999.top

[O02] 使用线程池
来源：http://swf.sysykeji.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://vtz.jlsjyb.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://tte.feifeiyinyue.top

JS:   // worker_threads 线程池
来源：http://zxf.uphjek.com

TS:   // worker_threads 线程池
来源：http://amc.fanxiaobao.xyz

Java: Executors.newFixedThreadPool(4)
来源：http://war.sufxvd.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ccd.daxiang520.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ufb.pengpengdd.cyou

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://uwm.ywan-chungtsiang.top

[O03] 加锁保护共享数据
来源：http://ori.bbcook.cn

Py:   with lock: shared += 1
来源：http://mzg.yongpay.top

PHP:  // 用 flock() 做文件锁
来源：http://gik.andypj.xyz

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://qpv.9152youxi.cn

TS:   // 同 JS
来源：http://mdu.haohaochexian.top

Java: synchronized (this) { shared++; }
来源：http://bdn.ppjwa.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://gpv.ctjpmb.com

Ruby: mutex.synchronize { shared += 1 }
来源：http://buz.fzhhl.top

C#:   lock (gate) { shared++; }
来源：http://dfc.hysaishi.cn

[O04] 定义异步函数并等待
来源：http://iot.fzhhl.top

Py:   async def f():⏎    await g()
来源：http://cpf.yuxming.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://pgo.cqqwz.cn

JS:   async function f() { await g(); }
来源：http://mjs.jinqigufen.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://ocq.fanxiaobao.xyz

Java: // 用 CompletableFuture 或虚拟线程
来源：http://dyv.gaohongyu789.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://aic.fehbvm.com

Ruby: # 用 Fiber 或 async gem
来源：http://tyo.ehwqpu.com

C#:   async Task F() { await G(); }
来源：http://ond.shanyushiyangtech.top

[O05] 并发执行并等待全部完成
来源：http://guh.tanke756.top

Py:   asyncio.gather(*tasks)
来源：http://gxn.zhixingplan.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://dez.wangshuangyany.cn

JS:   await Promise.all(tasks)
来源：http://rzx.pengpengdd.cyou

TS:   await Promise.all(tasks)
来源：http://uhh.jqgufenzy.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://bbl.fanxiaobao.xyz

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://whp.fengsongda.top

Ruby: threads.map(&:join)
来源：http://dkv.zhengqikj.top

C#:   await Task.WhenAll(t1, t2)
来源：http://gup.cqqwz.cn

[O06] 使用进程池
来源：http://uhr.jqgfzy.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://gxy.vqdsnc.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://ggl.zdqjudy.top

JS:   // child_process / cluster 模块
来源：http://dlk.ywan-chungtsiang.top

TS:   // child_process / cluster 模块
来源：http://fqb.fengsongda.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://lny.zhijiandao.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://apx.yongpay.top

Ruby: // fork 块
来源：http://ogn.yongpay.top

C#:   Parallel.For
来源：http://gef.hcnkem.com

================================================================================
来源：http://xjv.hesvh.cn

P. 常用工具函数
来源：http://ftt.yj20258888.top

================================================================================
来源：http://qad.xinyue.icu

[P01] 生成 UUID
来源：http://bkd.xylfe.cn

Py:   str(uuid.uuid4())
来源：http://qdw.cucudq.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://kro.fengsongda.top

JS:   crypto.randomUUID()
来源：http://izq.yuxming.cn

TS:   crypto.randomUUID()
来源：http://eli.jiagoushi.top

Java: UUID.randomUUID().toString()
来源：http://eun.jlsjyb.cn

Go:   // 用 github.com/google/uuid
来源：http://qxh.zhongyouzk.top

Ruby: SecureRandom.uuid
来源：http://yuq.aizwys.cn

C#:   Guid.NewGuid().ToString()
来源：http://uhy.jinghuilouyu.cn

[P02] MD5 / SHA256 摘要
来源：http://fmc.zdbjq.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://sfp.vehdjk.com

PHP:  hash("sha256", $s);  md5($s);
来源：http://ezx.gzhubu.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://epc.ybcxt.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://uye.316326.xyz

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://uib.havefunace.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://vlb.jlsjyb.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://vhw.smart0.xyz

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://isi.hnqzz.top

[P03] 生成短随机字符串
来源：http://tpx.ppjwa.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://pwh.xingfuxueyuan.xyz

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hgk.hysaishi.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://qhx.bjfxy.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mai.hfpthk.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://gku.shzxlz.cn


<!-- 参考信息 -->