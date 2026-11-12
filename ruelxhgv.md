代发 wailian999

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://cua.chenjidiqi.icu

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://oqi.ybcxt.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://tgz.nanxuanxn.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ctz.pengpengdd.cyou

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://fft.pengpengdd.cyou

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://bdk.jlsjyb.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://itj.daria6918.cn

[L06] 解析响应为 JSON
来源：http://oem.xuanzx.com

Py:   resp.json()
来源：http://wub.wangdashe.top

PHP:  json_decode($body, true);
来源：http://xew.yj20258.top

JS:   await resp.json()
来源：http://law.haohaochexian.top

TS:   await resp.json()
来源：http://rfa.ehwqpu.com

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://iyb.kuanghao11.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://tvb.cucudq.cn

Ruby: JSON.parse(resp.body)
来源：http://lve.fktsv.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://cxu.zhoulong.xyz

[L07] 处理 HTTP 状态码
来源：http://xge.ywan-chungtsiang.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://psv.jiagoushi.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://owc.yuxming.cn

JS:   resp.ok;  resp.status
来源：http://pzz.yj202588.top

TS:   resp.ok;  resp.status
来源：http://cbf.ydjk.org.cn

Java: resp.statusCode()
来源：http://qeq.pycfn.com

Go:   resp.StatusCode
来源：http://kgx.shzxlz.cn

Ruby: resp.code.to_i
来源：http://hex.havefunace.top

C#:   (int)resp.StatusCode
来源：http://wtj.hfpthk.cn

[L08] 并发请求多个地址
来源：http://bto.cqqwz.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ckj.tian-w.cn

PHP:  curl_multi_init() 系列
来源：http://pjy.zhengqikj.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ghx.pengpengdd.cyou

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ysd.jqgfzy.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://dxb.aizwys.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://caa.yueranfly.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ycn.xuetiantiany.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://nou.xylfe.cn

================================================================================
来源：http://upb.hcnkem.com

M. 命令行 / 进程 / 环境
来源：http://pmw.sjlbkw.cn

================================================================================
来源：http://gpc.sjlbkw.cn

[M01] 读取命令行参数
来源：http://msx.52xcode.cn

Py:   sys.argv[1:]
来源：http://rbe.yuanzhike.top

PHP:  $argv;  $argc;
来源：http://bpo.hongshengwenyu.top

JS:   process.argv.slice(2)
来源：http://yil.yfazqb.com

TS:   process.argv.slice(2)
来源：http://uas.redwolf501.top

Java: args 数组（main 方法参数）
来源：http://ahh.52xcode.cn

Go:   os.Args[1:]
来源：http://lgw.yueranfly.top

Ruby: ARGV
来源：http://fhv.zdbjq.cn

C#:   args 数组（Main 方法参数）
来源：http://mcc.svipenyu.cn

[M02] 读取环境变量
来源：http://elc.jyoumei.cn

Py:   os.environ.get("HOME")
来源：http://alq.jqgfzy.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://qbv.hesvh.cn

JS:   process.env.HOME
来源：http://rzn.jinqigufen.top

TS:   process.env.HOME
来源：http://kaj.yuxming.cn

Java: System.getenv("HOME")
来源：http://eum.zhixingplan.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://cjb.birdmap.top

Ruby: ENV["HOME"]
来源：http://xpk.yfazqb.com

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mpw.shzxlz.cn

[M03] 执行外部命令
来源：http://jxd.zycfv.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://zhm.wangdashe.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://jhy.ywan-chungtsiang.top

JS:   child_process.execSync("ls -l").toString()
来源：http://xup.fktsv.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://phv.tarul.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://weh.shzxlz.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://ofx.jqgufenzy.top

Ruby: system("ls -l");  `ls -l`
来源：http://oag.chenjidiqi.icu

C#:   Process.Start("ls", "-l");
来源：http://xfc.zhaomingkeji.xyz

[M04] 获取当前工作目录
来源：http://uhj.xziqi.cn

Py:   os.getcwd()
来源：http://ixv.shanyushiyangkeji.top

PHP:  getcwd();
来源：http://hpx.wangdashe.top

JS:   process.cwd()
来源：http://hkr.redwolf501.top

TS:   process.cwd()
来源：http://vgi.ydzc1.top

Java: Path.of("").toAbsolutePath()
来源：http://dvn.cucudq.cn

Go:   os.Getwd()
来源：http://lid.hfpthk.cn

Ruby: Dir.pwd
来源：http://ruc.gzhubu.top

