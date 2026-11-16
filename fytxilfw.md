代发 wailian999

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hln.nanxuanxn.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://xon.tianlin.xyz

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://gfs.hnxiangtu.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://vrn.jiagoushi.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ckj.andypj.xyz

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ngl.shanyushiyangtech.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mzk.jinqigufen.top

[L06] 解析响应为 JSON
来源：http://wqt.zhijiandao.cn

Py:   resp.json()
来源：http://rnn.hongshengwenyu.top

PHP:  json_decode($body, true);
来源：http://hot.shanyushiyangtech.top

JS:   await resp.json()
来源：http://iyr.shangyingyoupin.top

TS:   await resp.json()
来源：http://uwr.vqdsnc.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://vfn.ydjk.org.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://unn.xziqi.cn

Ruby: JSON.parse(resp.body)
来源：http://kqf.havefunace.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://syp.bbcook.cn

[L07] 处理 HTTP 状态码
来源：http://lgv.andypj.xyz

Py:   resp.status_code;  resp.raise_for_status()
来源：http://vor.hnqzz.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://gyw.haohaochexian.top

JS:   resp.ok;  resp.status
来源：http://vqi.xingfuxueyuan.xyz

TS:   resp.ok;  resp.status
来源：http://uya.pengpengdd.cyou

Java: resp.statusCode()
来源：http://ulz.sjlbkw.cn

Go:   resp.StatusCode
来源：http://bzv.wangshuangyany.cn

Ruby: resp.code.to_i
来源：http://fkh.mhx1999.top

C#:   (int)resp.StatusCode
来源：http://agy.mhx1999.top

[L08] 并发请求多个地址
来源：http://mio.nanxinkj.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://jus.zhoulong.xyz

PHP:  curl_multi_init() 系列
来源：http://bbe.316326.xyz

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://xvf.gotoacloud.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ify.aibaodan.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://sdf.pycfn.com

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://gfi.shuidangran.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://cgn.ppjwa.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://xef.gotoacloud.top

================================================================================
来源：http://ely.mhx1999.top

M. 命令行 / 进程 / 环境
来源：http://kzu.yuxming.cn

================================================================================
来源：http://dik.andypj.xyz

[M01] 读取命令行参数
来源：http://ewd.hysaishi.cn

Py:   sys.argv[1:]
来源：http://ikm.jqgufenzy.top

PHP:  $argv;  $argc;
来源：http://jrn.cashguo.top

JS:   process.argv.slice(2)
来源：http://lty.hywenlv.cn

TS:   process.argv.slice(2)
来源：http://vgq.dashuyun.cn

Java: args 数组（main 方法参数）
来源：http://mvr.birdmap.top

Go:   os.Args[1:]
来源：http://vba.mhx1999.top

Ruby: ARGV
来源：http://zqb.havefunace.top

C#:   args 数组（Main 方法参数）
来源：http://zor.vehdjk.com

[M02] 读取环境变量
来源：http://hjp.ctjpmb.com

Py:   os.environ.get("HOME")
来源：http://dcf.dashuyun.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ube.haohaochexian.top

JS:   process.env.HOME
来源：http://mil.cashguo.top

TS:   process.env.HOME
来源：http://ahz.daria6918.cn

Java: System.getenv("HOME")
来源：http://vgg.yanxiufei.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://esu.jlsjyb.cn

Ruby: ENV["HOME"]
来源：http://sso.yonumen.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ira.yj20258888.top

[M03] 执行外部命令
来源：http://xer.xingfuxueyuan.xyz

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://vtx.0kj1m.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://dvc.sweek.top

JS:   child_process.execSync("ls -l").toString()
来源：http://pjy.bjfxy.top

TS:   child_process.execSync("ls -l").toString()
来源：http://igl.guannengcc.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ogd.yvedp.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://sbd.jqgfzy.top

Ruby: system("ls -l");  `ls -l`
来源：http://kvw.hcnkem.com

C#:   Process.Start("ls", "-l");
来源：http://lvs.bjfxy.top

[M04] 获取当前工作目录
来源：http://jwp.jinghuilouyu.cn

Py:   os.getcwd()
来源：http://yfh.pengpengdd.cyou

PHP:  getcwd();
来源：http://smm.jinqigfzy.top

JS:   process.cwd()
来源：http://yhj.shanyushiyangtech.top

TS:   process.cwd()
来源：http://ykr.yj20258888.top

Java: Path.of("").toAbsolutePath()
来源：http://wlt.gaohongyu789.top

