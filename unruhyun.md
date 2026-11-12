代发 wailian999

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ngv.cashguo.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://vov.cdnleiting.top

[L05] 上传文件（multipart）
来源：http://ptn.cdnleiting.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ley.bbcook.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ccm.ywan-chungtsiang.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://pxf.jinqigufen.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://qjv.guowangkeji.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://isp.birdmap.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://dtx.dashuyun.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://krg.svipenyu.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://smg.hnqzz.top

[L06] 解析响应为 JSON
来源：http://bhv.yvedp.cn

Py:   resp.json()
来源：http://nex.wangdashe.top

PHP:  json_decode($body, true);
来源：http://vut.zhengqikj.top

JS:   await resp.json()
来源：http://pll.shzxlz.cn

TS:   await resp.json()
来源：http://ojo.sufxvd.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://tze.uphjek.com

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://gkg.hfpthk.cn

Ruby: JSON.parse(resp.body)
来源：http://xsz.jyoumei.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://lat.fengsongda.top

[L07] 处理 HTTP 状态码
来源：http://bwx.ivvv.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://nqf.fengsongda.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://lrz.wangshuangyany.cn

JS:   resp.ok;  resp.status
来源：http://fvo.shzxlz.cn

TS:   resp.ok;  resp.status
来源：http://gnh.sxryk.cn

Java: resp.statusCode()
来源：http://jry.9152youxi.cn

Go:   resp.StatusCode
来源：http://oar.daria6918.cn

Ruby: resp.code.to_i
来源：http://eim.zhaomingkeji.xyz

C#:   (int)resp.StatusCode
来源：http://bau.guowangkeji.top

[L08] 并发请求多个地址
来源：http://hhm.daria6918.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://lfx.chenzaomai.com

PHP:  curl_multi_init() 系列
来源：http://huz.smart0.xyz

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://jpr.chenlongwang.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://tyu.cucudq.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://dvv.yfazqb.com

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://rse.52xcode.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://pon.tianlin.xyz

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://rat.aizwys.cn

================================================================================
来源：http://stp.hcnkem.com

M. 命令行 / 进程 / 环境
来源：http://izf.xylfe.cn

================================================================================
来源：http://kva.yangfankeji.com

[M01] 读取命令行参数
来源：http://okm.sufxvd.cn

Py:   sys.argv[1:]
来源：http://vpf.daria6918.cn

PHP:  $argv;  $argc;
来源：http://vdx.gotoacloud.top

JS:   process.argv.slice(2)
来源：http://npo.xuanzx.com

TS:   process.argv.slice(2)
来源：http://jey.kuanghao11.cn

Java: args 数组（main 方法参数）
来源：http://pzf.fanxiaobao.xyz

Go:   os.Args[1:]
来源：http://ylr.zhijiandao.cn

Ruby: ARGV
来源：http://bir.ctjpmb.com

C#:   args 数组（Main 方法参数）
来源：http://rsg.feifeiyinyue.top

[M02] 读取环境变量
来源：http://yyr.fanxiaobao.xyz

Py:   os.environ.get("HOME")
来源：http://tlv.xziqi.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://lov.hnqzz.top

JS:   process.env.HOME
来源：http://ars.vehdjk.com

TS:   process.env.HOME
来源：http://enn.jqgfzy.top

Java: System.getenv("HOME")
来源：http://jqh.fktsv.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://rxs.chenlongwang.top

Ruby: ENV["HOME"]
来源：http://zkw.tianlin.xyz

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hpk.kuanghao11.cn

[M03] 执行外部命令
来源：http://mux.nwbrower.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://myw.cqqwz.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://qyv.jiagoushi.top

JS:   child_process.execSync("ls -l").toString()
来源：http://kbq.jinqigufen.top

TS:   child_process.execSync("ls -l").toString()
来源：http://eyf.quarkkingdee.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://pjf.sufxvd.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://mxg.zhijiandao.cn

Ruby: system("ls -l");  `ls -l`
来源：http://ouk.zhongyouzk.top

C#:   Process.Start("ls", "-l");
来源：http://eag.yanxiufei.cn

[M04] 获取当前工作目录
来源：http://vvv.smart0.xyz

Py:   os.getcwd()
来源：http://mqj.jqgufenzy.top

PHP:  getcwd();
来源：http://xdp.shanyushiyangtech.top

JS:   process.cwd()
来源：http://cbf.birdmap.top

TS:   process.cwd()
来源：http://fxk.jlsjyb.cn

