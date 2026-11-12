代发 wailian999

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://bkr.ivvv.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://opl.yj20258.top

[L05] 上传文件（multipart）
来源：http://rmz.nwbrower.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://kmf.ywan-chungtsiang.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://boc.yanxiufei.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://xoi.gaohongyu789.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://syu.xziqi.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://bic.cqqwz.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://jgb.feifeiyinyue.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://zwp.aibaodan.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://puf.aibaodan.cn

[L06] 解析响应为 JSON
来源：http://ytl.shangyingyoupin.top

Py:   resp.json()
来源：http://pqs.yuxming.cn

PHP:  json_decode($body, true);
来源：http://lmy.sweek.top

JS:   await resp.json()
来源：http://tdl.smart0.xyz

TS:   await resp.json()
来源：http://pvc.tanke756.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hkq.fehbvm.com

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://fnt.quarkkingdee.top

Ruby: JSON.parse(resp.body)
来源：http://mqy.zycfv.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ldd.jinghuilouyu.cn

[L07] 处理 HTTP 状态码
来源：http://oqk.ehwqpu.com

Py:   resp.status_code;  resp.raise_for_status()
来源：http://zda.cdnleiting.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wbp.gaohongyu789.top

JS:   resp.ok;  resp.status
来源：http://opk.hnqzz.top

TS:   resp.ok;  resp.status
来源：http://cjm.smart0.xyz

Java: resp.statusCode()
来源：http://mak.ppjwa.cn

Go:   resp.StatusCode
来源：http://afe.hywenlv.cn

Ruby: resp.code.to_i
来源：http://lnp.dianchejie.cn

C#:   (int)resp.StatusCode
来源：http://wap.kuanghao11.cn

[L08] 并发请求多个地址
来源：http://cfp.xingfuxueyuan.xyz

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wak.zhaomingkeji.xyz

PHP:  curl_multi_init() 系列
来源：http://jdi.chenzaomai.com

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://fls.iojbl.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://iue.ydjk.org.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://inz.chenjidiqi.icu

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://quh.hywenlv.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://dzf.0kj1m.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://tmj.zhijiandao.cn

================================================================================
来源：http://vgk.shangyingyoupin.top

M. 命令行 / 进程 / 环境
来源：http://gdj.ydzc1.top

================================================================================
来源：http://lde.sysykeji.top

[M01] 读取命令行参数
来源：http://gwt.52xcode.cn

Py:   sys.argv[1:]
来源：http://xlj.cqqwz.cn

PHP:  $argv;  $argc;
来源：http://dbf.guowangkeji.top

JS:   process.argv.slice(2)
来源：http://xdw.sysykeji.top

TS:   process.argv.slice(2)
来源：http://vaf.jianghu66.top

Java: args 数组（main 方法参数）
来源：http://jpi.shanyushiyangkeji.top

Go:   os.Args[1:]
来源：http://scu.epnwcf.com

Ruby: ARGV
来源：http://gfv.ehwqpu.com

C#:   args 数组（Main 方法参数）
来源：http://zap.shanyushiyangtech.top

[M02] 读取环境变量
来源：http://vzs.zhengqikj.top

Py:   os.environ.get("HOME")
来源：http://zzk.yj20258888.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://sno.shanyushiyangtech.top

JS:   process.env.HOME
来源：http://huj.ppjwa.cn

TS:   process.env.HOME
来源：http://kez.yangfankeji.com

Java: System.getenv("HOME")
来源：http://xte.gzhubu.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://gxn.birdmap.top

Ruby: ENV["HOME"]
来源：http://ley.zhongyouzk.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://yzn.jinqigufen.top

[M03] 执行外部命令
来源：http://vta.bbcook.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://gbg.yangfankeji.com

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://rui.tianlin.xyz

JS:   child_process.execSync("ls -l").toString()
来源：http://cbj.tarul.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://zjv.zdqjudy.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://vua.smart0.xyz

Go:   exec.Command("ls", "-l").Output()
来源：http://lou.jiagoushi.top

Ruby: system("ls -l");  `ls -l`
来源：http://zsy.cqqwz.cn

C#:   Process.Start("ls", "-l");
来源：http://fbu.meibo888.top

[M04] 获取当前工作目录
来源：http://tvh.yongpay.top

Py:   os.getcwd()
来源：http://uje.cheryme.top

PHP:  getcwd();
来源：http://urz.guowangkeji.top

JS:   process.cwd()
来源：http://icp.zhixingplan.top

TS:   process.cwd()
来源：http://esy.nwbrower.top

