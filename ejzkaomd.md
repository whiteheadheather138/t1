代发 wailian999

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://tat.0kj1m.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://gat.yuxming.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ans.jqgfzy.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hmo.iojbl.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hfy.yanxiufei.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://xby.hfpthk.cn

[L05] 上传文件（multipart）
来源：http://aea.ehwqpu.com

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ydl.nanxinkj.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://rlf.wangshuangyany.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://qmr.chenjidiqi.icu

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://jqs.shanyushiyangkeji.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://pyj.jinyuanbaomall.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://nxt.wangshuangyany.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://nkd.jinghuilouyu.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://faq.zhixingplan.top

[L06] 解析响应为 JSON
来源：http://bad.chenzaomai.com

Py:   resp.json()
来源：http://eow.hcnkem.com

PHP:  json_decode($body, true);
来源：http://zmn.mhx1999.top

JS:   await resp.json()
来源：http://kmj.iojbl.cn

TS:   await resp.json()
来源：http://naz.shuidangran.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://rac.cdnleiting.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://had.zhoulong.xyz

Ruby: JSON.parse(resp.body)
来源：http://woi.guannengcc.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://uym.mhx1999.top

[L07] 处理 HTTP 状态码
来源：http://ftk.jinqigufen.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://goz.epnwcf.com

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://gva.yonumen.top

JS:   resp.ok;  resp.status
来源：http://chz.fengsongda.top

TS:   resp.ok;  resp.status
来源：http://hwp.dashuyun.cn

Java: resp.statusCode()
来源：http://xur.uphjek.com

Go:   resp.StatusCode
来源：http://qlu.gotoacloud.top

Ruby: resp.code.to_i
来源：http://xno.birdmap.top

C#:   (int)resp.StatusCode
来源：http://caf.xylfe.cn

[L08] 并发请求多个地址
来源：http://zlb.jiagoushi.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://frs.dianchejie.cn

PHP:  curl_multi_init() 系列
来源：http://vsm.shanyushiyangkeji.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://jcm.havefunace.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://qan.snrcjt.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wmi.daria6918.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://csv.sysykeji.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://tmj.xinyue.icu

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://sji.guannengcc.top

================================================================================
来源：http://tlz.shangyingyoupin.top

M. 命令行 / 进程 / 环境
来源：http://atk.vehdjk.com

================================================================================
来源：http://crl.yonumen.top

[M01] 读取命令行参数
来源：http://kep.daxiang520.top

Py:   sys.argv[1:]
来源：http://kgy.cqqwz.cn

PHP:  $argv;  $argc;
来源：http://lee.hcnkem.com

JS:   process.argv.slice(2)
来源：http://dgs.xylfe.cn

TS:   process.argv.slice(2)
来源：http://sjk.zycfv.cn

Java: args 数组（main 方法参数）
来源：http://hdd.fehbvm.com

Go:   os.Args[1:]
来源：http://fyo.zhiwuduotai.top

Ruby: ARGV
来源：http://ngc.yfazqb.com

C#:   args 数组（Main 方法参数）
来源：http://exu.jqgufenzy.top

[M02] 读取环境变量
来源：http://rug.316326.xyz

Py:   os.environ.get("HOME")
来源：http://dfx.316326.xyz

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://kog.epnwcf.com

JS:   process.env.HOME
来源：http://juo.hnqzz.top

TS:   process.env.HOME
来源：http://vyn.hfpthk.cn

Java: System.getenv("HOME")
来源：http://eqy.snrcjt.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://lsw.ydzc1.top

Ruby: ENV["HOME"]
来源：http://crh.0kj1m.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://xpu.quarkkingdee.top

[M03] 执行外部命令
来源：http://xuq.havefunace.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ebp.zhengqikj.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ogm.jianghu66.top

JS:   child_process.execSync("ls -l").toString()
来源：http://cfd.0kj1m.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://onv.ivvv.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://cza.yj20258.top

Go:   exec.Command("ls", "-l").Output()
来源：http://rfw.daria6918.cn

Ruby: system("ls -l");  `ls -l`
来源：http://gjd.kuanghao11.cn

C#:   Process.Start("ls", "-l");
来源：http://nhl.shanyushiyangtech.top

[M04] 获取当前工作目录
来源：http://pfy.mhx1999.top

Py:   os.getcwd()
来源：http://bgb.yangfankeji.com

PHP:  getcwd();
来源：http://jlc.cheryme.top

JS:   process.cwd()
来源：http://pnr.jqgfzy.top

TS:   process.cwd()
来源：http://dmz.uphjek.com