Java: Path.of("").toAbsolutePath()
来源：http://utd.uphjek.com

Go:   os.Getwd()
来源：http://kfq.9152youxi.cn

Ruby: Dir.pwd
来源：http://czm.pengpengdd.cyou

C#:   Directory.GetCurrentDirectory()
来源：http://xvo.bbcook.cn

[M05] 设置退出码
来源：http://mba.hnqzz.top

Py:   sys.exit(1)
来源：http://fwn.epnwcf.com

PHP:  exit(1);
来源：http://ptd.xuanzx.com

JS:   process.exit(1)
来源：http://bin.daria6918.cn

TS:   process.exit(1)
来源：http://lmq.zhijiandao.cn

Java: System.exit(1)
来源：http://xil.tianlin.xyz

Go:   os.Exit(1)
来源：http://nuv.cqqwz.cn

Ruby: exit 1
来源：http://pjh.yj20258.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://jpq.tian-w.cn

[M06] 向标准错误输出
来源：http://wli.dashuyun.cn

Py:   print("err", file=sys.stderr)
来源：http://oxv.zhoulong.xyz

PHP:  fwrite(STDERR, "err\n");
来源：http://upp.sufxvd.cn

JS:   console.error("err")
来源：http://zpp.hammf.cn

TS:   console.error("err")
来源：http://wdx.gogol.net.cn

Java: System.err.println("err")
来源：http://dqv.guowangkeji.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://yzi.yuanzhike.top

Ruby: warn "err"
来源：http://zjp.uphjek.com

C#:   Console.Error.WriteLine("err")
来源：http://xjz.daxiang520.top

[M07] 判断是否为主入口
来源：http://koe.jianghu66.top

Py:   if __name__ == "__main__":
来源：http://nrn.hesvh.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://bsa.aibaodan.cn

JS:   require.main === module
来源：http://ryc.jqgfzy.top

TS:   require.main === module
来源：http://cfi.jinyuanbaomall.cn

Java: public static void main(String[] args)
来源：http://jfe.sysykeji.top

Go:   func main()
来源：http://gql.tanke756.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://bzr.birdmap.top

C#:   static void Main(string[] args)
来源：http://nwk.bjfxy.top

[M08] 获取系统与运行时信息
来源：http://saf.chenjidiqi.icu

Py:   platform.system();  platform.python_version()
来源：http://inn.cqqwz.cn

PHP:  PHP_OS;  phpversion();
来源：http://qgc.tanke756.top

JS:   process.platform;  process.version
来源：http://zss.yj202588.top

TS:   process.platform;  process.version
来源：http://sdx.52xcode.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://vmf.hysaishi.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://pnk.xuetiantiany.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wtq.cqqwz.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://fxl.guannengcc.top

================================================================================
来源：http://tlv.zhoulong.xyz

N. 数据结构与算法
来源：http://wji.nanxuanxn.top

================================================================================
来源：http://ssc.zhengqikj.top

[N01] 二分查找（有序数组）
来源：http://kau.fengsongda.top

Py:   bisect.bisect_left(arr, x)
来源：http://iqn.zhongyouzk.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://dxj.zhixingplan.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://bqf.meibo888.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://rcq.jqgfzy.top

Java: Arrays.binarySearch(arr, x)
来源：http://gkh.c1oappe.top

Go:   sort.SearchInts(arr, x)
来源：http://rul.dashuyun.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://gmw.sysykeji.top

C#:   Array.BinarySearch(arr, x)
来源：http://pvs.hesvh.cn

[N02] 排序（工程实践用内置实现）
来源：http://dyi.hongshengwenyu.top

Py:   sorted(arr);  arr.sort()
来源：http://duf.nanxinkj.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://nwi.jqgfzy.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://mkm.zhaomingkeji.xyz

TS:   [...arr].sort((a, b) => a - b)
来源：http://swb.jinyuanbaomall.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hbr.bbcook.cn

Go:   slices.Sort(arr)
来源：http://jst.daria6918.cn

Ruby: arr.sort
来源：http://lzr.hongshengwenyu.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://btr.yj20258888.top

[N03] 快速排序（分治示例）
来源：http://skz.fanxiaobao.xyz

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://oil.xuanzx.com

PHP:  // 递归实现，或用 usort
来源：http://mlv.cdnleiting.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://chu.cdnleiting.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://zgt.hfpthk.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mia.zhiwuduotai.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://aku.snrcjt.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hha.c1oappe.top

C#:   // 手写递归，或 Array.Sort
来源：http://uqm.chenzaomai.com