Java: Path.of("").toAbsolutePath()
来源：http://cwf.ppjwa.cn

Go:   os.Getwd()
来源：http://qrw.sweek.top

Ruby: Dir.pwd
来源：http://eql.xinyue.icu

C#:   Directory.GetCurrentDirectory()
来源：http://yif.hysaishi.cn

[M05] 设置退出码
来源：http://krw.ydzc1.top

Py:   sys.exit(1)
来源：http://hvr.bjfxy.top

PHP:  exit(1);
来源：http://ayh.zhixingplan.top

JS:   process.exit(1)
来源：http://jfh.chenlongwang.top

TS:   process.exit(1)
来源：http://thh.svipenyu.cn

Java: System.exit(1)
来源：http://qgj.zhiwuduotai.top

Go:   os.Exit(1)
来源：http://mhg.yvedp.cn

Ruby: exit 1
来源：http://jwl.guowangkeji.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://eli.xylfe.cn

[M06] 向标准错误输出
来源：http://dkz.xuanzx.com

Py:   print("err", file=sys.stderr)
来源：http://dgv.sysykeji.top

PHP:  fwrite(STDERR, "err\n");
来源：http://lxy.kuanghao11.cn

JS:   console.error("err")
来源：http://rzt.yuxming.cn

TS:   console.error("err")
来源：http://ojs.fktsv.cn

Java: System.err.println("err")
来源：http://ivx.yj20258888.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://tze.cheryme.top

Ruby: warn "err"
来源：http://qxt.yongpay.top

C#:   Console.Error.WriteLine("err")
来源：http://sxf.fzhhl.top

[M07] 判断是否为主入口
来源：http://qjr.hfpthk.cn

Py:   if __name__ == "__main__":
来源：http://zxg.mhx1999.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://tlz.iojbl.cn

JS:   require.main === module
来源：http://kaf.yfazqb.com

TS:   require.main === module
来源：http://eyf.zhijiandao.cn

Java: public static void main(String[] args)
来源：http://wiu.yj202588.top

Go:   func main()
来源：http://ywr.redwolf501.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://cfg.sysykeji.top

C#:   static void Main(string[] args)
来源：http://feo.aizwys.cn

[M08] 获取系统与运行时信息
来源：http://qzf.redwolf501.top

Py:   platform.system();  platform.python_version()
来源：http://ytw.havefunace.top

PHP:  PHP_OS;  phpversion();
来源：http://anx.hnqzz.top

JS:   process.platform;  process.version
来源：http://wpi.yj20258.top

TS:   process.platform;  process.version
来源：http://imj.xziqi.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://pwj.cheryme.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://asq.yj20258.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://req.meibo888.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://awl.vehdjk.com

================================================================================
来源：http://txo.9152youxi.cn

N. 数据结构与算法
来源：http://ogf.cqqwz.cn

================================================================================
来源：http://zos.daria6918.cn

[N01] 二分查找（有序数组）
来源：http://ggo.yvedp.cn

Py:   bisect.bisect_left(arr, x)
来源：http://gke.iojbl.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://sva.shangyingyoupin.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://oay.52xcode.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://rwh.aibaodan.cn

Java: Arrays.binarySearch(arr, x)
来源：http://hcq.mhx1999.top

Go:   sort.SearchInts(arr, x)
来源：http://xnt.daxiang520.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://vjg.snrcjt.cn

C#:   Array.BinarySearch(arr, x)
来源：http://qde.zhongyouzk.top

[N02] 排序（工程实践用内置实现）
来源：http://ffa.andypj.xyz

Py:   sorted(arr);  arr.sort()
来源：http://shk.ctjpmb.com

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://nmb.feifeiyinyue.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://cox.guowangkeji.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://egr.jyoumei.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://lwz.jinghuilouyu.cn

Go:   slices.Sort(arr)
来源：http://vip.yj20258888.top

Ruby: arr.sort
来源：http://msw.dashuyun.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://ocf.yuanzhike.top

[N03] 快速排序（分治示例）
来源：http://xpm.jqgfzy.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://jpp.ydzc1.top

PHP:  // 递归实现，或用 usort
来源：http://cah.hnqzz.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://afb.svipenyu.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://aif.mhx1999.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://rsr.jqgufenzy.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://bwi.svipenyu.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mnz.epnwcf.com

C#:   // 手写递归，或 Array.Sort
来源：http://rql.316326.xyz

[N04] 斐波那契数列
来源：http://rsd.smart0.xyz

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hxe.ctjpmb.com

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://lpj.bbcook.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ubd.gzhubu.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://phq.c1oappe.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ked.yj20258.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://pma.pycfn.com

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://vvd.bbcook.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wbx.cucudq.cn