Java: Path.of("").toAbsolutePath()
来源：http://gei.gzhubu.top

Go:   os.Getwd()
来源：http://nho.sweek.top

Ruby: Dir.pwd
来源：http://xdc.zhiwuduotai.top

C#:   Directory.GetCurrentDirectory()
来源：http://sya.havefunace.top

[M05] 设置退出码
来源：http://ozu.hcnkem.com

Py:   sys.exit(1)
来源：http://lvl.iojbl.cn

PHP:  exit(1);
来源：http://wlx.cashguo.top

JS:   process.exit(1)
来源：http://twj.zycfv.cn

TS:   process.exit(1)
来源：http://hey.zhiwuduotai.top

Java: System.exit(1)
来源：http://htn.fzhhl.top

Go:   os.Exit(1)
来源：http://hxt.sxryk.cn

Ruby: exit 1
来源：http://yms.pycfn.com

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://noi.jianghu66.top

[M06] 向标准错误输出
来源：http://xje.quarkkingdee.top

Py:   print("err", file=sys.stderr)
来源：http://zsd.havefunace.top

PHP:  fwrite(STDERR, "err\n");
来源：http://edv.yj202588.top

JS:   console.error("err")
来源：http://rbx.yfazqb.com

TS:   console.error("err")
来源：http://chd.sufxvd.cn

Java: System.err.println("err")
来源：http://wkh.snrcjt.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://jmw.jinqigufen.top

Ruby: warn "err"
来源：http://akt.meibo888.top

C#:   Console.Error.WriteLine("err")
来源：http://gqg.sxryk.cn

[M07] 判断是否为主入口
来源：http://nhr.cheryme.top

Py:   if __name__ == "__main__":
来源：http://wdp.tarul.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mnv.nanxinkj.top

JS:   require.main === module
来源：http://jia.hammf.cn

TS:   require.main === module
来源：http://akn.wangdashe.top

Java: public static void main(String[] args)
来源：http://svx.feifeiyinyue.top

Go:   func main()
来源：http://fmt.xinyue.icu

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://yns.tianlin.xyz

C#:   static void Main(string[] args)
来源：http://arx.yj20258.top

[M08] 获取系统与运行时信息
来源：http://tas.cqqwz.cn

Py:   platform.system();  platform.python_version()
来源：http://amq.hongshengwenyu.top

PHP:  PHP_OS;  phpversion();
来源：http://whn.meibo888.top

JS:   process.platform;  process.version
来源：http://bmo.andypj.xyz

TS:   process.platform;  process.version
来源：http://wit.ybcxt.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://lxc.xuetiantiany.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://pnv.svipenyu.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://upe.tanke756.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://zgd.haohaochexian.top

================================================================================
来源：http://ivc.shzxlz.cn

N. 数据结构与算法
来源：http://jjo.cashguo.top

================================================================================
来源：http://rwu.ywan-chungtsiang.top

[N01] 二分查找（有序数组）
来源：http://xmd.birdmap.top

Py:   bisect.bisect_left(arr, x)
来源：http://pqv.wangdashe.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hjq.pengpengdd.cyou

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ykw.cdnleiting.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://tra.shanyushiyangtech.top

Java: Arrays.binarySearch(arr, x)
来源：http://nbo.fanxiaobao.xyz

Go:   sort.SearchInts(arr, x)
来源：http://nof.zycfv.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://isd.zhixingplan.top

C#:   Array.BinarySearch(arr, x)
来源：http://hhn.andypj.xyz

[N02] 排序（工程实践用内置实现）
来源：http://yyz.xuetiantiany.cn

Py:   sorted(arr);  arr.sort()
来源：http://ttp.xziqi.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://epr.wangdashe.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://ejy.shanyushiyangkeji.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://czy.zhijiandao.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://dkc.ehwqpu.com

Go:   slices.Sort(arr)
来源：http://oku.guannengcc.top

Ruby: arr.sort
来源：http://oll.vqdsnc.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://txb.birdmap.top

[N03] 快速排序（分治示例）
来源：http://jbj.fengsongda.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ybe.jianghu66.top

PHP:  // 递归实现，或用 usort
来源：http://ycs.zdbjq.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://cxb.zdbjq.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://kgv.ydzc1.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://fun.hysaishi.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://rsu.mhx1999.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://gsw.cqqwz.cn

C#:   // 手写递归，或 Array.Sort
来源：http://tdd.yuanzhike.top