C#:   Directory.GetCurrentDirectory()
来源：http://qlv.yonumen.top

[M05] 设置退出码
来源：http://xiw.nanxuanxn.top

Py:   sys.exit(1)
来源：http://zqh.yj202588.top

PHP:  exit(1);
来源：http://ybq.dianchejie.cn

JS:   process.exit(1)
来源：http://ete.zhongyouzk.top

TS:   process.exit(1)
来源：http://zkb.cucudq.cn

Java: System.exit(1)
来源：http://zmc.cashguo.top

Go:   os.Exit(1)
来源：http://lmi.jinghuilouyu.cn

Ruby: exit 1
来源：http://zrd.epnwcf.com

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://kab.wangshuangyany.cn

[M06] 向标准错误输出
来源：http://tpd.guannengcc.top

Py:   print("err", file=sys.stderr)
来源：http://gfs.andypj.xyz

PHP:  fwrite(STDERR, "err\n");
来源：http://qhb.redwolf501.top

JS:   console.error("err")
来源：http://dqx.shuidangran.top

TS:   console.error("err")
来源：http://rye.dashuyun.cn

Java: System.err.println("err")
来源：http://cba.havefunace.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wfv.gotoacloud.top

Ruby: warn "err"
来源：http://ugb.ybcxt.top

C#:   Console.Error.WriteLine("err")
来源：http://ukt.gogol.net.cn

[M07] 判断是否为主入口
来源：http://zpz.zhengqikj.top

Py:   if __name__ == "__main__":
来源：http://nud.cheryme.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://djr.yanxiufei.cn

JS:   require.main === module
来源：http://lfu.316326.xyz

TS:   require.main === module
来源：http://fcj.shanyushiyangtech.top

Java: public static void main(String[] args)
来源：http://vnn.ybcxt.top

Go:   func main()
来源：http://ujq.tian-w.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hge.tarul.cn

C#:   static void Main(string[] args)
来源：http://rbz.shanyushiyangtech.top

[M08] 获取系统与运行时信息
来源：http://miy.andypj.xyz

Py:   platform.system();  platform.python_version()
来源：http://hzd.jqgufenzy.top

PHP:  PHP_OS;  phpversion();
来源：http://tmy.fanxiaobao.xyz

JS:   process.platform;  process.version
来源：http://dbq.snrcjt.cn

TS:   process.platform;  process.version
来源：http://pkf.shanyushiyangkeji.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wue.tarul.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://axr.c1oappe.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://uel.hesvh.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://nyv.pycfn.com

================================================================================
来源：http://clp.shuidangran.top

N. 数据结构与算法
来源：http://zkp.dianchejie.cn

================================================================================
来源：http://ssy.quarkkingdee.top

[N01] 二分查找（有序数组）
来源：http://yns.chenjidiqi.icu

Py:   bisect.bisect_left(arr, x)
来源：http://mlj.mhx1999.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://yri.ehwqpu.com

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ghy.yongpay.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://tkj.yueranfly.top

Java: Arrays.binarySearch(arr, x)
来源：http://bdm.jianghu66.top

Go:   sort.SearchInts(arr, x)
来源：http://bys.gaohongyu789.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://mtt.wangdashe.top

C#:   Array.BinarySearch(arr, x)
来源：http://sff.jinyuanbaomall.cn

[N02] 排序（工程实践用内置实现）
来源：http://amd.zhijiandao.cn

Py:   sorted(arr);  arr.sort()
来源：http://ylf.snrcjt.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://jsa.wangshuangyany.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://rqs.quarkkingdee.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://mmc.jqgufenzy.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://own.yuanzhike.top

Go:   slices.Sort(arr)
来源：http://xpm.havefunace.top

Ruby: arr.sort
来源：http://ujf.zhixingplan.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://fow.ivvv.top

[N03] 快速排序（分治示例）
来源：http://vib.xinyue.icu

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://bgb.chenjidiqi.icu

PHP:  // 递归实现，或用 usort
来源：http://qxr.bjfxy.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://exd.tian-w.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://rqx.ppjwa.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ssr.cheryme.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://zwh.hnqzz.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://xbm.fzhhl.top

C#:   // 手写递归，或 Array.Sort
来源：http://ios.sxryk.cn

[N04] 斐波那契数列
来源：http://gan.yanxiufei.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ula.tianlin.xyz

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://dvj.chenlongwang.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://lmt.yj20258888.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ejs.yuanzhike.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://nvk.nanxinkj.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://zkj.cdnleiting.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://yvo.fengsongda.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://jhx.9152youxi.cn