[N04] 斐波那契数列
来源：http://dys.pycfn.com

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://bkh.iojbl.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://otr.kuanghao11.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mpq.tian-w.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://aes.fzhhl.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://jwz.yj20258.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://pwq.snrcjt.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://jxo.shzxlz.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mvq.shuidangran.top

[N05] 最大公约数
来源：http://oae.uphjek.com

Py:   math.gcd(a, b)
来源：http://wbh.dashuyun.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://bgj.yanxiufei.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://rxw.0kj1m.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://jip.cqqwz.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://dwo.xingfuxueyuan.xyz

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://nee.guannengcc.top

Ruby: a.gcd(b)
来源：http://squ.fktsv.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://gan.birdmap.top

[N06] 判断回文字符串
来源：http://mvz.smart0.xyz

Py:   s == s[::-1]
来源：http://opz.xuetiantiany.cn

PHP:  $s === strrev($s);
来源：http://rqu.daxiang520.top

JS:   s === [...s].reverse().join("")
来源：http://yoo.cheryme.top

TS:   s === [...s].reverse().join("")
来源：http://shp.hfpthk.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://fnt.zdqjudy.top

Go:   // 双指针从两端比较
来源：http://dcy.yonumen.top

Ruby: s == s.reverse
来源：http://lww.hfpthk.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://emp.vqdsnc.cn

[N07] 两数之和（返回下标）
来源：http://bju.uphjek.com

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://knb.fehbvm.com

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ury.zhongyouzk.top

JS:   // 手写 Map：map.set(v, i)
来源：http://hqf.dashuyun.cn

TS:   // 手写 Map<string, number>
来源：http://dxs.jlsjyb.cn

Java: // 手写 HashMap
来源：http://bqg.zhongyouzk.top

Go:   // 手写 map[int]int
来源：http://zia.pycfn.com

Ruby: // 手写 Hash
来源：http://uhi.jinqigufen.top

C#:   // 手写 Dictionary<int, int>
来源：http://wpy.yuanzhike.top

[N08] 生成全排列
来源：http://oal.zhiwuduotai.top

Py:   itertools.permutations(arr)
来源：http://fmc.shanyushiyangtech.top

PHP:  // 手写递归交换
来源：http://jrb.gzhubu.top

JS:   // 手写回溯递归
来源：http://gtv.xuetiantiany.cn

TS:   // 手写回溯递归
来源：http://qhe.ivvv.top

Java: // 手写回溯递归
来源：http://usb.fehbvm.com

Go:   // 手写回溯递归
来源：http://gzq.jinqigufen.top

Ruby: arr.permutation.to_a
来源：http://cyb.hysaishi.cn

C#:   // 手写回溯递归
来源：http://std.gogol.net.cn

[N09] 栈与队列
来源：http://vma.ywan-chungtsiang.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://pgk.jqgufenzy.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://amz.birdmap.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ugh.yangfankeji.com

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mtz.epnwcf.com

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://gbf.ehwqpu.com

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ubs.yj20258888.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://cqh.tian-w.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://cox.yj20258.top

[N10] 链表节点定义
来源：http://nfr.yj20258.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://fsi.quarkkingdee.top

PHP:  class Node { public $v; public $next = null; }
来源：http://swd.birdmap.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://drj.sufxvd.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ire.xylfe.cn

Java: class Node { int v; Node next; }
来源：http://klv.meibo888.top

Go:   type Node struct { V int; Next *Node }
来源：http://pkp.aibaodan.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://wax.chenjidiqi.icu

C#:   class Node { public int V; public Node? Next; }
来源：http://qzn.316326.xyz

[N11] 二叉树中序遍历
来源：http://tnz.sufxvd.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://fcz.yj202588.top

PHP:  // 手写递归函数
来源：http://cvk.sxryk.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://pxj.jiagoushi.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://bez.jinqigufen.top

Java: // 手写递归
来源：http://xbo.sjlbkw.cn

Go:   // 手写递归
来源：http://qlp.fanxiaobao.xyz

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://qgl.hywenlv.cn

C#:   // 手写递归
来源：http://yvw.hongshengwenyu.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wyd.316326.xyz

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://qxg.xinyue.icu

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://qmh.nanxinkj.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://gti.xinyue.icu

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://nty.daxiang520.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://luv.shanyushiyangkeji.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://lvt.jiagoushi.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wax.birdmap.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://nsv.yongpay.top

================================================================================
来源：http://gbe.hnqzz.top