Go:   os.Getwd()
来源：http://ugx.epnwcf.com

Ruby: Dir.pwd
来源：http://tnp.quarkkingdee.top

C#:   Directory.GetCurrentDirectory()
来源：http://xqo.yj202588.top

[M05] 设置退出码
来源：http://run.nanxuanxn.top

Py:   sys.exit(1)
来源：http://cnm.smart0.xyz

PHP:  exit(1);
来源：http://bjd.jinqigufen.top

JS:   process.exit(1)
来源：http://fvw.dashuyun.cn

TS:   process.exit(1)
来源：http://zkk.ywan-chungtsiang.top

Java: System.exit(1)
来源：http://ews.bbcook.cn

Go:   os.Exit(1)
来源：http://thz.kuanghao11.cn

Ruby: exit 1
来源：http://oek.dianchejie.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wnn.jiagoushi.top

[M06] 向标准错误输出
来源：http://apt.jianghu66.top

Py:   print("err", file=sys.stderr)
来源：http://tnj.hfpthk.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://ixl.ehwqpu.com

JS:   console.error("err")
来源：http://qso.ydzc1.top

TS:   console.error("err")
来源：http://xyj.dianchejie.cn

Java: System.err.println("err")
来源：http://zip.iojbl.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://rea.zycfv.cn

Ruby: warn "err"
来源：http://clz.yongpay.top

C#:   Console.Error.WriteLine("err")
来源：http://bup.zycfv.cn

[M07] 判断是否为主入口
来源：http://ttx.guowangkeji.top

Py:   if __name__ == "__main__":
来源：http://vxd.birdmap.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://jmv.hammf.cn

JS:   require.main === module
来源：http://qnf.guannengcc.top

TS:   require.main === module
来源：http://chq.haohaochexian.top

Java: public static void main(String[] args)
来源：http://bqw.chenlongwang.top

Go:   func main()
来源：http://uyk.shuidangran.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hxn.hnqzz.top

C#:   static void Main(string[] args)
来源：http://heu.shanyushiyangkeji.top

[M08] 获取系统与运行时信息
来源：http://bii.zhixingplan.top

Py:   platform.system();  platform.python_version()
来源：http://mfm.vehdjk.com

PHP:  PHP_OS;  phpversion();
来源：http://ggm.daxiang520.top

JS:   process.platform;  process.version
来源：http://kka.yueranfly.top

TS:   process.platform;  process.version
来源：http://umu.hcnkem.com

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://asb.gaohongyu789.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://dae.xinyue.icu

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wxa.hysaishi.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://yyq.yvedp.cn

================================================================================
来源：http://rfr.ppjwa.cn

N. 数据结构与算法
来源：http://jdr.bbcook.cn

================================================================================
来源：http://czz.c1oappe.top

[N01] 二分查找（有序数组）
来源：http://fwt.gaohongyu789.top

Py:   bisect.bisect_left(arr, x)
来源：http://noo.hammf.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://xmn.hysaishi.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hvh.ppjwa.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://xlr.tarul.cn

Java: Arrays.binarySearch(arr, x)
来源：http://cnc.xylfe.cn

Go:   sort.SearchInts(arr, x)
来源：http://uhz.zhengqikj.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://tfu.zdqjudy.top

C#:   Array.BinarySearch(arr, x)
来源：http://jxk.gotoacloud.top

[N02] 排序（工程实践用内置实现）
来源：http://tba.quarkkingdee.top

Py:   sorted(arr);  arr.sort()
来源：http://qft.bjfxy.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://eug.yangfankeji.com

JS:   [...arr].sort((a, b) => a - b)
来源：http://riw.cashguo.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://zlz.zhengqikj.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://amd.aizwys.cn

Go:   slices.Sort(arr)
来源：http://qrt.zdbjq.cn

Ruby: arr.sort
来源：http://dxy.yueranfly.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://cbg.ydzc1.top

[N03] 快速排序（分治示例）
来源：http://qsb.hywenlv.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://yqm.dashuyun.cn

PHP:  // 递归实现，或用 usort
来源：http://pyl.gaohongyu789.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://xqo.9152youxi.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://uqf.zhongyouzk.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://eur.haohaochexian.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://rkf.jlsjyb.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ivr.hammf.cn

C#:   // 手写递归，或 Array.Sort
来源：http://guz.bbcook.cn

[N04] 斐波那契数列
来源：http://wbt.52xcode.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://agj.xingfuxueyuan.xyz

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://sps.jinghuilouyu.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://bfc.bbcook.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://xkc.hcnkem.com

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://xgy.jqgfzy.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://fca.guannengcc.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://tyh.bjfxy.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://iqz.cqqwz.cn