[N05] 最大公约数
来源：http://toq.yuanzhike.top

Py:   math.gcd(a, b)
来源：http://scy.dashuyun.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ibp.sweek.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://eam.0kj1m.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://rbo.chenjidiqi.icu

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wyn.9152youxi.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://nmu.jinghuilouyu.cn

Ruby: a.gcd(b)
来源：http://yys.9152youxi.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://uiq.zhongyouzk.top

[N06] 判断回文字符串
来源：http://qoe.ywan-chungtsiang.top

Py:   s == s[::-1]
来源：http://erz.yuanzhike.top

PHP:  $s === strrev($s);
来源：http://afs.hywenlv.cn

JS:   s === [...s].reverse().join("")
来源：http://jbb.yueranfly.top

TS:   s === [...s].reverse().join("")
来源：http://zno.zhiwuduotai.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://btm.jianghu66.top

Go:   // 双指针从两端比较
来源：http://gmp.jinqigfzy.top

Ruby: s == s.reverse
来源：http://hnx.9152youxi.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://vfh.sysykeji.top

[N07] 两数之和（返回下标）
来源：http://pdq.zhiwuduotai.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wis.fanxiaobao.xyz

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://xtl.vehdjk.com

JS:   // 手写 Map：map.set(v, i)
来源：http://cgy.fanxiaobao.xyz

TS:   // 手写 Map<string, number>
来源：http://mdh.jinqigfzy.top

Java: // 手写 HashMap
来源：http://hfu.pengpengdd.cyou

Go:   // 手写 map[int]int
来源：http://kom.ydzc1.top

Ruby: // 手写 Hash
来源：http://oog.zhongyouzk.top

C#:   // 手写 Dictionary<int, int>
来源：http://mfm.xingfuxueyuan.xyz

[N08] 生成全排列
来源：http://ewh.ppjwa.cn

Py:   itertools.permutations(arr)
来源：http://rrt.yongpay.top

PHP:  // 手写递归交换
来源：http://lcm.hammf.cn

JS:   // 手写回溯递归
来源：http://spg.epnwcf.com

TS:   // 手写回溯递归
来源：http://ozn.sufxvd.cn

Java: // 手写回溯递归
来源：http://swy.9152youxi.cn

Go:   // 手写回溯递归
来源：http://ciu.hysaishi.cn

Ruby: arr.permutation.to_a
来源：http://ago.yueranfly.top

C#:   // 手写回溯递归
来源：http://jwk.bjfxy.top

[N09] 栈与队列
来源：http://hqp.tian-w.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://odf.tianlin.xyz

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://nyy.jiagoushi.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://dkv.xinyue.icu

TS:   arr.push(x) / arr.pop() 作栈
来源：http://nhv.jinyuanbaomall.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mqk.smart0.xyz

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://jxd.haohaochexian.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://xww.yueranfly.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://fou.ppjwa.cn

[N10] 链表节点定义
来源：http://tnc.uphjek.com

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://elz.zycfv.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://eha.hysaishi.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://fjv.gzhubu.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://moh.ppjwa.cn

Java: class Node { int v; Node next; }
来源：http://gzk.zhixingplan.top

Go:   type Node struct { V int; Next *Node }
来源：http://aac.ehwqpu.com

Ruby: Node = Struct.new(:v, :next)
来源：http://omm.snrcjt.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://oqx.jianghu66.top

[N11] 二叉树中序遍历
来源：http://xxy.fktsv.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hcu.shuidangran.top

PHP:  // 手写递归函数
来源：http://gce.yuanzhike.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://chh.aibaodan.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://pke.cqqwz.cn

Java: // 手写递归
来源：http://lgv.dashuyun.cn

Go:   // 手写递归
来源：http://luq.daxiang520.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://nte.fehbvm.com

C#:   // 手写递归
来源：http://qsy.sxryk.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://tzn.chenjidiqi.icu

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://qyk.hcnkem.com

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://pyr.guannengcc.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://pqt.shzxlz.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ssf.cucudq.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://byc.shanyushiyangtech.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://qdv.dashuyun.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://sjo.yuxming.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://sow.andypj.xyz

================================================================================
来源：http://fha.hysaishi.cn

O. 并发与异步
来源：http://gco.chenlongwang.top

================================================================================
来源：http://koz.yj202588.top

[O01] 启动一个线程
来源：http://hur.birdmap.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ggc.yj202588.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://abl.shanyushiyangtech.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://qfj.cheryme.top

TS:   // 同 JS
来源：http://ocf.vehdjk.com