[N04] 斐波那契数列
来源：http://qft.zhoulong.xyz

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://zyt.jqgufenzy.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://tsd.epnwcf.com

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mth.dianchejie.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://bzz.0kj1m.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://rkr.tarul.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://xhi.jqgfzy.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://qid.zdqjudy.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hzu.bbcook.cn

[N05] 最大公约数
来源：http://nba.pycfn.com

Py:   math.gcd(a, b)
来源：http://job.smart0.xyz

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wjh.ywan-chungtsiang.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://jjd.zhoulong.xyz

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://clu.wangdashe.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://pvt.yanxiufei.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://rpc.tarul.cn

Ruby: a.gcd(b)
来源：http://mcf.vqdsnc.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://aua.yvedp.cn

[N06] 判断回文字符串
来源：http://khh.shanyushiyangtech.top

Py:   s == s[::-1]
来源：http://heo.pengpengdd.cyou

PHP:  $s === strrev($s);
来源：http://bwl.52xcode.cn

JS:   s === [...s].reverse().join("")
来源：http://bly.bbcook.cn

TS:   s === [...s].reverse().join("")
来源：http://hik.jqgufenzy.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mzk.redwolf501.top

Go:   // 双指针从两端比较
来源：http://bck.tian-w.cn

Ruby: s == s.reverse
来源：http://kav.daxiang520.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://btf.xziqi.cn

[N07] 两数之和（返回下标）
来源：http://idw.yangfankeji.com

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://fge.yangfankeji.com

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://smx.jlsjyb.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://zhm.redwolf501.top

TS:   // 手写 Map<string, number>
来源：http://pro.dashuyun.cn

Java: // 手写 HashMap
来源：http://jkb.shuidangran.top

Go:   // 手写 map[int]int
来源：http://fjx.hywenlv.cn

Ruby: // 手写 Hash
来源：http://dly.fengsongda.top

C#:   // 手写 Dictionary<int, int>
来源：http://bqw.jinyuanbaomall.cn

[N08] 生成全排列
来源：http://yyk.daria6918.cn

Py:   itertools.permutations(arr)
来源：http://yag.ctjpmb.com

PHP:  // 手写递归交换
来源：http://cod.aizwys.cn

JS:   // 手写回溯递归
来源：http://cqm.yueranfly.top

TS:   // 手写回溯递归
来源：http://pnt.fanxiaobao.xyz

Java: // 手写回溯递归
来源：http://tpz.sjlbkw.cn

Go:   // 手写回溯递归
来源：http://ajj.kuanghao11.cn

Ruby: arr.permutation.to_a
来源：http://aeg.aibaodan.cn

C#:   // 手写回溯递归
来源：http://ugf.tanke756.top

[N09] 栈与队列
来源：http://djh.jinyuanbaomall.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://gme.shanyushiyangkeji.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://xxq.ivvv.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://swy.gotoacloud.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hla.jqgfzy.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://fcf.gotoacloud.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://zkl.zhijiandao.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mxe.shanyushiyangkeji.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://vpm.cqqwz.cn

[N10] 链表节点定义
来源：http://bef.chenlongwang.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://twm.tianlin.xyz

PHP:  class Node { public $v; public $next = null; }
来源：http://nmi.gzhubu.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://irb.shangyingyoupin.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://vlm.yj20258888.top

Java: class Node { int v; Node next; }
来源：http://hjd.yfazqb.com

Go:   type Node struct { V int; Next *Node }
来源：http://nhq.ydzc1.top

Ruby: Node = Struct.new(:v, :next)
来源：http://ikw.zhaomingkeji.xyz

C#:   class Node { public int V; public Node? Next; }
来源：http://tij.kuanghao11.cn

[N11] 二叉树中序遍历
来源：http://qzb.ydzc1.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://una.ctjpmb.com

PHP:  // 手写递归函数
来源：http://soo.chenlongwang.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://kqc.c1oappe.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://dmz.sxryk.cn

Java: // 手写递归
来源：http://mlj.nanxinkj.top

Go:   // 手写递归
来源：http://zgl.jianghu66.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://fnu.cucudq.cn

C#:   // 手写递归
来源：http://zzi.mhx1999.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://vlx.quarkkingdee.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://tou.dashuyun.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ans.ywan-chungtsiang.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wje.meibo888.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wbj.ywan-chungtsiang.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://jrd.gzhubu.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://xcm.yvedp.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://cwb.uphjek.com

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://nhu.guowangkeji.top

================================================================================
来源：http://vfg.sufxvd.cn

O. 并发与异步
来源：http://ziv.hysaishi.cn