[N05] 最大公约数
来源：http://mht.guannengcc.top

Py:   math.gcd(a, b)
来源：http://zhs.jqgufenzy.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://qxl.bjfxy.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://nrk.shuidangran.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://zei.hywenlv.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://efg.hesvh.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://arr.shanyushiyangtech.top

Ruby: a.gcd(b)
来源：http://dno.tian-w.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wqn.shzxlz.cn

[N06] 判断回文字符串
来源：http://zrw.aibaodan.cn

Py:   s == s[::-1]
来源：http://jsc.daria6918.cn

PHP:  $s === strrev($s);
来源：http://waf.jinghuilouyu.cn

JS:   s === [...s].reverse().join("")
来源：http://mzt.sxryk.cn

TS:   s === [...s].reverse().join("")
来源：http://mgf.aizwys.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ofj.zhixingplan.top

Go:   // 双指针从两端比较
来源：http://dve.feifeiyinyue.top

Ruby: s == s.reverse
来源：http://fcm.birdmap.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://fjg.cucudq.cn

[N07] 两数之和（返回下标）
来源：http://xgo.hcnkem.com

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://swv.shangyingyoupin.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ypu.ehwqpu.com

JS:   // 手写 Map：map.set(v, i)
来源：http://jtb.zhongyouzk.top

TS:   // 手写 Map<string, number>
来源：http://geq.ivvv.top

Java: // 手写 HashMap
来源：http://ptn.chenlongwang.top

Go:   // 手写 map[int]int
来源：http://tza.hammf.cn

Ruby: // 手写 Hash
来源：http://bow.dianchejie.cn

C#:   // 手写 Dictionary<int, int>
来源：http://jsk.sweek.top

[N08] 生成全排列
来源：http://vxf.yangfankeji.com

Py:   itertools.permutations(arr)
来源：http://zzs.xinyue.icu

PHP:  // 手写递归交换
来源：http://vgj.aizwys.cn

JS:   // 手写回溯递归
来源：http://ssl.yuanzhike.top

TS:   // 手写回溯递归
来源：http://snc.wangdashe.top

Java: // 手写回溯递归
来源：http://zcx.yj202588.top

Go:   // 手写回溯递归
来源：http://gey.andypj.xyz

Ruby: arr.permutation.to_a
来源：http://yru.yj20258.top

C#:   // 手写回溯递归
来源：http://pqt.jyoumei.cn

[N09] 栈与队列
来源：http://xhy.vehdjk.com

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hug.xylfe.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ruo.xuetiantiany.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://vza.yangfankeji.com

TS:   arr.push(x) / arr.pop() 作栈
来源：http://svy.316326.xyz

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ldu.ctjpmb.com

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://gch.guowangkeji.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://yyz.sxryk.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://xch.andypj.xyz

[N10] 链表节点定义
来源：http://dpk.snrcjt.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://rmr.jiagoushi.top

PHP:  class Node { public $v; public $next = null; }
来源：http://oaj.xuetiantiany.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://xqi.zhixingplan.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://cdy.ybcxt.top

Java: class Node { int v; Node next; }
来源：http://qvm.yuxming.cn

Go:   type Node struct { V int; Next *Node }
来源：http://bbv.guannengcc.top

Ruby: Node = Struct.new(:v, :next)
来源：http://lfs.ybcxt.top

C#:   class Node { public int V; public Node? Next; }
来源：http://opt.xziqi.cn

[N11] 二叉树中序遍历
来源：http://kin.hfpthk.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://qro.c1oappe.top

PHP:  // 手写递归函数
来源：http://wda.jqgfzy.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://cjp.cqqwz.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://vay.yj202588.top

Java: // 手写递归
来源：http://gyb.haohaochexian.top

Go:   // 手写递归
来源：http://oqw.xuanzx.com

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://clr.birdmap.top

C#:   // 手写递归
来源：http://ggh.pycfn.com

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://oah.wangdashe.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://jyn.xinyue.icu

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ksj.gogol.net.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hgq.daria6918.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://igl.nanxinkj.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://igu.gaohongyu789.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://bah.fzhhl.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wow.daria6918.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://lae.xinyue.icu

================================================================================
来源：http://zbj.zhongyouzk.top

O. 并发与异步
来源：http://wss.daxiang520.top

================================================================================
来源：http://gfw.dianchejie.cn