[N05] 最大公约数
来源：http://slw.redwolf501.top

Py:   math.gcd(a, b)
来源：http://pwe.jqgufenzy.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://uyr.cashguo.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://cui.ivvv.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://vnc.ybcxt.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ivy.fanxiaobao.xyz

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://atu.zhoulong.xyz

Ruby: a.gcd(b)
来源：http://nul.daria6918.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wuk.daxiang520.top

[N06] 判断回文字符串
来源：http://iib.zdqjudy.top

Py:   s == s[::-1]
来源：http://zgy.cashguo.top

PHP:  $s === strrev($s);
来源：http://uhm.aibaodan.cn

JS:   s === [...s].reverse().join("")
来源：http://iyw.jyoumei.cn

TS:   s === [...s].reverse().join("")
来源：http://auv.zhiwuduotai.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ifq.yvedp.cn

Go:   // 双指针从两端比较
来源：http://vbf.316326.xyz

Ruby: s == s.reverse
来源：http://cuj.nanxinkj.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://wju.mhx1999.top

[N07] 两数之和（返回下标）
来源：http://sdl.fktsv.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ydg.yj20258.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://jic.yanxiufei.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://gcy.jyoumei.cn

TS:   // 手写 Map<string, number>
来源：http://uys.pycfn.com

Java: // 手写 HashMap
来源：http://tvj.kuanghao11.cn

Go:   // 手写 map[int]int
来源：http://trs.dashuyun.cn

Ruby: // 手写 Hash
来源：http://zng.yuxming.cn

C#:   // 手写 Dictionary<int, int>
来源：http://fym.fengsongda.top

[N08] 生成全排列
来源：http://jib.vqdsnc.cn

Py:   itertools.permutations(arr)
来源：http://cxn.zhongyouzk.top

PHP:  // 手写递归交换
来源：http://kmb.gzhubu.top

JS:   // 手写回溯递归
来源：http://gxy.52xcode.cn

TS:   // 手写回溯递归
来源：http://shq.daria6918.cn

Java: // 手写回溯递归
来源：http://hqc.yuxming.cn

Go:   // 手写回溯递归
来源：http://ebo.zhijiandao.cn

Ruby: arr.permutation.to_a
来源：http://mjc.snrcjt.cn

C#:   // 手写回溯递归
来源：http://wfv.sxryk.cn

[N09] 栈与队列
来源：http://sse.aibaodan.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://zon.ppjwa.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ckx.shangyingyoupin.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://pbr.cdnleiting.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://qes.jqgufenzy.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://igh.xinyue.icu

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://goh.shangyingyoupin.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://iim.yueranfly.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://aru.xuanzx.com

[N10] 链表节点定义
来源：http://nxq.epnwcf.com

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://drb.ctjpmb.com

PHP:  class Node { public $v; public $next = null; }
来源：http://yck.quarkkingdee.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ooq.yuxming.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ebr.shuidangran.top

Java: class Node { int v; Node next; }
来源：http://frp.tian-w.cn

Go:   type Node struct { V int; Next *Node }
来源：http://zpa.bbcook.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://eoo.zhengqikj.top

C#:   class Node { public int V; public Node? Next; }
来源：http://eze.yueranfly.top

[N11] 二叉树中序遍历
来源：http://wgv.pycfn.com

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wpr.cheryme.top

PHP:  // 手写递归函数
来源：http://xrk.cqqwz.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ten.pengpengdd.cyou

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://dnc.yuanzhike.top

Java: // 手写递归
来源：http://bhx.yuxming.cn

Go:   // 手写递归
来源：http://epf.cdnleiting.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://fuq.gotoacloud.top

C#:   // 手写递归
来源：http://uth.bbcook.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://nqv.shangyingyoupin.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ebb.tanke756.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://nke.wangdashe.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://nmr.chenjidiqi.icu

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://kus.wangshuangyany.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://pdn.9152youxi.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://djv.yj20258.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://htv.ybcxt.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://vxa.aizwys.cn

================================================================================
来源：http://dqk.dianchejie.cn

O. 并发与异步
来源：http://jmj.uphjek.com

================================================================================
来源：http://nxa.uphjek.com

[O01] 启动一个线程
来源：http://elc.jinqigufen.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://eyb.yfazqb.com

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://qjw.yvedp.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://jug.guowangkeji.top

TS:   // 同 JS
来源：http://sie.vehdjk.com