Java: new Thread(() -> f()).start()
来源：http://lfj.aizwys.cn

Go:   go f()
来源：http://ovb.sufxvd.cn

Ruby: Thread.new { f }
来源：http://qfz.chenjidiqi.icu

C#:   Task.Run(() => F());
来源：http://bmk.hcnkem.com

[O02] 使用线程池
来源：http://xay.dianchejie.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://cbv.yvedp.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wya.guowangkeji.top

JS:   // worker_threads 线程池
来源：http://vyo.yvedp.cn

TS:   // worker_threads 线程池
来源：http://gbc.tianlin.xyz

Java: Executors.newFixedThreadPool(4)
来源：http://ceg.zhijiandao.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://iqv.gaohongyu789.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://lgb.fehbvm.com

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wqy.smart0.xyz

[O03] 加锁保护共享数据
来源：http://cxp.pengpengdd.cyou

Py:   with lock: shared += 1
来源：http://dzw.gogol.net.cn

PHP:  // 用 flock() 做文件锁
来源：http://zvd.zhaomingkeji.xyz

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://erl.ywan-chungtsiang.top

TS:   // 同 JS
来源：http://lkd.zycfv.cn

Java: synchronized (this) { shared++; }
来源：http://uih.hcnkem.com

Go:   mu.Lock();  defer mu.Unlock()
来源：http://zpw.ehwqpu.com

Ruby: mutex.synchronize { shared += 1 }
来源：http://wgz.sufxvd.cn

C#:   lock (gate) { shared++; }
来源：http://mfo.ydjk.org.cn

[O04] 定义异步函数并等待
来源：http://xbv.fehbvm.com

Py:   async def f():⏎    await g()
来源：http://hnk.zhaomingkeji.xyz

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://upm.uphjek.com

JS:   async function f() { await g(); }
来源：http://emo.smart0.xyz

TS:   async function f(): Promise<void> { await g(); }
来源：http://olk.hcnkem.com

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ecl.xylfe.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://dqv.feifeiyinyue.top

Ruby: # 用 Fiber 或 async gem
来源：http://qqm.feifeiyinyue.top

C#:   async Task F() { await G(); }
来源：http://bbh.guannengcc.top

[O05] 并发执行并等待全部完成
来源：http://ebg.jinghuilouyu.cn

Py:   asyncio.gather(*tasks)
来源：http://ard.pengpengdd.cyou

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://jwx.aibaodan.cn

JS:   await Promise.all(tasks)
来源：http://fwy.xylfe.cn

TS:   await Promise.all(tasks)
来源：http://sln.tarul.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://fnv.zdbjq.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://kpo.bjfxy.top

Ruby: threads.map(&:join)
来源：http://cbn.yj20258.top

C#:   await Task.WhenAll(t1, t2)
来源：http://afl.yanxiufei.cn

[O06] 使用进程池
来源：http://kck.cheryme.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://rnu.zhixingplan.top

PHP:  // pcntl_fork 或多进程队列
来源：http://eyq.kuanghao11.cn

JS:   // child_process / cluster 模块
来源：http://xeb.wangdashe.top

TS:   // child_process / cluster 模块
来源：http://mqw.tarul.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://iog.shanyushiyangkeji.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://noe.tarul.cn

Ruby: // fork 块
来源：http://rdx.kuanghao11.cn

C#:   Parallel.For
来源：http://uzf.xinyue.icu

================================================================================
来源：http://xxx.birdmap.top

P. 常用工具函数
来源：http://cqa.ctjpmb.com

================================================================================
来源：http://hjw.xingfuxueyuan.xyz

[P01] 生成 UUID
来源：http://jux.vehdjk.com

Py:   str(uuid.uuid4())
来源：http://oov.hfpthk.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://nga.dashuyun.cn

JS:   crypto.randomUUID()
来源：http://pgt.gotoacloud.top

TS:   crypto.randomUUID()
来源：http://afv.wangshuangyany.cn

Java: UUID.randomUUID().toString()
来源：http://fed.ydzc1.top

Go:   // 用 github.com/google/uuid
来源：http://ilr.ivvv.top

Ruby: SecureRandom.uuid
来源：http://cht.yvedp.cn

C#:   Guid.NewGuid().ToString()
来源：http://ewb.shangyingyoupin.top

[P02] MD5 / SHA256 摘要
来源：http://ltb.zycfv.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://aje.ybcxt.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://noo.zhixingplan.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hex.havefunace.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://csj.xziqi.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://yyz.nanxuanxn.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://igi.uphjek.com


<!-- 参考信息 -->