O. 并发与异步
来源：http://vbp.aizwys.cn

================================================================================
来源：http://vwy.yj20258888.top

[O01] 启动一个线程
来源：http://lcc.yvedp.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://zms.jyoumei.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://rpu.yj202588.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://bem.zhixingplan.top

TS:   // 同 JS
来源：http://yer.hfpthk.cn

Java: new Thread(() -> f()).start()
来源：http://vra.redwolf501.top

Go:   go f()
来源：http://neq.jinqigfzy.top

Ruby: Thread.new { f }
来源：http://jhn.xuanzx.com

C#:   Task.Run(() => F());
来源：http://kmt.yj20258.top

[O02] 使用线程池
来源：http://efv.chenjidiqi.icu

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mdw.pycfn.com

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://dwr.gaohongyu789.top

JS:   // worker_threads 线程池
来源：http://dlz.ctjpmb.com

TS:   // worker_threads 线程池
来源：http://vrv.yfazqb.com

Java: Executors.newFixedThreadPool(4)
来源：http://csn.hcnkem.com

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://neq.smart0.xyz

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ekv.shanyushiyangtech.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ytx.wangdashe.top

[O03] 加锁保护共享数据
来源：http://jqj.xziqi.cn

Py:   with lock: shared += 1
来源：http://izy.yj202588.top

PHP:  // 用 flock() 做文件锁
来源：http://lyi.zhijiandao.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://sqd.ppjwa.cn

TS:   // 同 JS
来源：http://pan.tanke756.top

Java: synchronized (this) { shared++; }
来源：http://vay.jinyuanbaomall.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://soe.zhiwuduotai.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://oit.aizwys.cn

C#:   lock (gate) { shared++; }
来源：http://liz.wangdashe.top

[O04] 定义异步函数并等待
来源：http://vui.uphjek.com

Py:   async def f():⏎    await g()
来源：http://dxa.zhoulong.xyz

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://elw.zhongyouzk.top

JS:   async function f() { await g(); }
来源：http://jvz.guannengcc.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://aez.zhixingplan.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ctp.guannengcc.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hwc.yuxming.cn

Ruby: # 用 Fiber 或 async gem
来源：http://zfj.jinqigufen.top

C#:   async Task F() { await G(); }
来源：http://gaf.aizwys.cn

[O05] 并发执行并等待全部完成
来源：http://tmv.jqgfzy.top

Py:   asyncio.gather(*tasks)
来源：http://awd.nwbrower.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://gaw.hnxiangtu.top

JS:   await Promise.all(tasks)
来源：http://dye.zhiwuduotai.top

TS:   await Promise.all(tasks)
来源：http://lhh.cqqwz.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://odm.dashuyun.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://lwe.zdbjq.cn

Ruby: threads.map(&:join)
来源：http://sea.dashuyun.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://kus.ybcxt.top

[O06] 使用进程池
来源：http://vxv.chenzaomai.com

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://tei.zycfv.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://vuf.cdnleiting.top

JS:   // child_process / cluster 模块
来源：http://vhp.cucudq.cn

TS:   // child_process / cluster 模块
来源：http://hiy.52xcode.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://fhi.vqdsnc.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ovn.shzxlz.cn

Ruby: // fork 块
来源：http://wja.zhaomingkeji.xyz

C#:   Parallel.For
来源：http://nfe.zhijiandao.cn

================================================================================
来源：http://iyb.shzxlz.cn

P. 常用工具函数
来源：http://xwx.xylfe.cn

================================================================================
来源：http://miv.vehdjk.com

[P01] 生成 UUID
来源：http://thp.ybcxt.top

Py:   str(uuid.uuid4())
来源：http://kjm.cheryme.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://xkr.0kj1m.cn

JS:   crypto.randomUUID()
来源：http://hyj.ybcxt.top

TS:   crypto.randomUUID()
来源：http://lms.nanxuanxn.top

Java: UUID.randomUUID().toString()
来源：http://ncy.bjfxy.top

Go:   // 用 github.com/google/uuid
来源：http://fxo.feifeiyinyue.top

Ruby: SecureRandom.uuid
来源：http://qhi.tarul.cn

C#:   Guid.NewGuid().ToString()
来源：http://ssd.cashguo.top

[P02] MD5 / SHA256 摘要
来源：http://ebp.yuanzhike.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://iwc.sxryk.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://zld.uphjek.com

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://dqt.xuanzx.com

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://irq.shuidangran.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://txf.sweek.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://qsr.52xcode.cn


<!-- 参考信息 -->