Java: new Thread(() -> f()).start()
来源：http://wxr.epnwcf.com

Go:   go f()
来源：http://tuv.zdqjudy.top

Ruby: Thread.new { f }
来源：http://jig.zhengqikj.top

C#:   Task.Run(() => F());
来源：http://vwr.shanyushiyangkeji.top

[O02] 使用线程池
来源：http://ueo.cdnleiting.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ypz.yuanzhike.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://nnv.yongpay.top

JS:   // worker_threads 线程池
来源：http://lyw.daxiang520.top

TS:   // worker_threads 线程池
来源：http://mwg.daxiang520.top

Java: Executors.newFixedThreadPool(4)
来源：http://jfu.bjfxy.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://xcf.jqgfzy.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ass.nwbrower.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hya.jianghu66.top

[O03] 加锁保护共享数据
来源：http://lhn.shzxlz.cn

Py:   with lock: shared += 1
来源：http://aye.daria6918.cn

PHP:  // 用 flock() 做文件锁
来源：http://twp.pycfn.com

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://rkl.cucudq.cn

TS:   // 同 JS
来源：http://vro.tarul.cn

Java: synchronized (this) { shared++; }
来源：http://ezg.yj20258.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://sos.cqqwz.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://smg.jyoumei.cn

C#:   lock (gate) { shared++; }
来源：http://gxv.vehdjk.com

[O04] 定义异步函数并等待
来源：http://mur.wangshuangyany.cn

Py:   async def f():⏎    await g()
来源：http://crt.cheryme.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://iiy.zhaomingkeji.xyz

JS:   async function f() { await g(); }
来源：http://hxk.yfazqb.com

TS:   async function f(): Promise<void> { await g(); }
来源：http://ucz.jiagoushi.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://oad.jinqigfzy.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://rue.hongshengwenyu.top

Ruby: # 用 Fiber 或 async gem
来源：http://ier.bjfxy.top

C#:   async Task F() { await G(); }
来源：http://fbl.mhx1999.top

[O05] 并发执行并等待全部完成
来源：http://kzv.dashuyun.cn

Py:   asyncio.gather(*tasks)
来源：http://zos.shanyushiyangkeji.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ajs.shzxlz.cn

JS:   await Promise.all(tasks)
来源：http://tiu.ybcxt.top

TS:   await Promise.all(tasks)
来源：http://sio.jlsjyb.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://fcf.fktsv.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://dbi.jianghu66.top

Ruby: threads.map(&:join)
来源：http://kcu.cdnleiting.top

C#:   await Task.WhenAll(t1, t2)
来源：http://ajj.hcnkem.com

[O06] 使用进程池
来源：http://lwq.jinghuilouyu.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://qju.hesvh.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://hcg.c1oappe.top

JS:   // child_process / cluster 模块
来源：http://jmu.bbcook.cn

TS:   // child_process / cluster 模块
来源：http://rtu.hnxiangtu.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://xlc.redwolf501.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://njs.yj20258.top

Ruby: // fork 块
来源：http://ruu.cheryme.top

C#:   Parallel.For
来源：http://rod.mhx1999.top

================================================================================
来源：http://szr.yuxming.cn

P. 常用工具函数
来源：http://jzl.shuidangran.top

================================================================================
来源：http://gsa.shangyingyoupin.top

[P01] 生成 UUID
来源：http://afr.svipenyu.cn

Py:   str(uuid.uuid4())
来源：http://ihh.nwbrower.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://jjq.pycfn.com

JS:   crypto.randomUUID()
来源：http://lek.tian-w.cn

TS:   crypto.randomUUID()
来源：http://oqk.9152youxi.cn

Java: UUID.randomUUID().toString()
来源：http://izi.daria6918.cn

Go:   // 用 github.com/google/uuid
来源：http://lmz.tarul.cn

Ruby: SecureRandom.uuid
来源：http://jox.zycfv.cn

C#:   Guid.NewGuid().ToString()
来源：http://bqb.shuidangran.top

[P02] MD5 / SHA256 摘要
来源：http://jgu.c1oappe.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mfo.yuxming.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://uue.cdnleiting.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://gfh.fehbvm.com

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mcu.hnqzz.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://fsa.gogol.net.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://vbe.chenlongwang.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://slq.guannengcc.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wae.xuetiantiany.cn

[P03] 生成短随机字符串
来源：http://ylc.cucudq.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://lcl.andypj.xyz


<!-- 参考信息 -->