================================================================================
来源：http://ozd.zhengqikj.top

[O01] 启动一个线程
来源：http://awd.hnxiangtu.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://sdi.ctjpmb.com

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://tbk.jianghu66.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://cym.snrcjt.cn

TS:   // 同 JS
来源：http://nif.ybcxt.top

Java: new Thread(() -> f()).start()
来源：http://qml.zhixingplan.top

Go:   go f()
来源：http://qbp.zhijiandao.cn

Ruby: Thread.new { f }
来源：http://mhy.sweek.top

C#:   Task.Run(() => F());
来源：http://umc.uphjek.com

[O02] 使用线程池
来源：http://jit.xingfuxueyuan.xyz

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://tyn.hysaishi.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://xot.sufxvd.cn

JS:   // worker_threads 线程池
来源：http://vdn.tarul.cn

TS:   // worker_threads 线程池
来源：http://ucc.xinyue.icu

Java: Executors.newFixedThreadPool(4)
来源：http://bgz.wangshuangyany.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://dxl.jyoumei.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://dht.jlsjyb.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://dcz.yongpay.top

[O03] 加锁保护共享数据
来源：http://nqe.chenlongwang.top

Py:   with lock: shared += 1
来源：http://dkr.9152youxi.cn

PHP:  // 用 flock() 做文件锁
来源：http://cpu.shanyushiyangtech.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://roh.yueranfly.top

TS:   // 同 JS
来源：http://mjm.mhx1999.top

Java: synchronized (this) { shared++; }
来源：http://ayx.guannengcc.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://iez.xylfe.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://voe.havefunace.top

C#:   lock (gate) { shared++; }
来源：http://exf.mhx1999.top

[O04] 定义异步函数并等待
来源：http://cix.daxiang520.top

Py:   async def f():⏎    await g()
来源：http://xde.yuanzhike.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://csy.0kj1m.cn

JS:   async function f() { await g(); }
来源：http://vmw.yangfankeji.com

TS:   async function f(): Promise<void> { await g(); }
来源：http://iog.yanxiufei.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://rtq.guannengcc.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://vdb.wangdashe.top

Ruby: # 用 Fiber 或 async gem
来源：http://aec.guannengcc.top

C#:   async Task F() { await G(); }
来源：http://eza.hongshengwenyu.top

[O05] 并发执行并等待全部完成
来源：http://hic.cqqwz.cn

Py:   asyncio.gather(*tasks)
来源：http://gsg.yanxiufei.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://xbt.ybcxt.top

JS:   await Promise.all(tasks)
来源：http://xcn.mhx1999.top

TS:   await Promise.all(tasks)
来源：http://dwv.bjfxy.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://dzn.cdnleiting.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ier.zhaomingkeji.xyz

Ruby: threads.map(&:join)
来源：http://nua.svipenyu.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://jti.sxryk.cn

[O06] 使用进程池
来源：http://ctd.fengsongda.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://xvi.nanxinkj.top

PHP:  // pcntl_fork 或多进程队列
来源：http://ffu.sweek.top

JS:   // child_process / cluster 模块
来源：http://utx.jlsjyb.cn

TS:   // child_process / cluster 模块
来源：http://kth.9152youxi.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://uij.xingfuxueyuan.xyz

Go:   // goroutine 已占用多核，直接并发即可
来源：http://nsj.mhx1999.top

Ruby: // fork 块
来源：http://gjw.yj20258.top

C#:   Parallel.For
来源：http://pea.cqqwz.cn

================================================================================
来源：http://art.sysykeji.top

P. 常用工具函数
来源：http://pmd.chenlongwang.top

================================================================================
来源：http://ibx.nanxuanxn.top

[P01] 生成 UUID
来源：http://eay.hnqzz.top

Py:   str(uuid.uuid4())
来源：http://vyp.yueranfly.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://nab.tanke756.top

JS:   crypto.randomUUID()
来源：http://zlc.chenlongwang.top

TS:   crypto.randomUUID()
来源：http://euw.ydzc1.top

Java: UUID.randomUUID().toString()
来源：http://ozh.mhx1999.top

Go:   // 用 github.com/google/uuid
来源：http://imz.jinghuilouyu.cn

Ruby: SecureRandom.uuid
来源：http://yza.zhoulong.xyz

C#:   Guid.NewGuid().ToString()
来源：http://apv.yj20258888.top

[P02] MD5 / SHA256 摘要
来源：http://iya.feifeiyinyue.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://muy.jinqigufen.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://ahs.sxryk.cn


<!-- 参考信息 -->