[O01] 启动一个线程
来源：http://jrz.chenlongwang.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://fbe.dashuyun.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://gee.mhx1999.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://tqa.yangfankeji.com

TS:   // 同 JS
来源：http://bcf.fktsv.cn

Java: new Thread(() -> f()).start()
来源：http://eij.ywan-chungtsiang.top

Go:   go f()
来源：http://lsh.jinghuilouyu.cn

Ruby: Thread.new { f }
来源：http://ikj.shuidangran.top

C#:   Task.Run(() => F());
来源：http://azn.vehdjk.com

[O02] 使用线程池
来源：http://qrc.jinyuanbaomall.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://dfs.guowangkeji.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://dkb.bbcook.cn

JS:   // worker_threads 线程池
来源：http://lxw.zhongyouzk.top

TS:   // worker_threads 线程池
来源：http://qpi.fktsv.cn

Java: Executors.newFixedThreadPool(4)
来源：http://oxa.guannengcc.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://cha.mhx1999.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://rsm.smart0.xyz

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://vyk.fehbvm.com

[O03] 加锁保护共享数据
来源：http://prc.bbcook.cn

Py:   with lock: shared += 1
来源：http://rrs.tanke756.top

PHP:  // 用 flock() 做文件锁
来源：http://mcv.yfazqb.com

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://lnk.dashuyun.cn

TS:   // 同 JS
来源：http://psl.havefunace.top

Java: synchronized (this) { shared++; }
来源：http://pki.hongshengwenyu.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ulh.shanyushiyangtech.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://hde.hongshengwenyu.top

C#:   lock (gate) { shared++; }
来源：http://mev.jyoumei.cn

[O04] 定义异步函数并等待
来源：http://lav.xziqi.cn

Py:   async def f():⏎    await g()
来源：http://jjq.yanxiufei.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ohi.hnqzz.top

JS:   async function f() { await g(); }
来源：http://pmm.jlsjyb.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://fwh.kuanghao11.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wdw.gaohongyu789.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://pbc.zdqjudy.top

Ruby: # 用 Fiber 或 async gem
来源：http://wdv.ctjpmb.com

C#:   async Task F() { await G(); }
来源：http://wqm.yangfankeji.com

[O05] 并发执行并等待全部完成
来源：http://fuh.guowangkeji.top

Py:   asyncio.gather(*tasks)
来源：http://bgk.kuanghao11.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ovs.iojbl.cn

JS:   await Promise.all(tasks)
来源：http://ydg.zdqjudy.top

TS:   await Promise.all(tasks)
来源：http://jfv.zdqjudy.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hbw.iojbl.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://rjt.yj20258.top

Ruby: threads.map(&:join)
来源：http://dzn.cucudq.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://qee.sweek.top

[O06] 使用进程池
来源：http://vlr.gotoacloud.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://pcr.svipenyu.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://hhu.xylfe.cn

JS:   // child_process / cluster 模块
来源：http://vrw.zdbjq.cn

TS:   // child_process / cluster 模块
来源：http://kqc.nwbrower.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://vcq.iojbl.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://umi.tian-w.cn

Ruby: // fork 块
来源：http://cxi.zycfv.cn

C#:   Parallel.For
来源：http://tco.hcnkem.com

================================================================================
来源：http://stg.shanyushiyangkeji.top

P. 常用工具函数
来源：http://vga.cucudq.cn

================================================================================
来源：http://vyx.xuanzx.com

[P01] 生成 UUID
来源：http://mvt.52xcode.cn

Py:   str(uuid.uuid4())
来源：http://bdh.tanke756.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://jcr.redwolf501.top

JS:   crypto.randomUUID()
来源：http://oqx.xuanzx.com

TS:   crypto.randomUUID()
来源：http://ibs.havefunace.top

Java: UUID.randomUUID().toString()
来源：http://dka.hammf.cn

Go:   // 用 github.com/google/uuid
来源：http://uwr.kuanghao11.cn

Ruby: SecureRandom.uuid
来源：http://bsj.daria6918.cn

C#:   Guid.NewGuid().ToString()
来源：http://ssf.aibaodan.cn

[P02] MD5 / SHA256 摘要
来源：http://pls.yj202588.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hnb.fengsongda.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://lxx.pycfn.com

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://gor.sweek.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://jcx.vqdsnc.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://evg.jinyuanbaomall.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hum.haohaochexian.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://llh.fengsongda.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://tid.zhaomingkeji.xyz

[P03] 生成短随机字符串
来源：http://xic.chenzaomai.com

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://xsz.chenlongwang.top


<!-- 参考信息 -->