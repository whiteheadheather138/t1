代发 wailian999

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mab.fengsongda.top

[L04] 设置超时
来源：http://rjd.jlsjyb.cn

Py:   requests.get(url, timeout=5)
来源：http://xjk.hongshengwenyu.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://gxg.gaohongyu789.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://uec.cucudq.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://nru.hesvh.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://cxo.sysykeji.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wbe.birdmap.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://foz.daria6918.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://bvs.yvedp.cn

[L05] 上传文件（multipart）
来源：http://lpx.hywenlv.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://lrm.fanxiaobao.xyz

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ioi.ybcxt.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://heb.dianchejie.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://rfj.svipenyu.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://vdq.fzhhl.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://rkk.jianghu66.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://crb.gaohongyu789.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://fzl.svipenyu.cn

[L06] 解析响应为 JSON
来源：http://mux.birdmap.top

Py:   resp.json()
来源：http://lwx.chenzaomai.com

PHP:  json_decode($body, true);
来源：http://gyr.zhengqikj.top

JS:   await resp.json()
来源：http://fay.316326.xyz

TS:   await resp.json()
来源：http://hmh.fktsv.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://rxt.jlsjyb.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://aeg.cashguo.top

Ruby: JSON.parse(resp.body)
来源：http://fxs.gotoacloud.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://qdn.jinghuilouyu.cn

[L07] 处理 HTTP 状态码
来源：http://srn.gogol.net.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://dhe.haohaochexian.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://jyk.smart0.xyz

JS:   resp.ok;  resp.status
来源：http://snv.cucudq.cn

TS:   resp.ok;  resp.status
来源：http://dqa.zdqjudy.top

Java: resp.statusCode()
来源：http://psq.tian-w.cn

Go:   resp.StatusCode
来源：http://unm.xuetiantiany.cn

Ruby: resp.code.to_i
来源：http://gst.yvedp.cn

C#:   (int)resp.StatusCode
来源：http://aqp.xziqi.cn

[L08] 并发请求多个地址
来源：http://jkf.gotoacloud.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://whh.yj20258888.top

PHP:  curl_multi_init() 系列
来源：http://lfq.cqqwz.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://pfu.havefunace.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://qeo.hfpthk.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ilv.jqgufenzy.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://glt.sjlbkw.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://prc.wangshuangyany.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://sxt.sysykeji.top

================================================================================
来源：http://ibw.havefunace.top

M. 命令行 / 进程 / 环境
来源：http://ero.tanke756.top

================================================================================
来源：http://hyv.fengsongda.top

[M01] 读取命令行参数
来源：http://rde.feifeiyinyue.top

Py:   sys.argv[1:]
来源：http://tot.hysaishi.cn

PHP:  $argv;  $argc;
来源：http://nfh.cucudq.cn

JS:   process.argv.slice(2)
来源：http://qtg.xuanzx.com

TS:   process.argv.slice(2)
来源：http://uqm.ydjk.org.cn

Java: args 数组（main 方法参数）
来源：http://tfs.xinyue.icu

Go:   os.Args[1:]
来源：http://vrx.yonumen.top

Ruby: ARGV
来源：http://phy.smart0.xyz

C#:   args 数组（Main 方法参数）
来源：http://nju.xinyue.icu

[M02] 读取环境变量
来源：http://gvl.kuanghao11.cn

Py:   os.environ.get("HOME")
来源：http://qsp.pengpengdd.cyou

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://awh.sufxvd.cn

JS:   process.env.HOME
来源：http://pip.hongshengwenyu.top

TS:   process.env.HOME
来源：http://tdb.ydzc1.top

Java: System.getenv("HOME")
来源：http://ssp.yj20258.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://qzs.zycfv.cn

Ruby: ENV["HOME"]
来源：http://sye.xziqi.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://rfm.chenlongwang.top

[M03] 执行外部命令
来源：http://jxx.cucudq.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://pgm.pycfn.com

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://gnn.jiagoushi.top

JS:   child_process.execSync("ls -l").toString()
来源：http://rvm.guannengcc.top

TS:   child_process.execSync("ls -l").toString()
来源：http://teg.hfpthk.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ohe.redwolf501.top

Go:   exec.Command("ls", "-l").Output()
来源：http://edc.yj20258888.top

Ruby: system("ls -l");  `ls -l`
来源：http://tuh.kuanghao11.cn

C#:   Process.Start("ls", "-l");
来源：http://uxb.wangshuangyany.cn

[M04] 获取当前工作目录
来源：http://kfq.redwolf501.top

Py:   os.getcwd()
来源：http://yri.gotoacloud.top

PHP:  getcwd();
来源：http://qjx.tanke756.top

JS:   process.cwd()
来源：http://vud.sufxvd.cn

TS:   process.cwd()
来源：http://uig.sweek.top

Java: Path.of("").toAbsolutePath()
来源：http://mzr.jyoumei.cn

Go:   os.Getwd()
来源：http://kna.zhixingplan.top

Ruby: Dir.pwd
来源：http://oqg.yfazqb.com

C#:   Directory.GetCurrentDirectory()
来源：http://jju.zhaomingkeji.xyz

[M05] 设置退出码
来源：http://gxw.gzhubu.top

Py:   sys.exit(1)
来源：http://azv.zhongyouzk.top

PHP:  exit(1);
来源：http://rux.52xcode.cn

JS:   process.exit(1)
来源：http://tjb.hnqzz.top

TS:   process.exit(1)
来源：http://ixs.dianchejie.cn

Java: System.exit(1)
来源：http://rfl.shanyushiyangkeji.top

Go:   os.Exit(1)
来源：http://mlu.mhx1999.top

Ruby: exit 1
来源：http://edu.birdmap.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://zjf.shangyingyoupin.top

[M06] 向标准错误输出
来源：http://aub.0kj1m.cn

Py:   print("err", file=sys.stderr)
来源：http://vom.yongpay.top

PHP:  fwrite(STDERR, "err\n");
来源：http://ohk.yuxming.cn

JS:   console.error("err")
来源：http://uqk.meibo888.top

TS:   console.error("err")
来源：http://jfv.gogol.net.cn

Java: System.err.println("err")
来源：http://lhn.gaohongyu789.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://nfn.hcnkem.com

Ruby: warn "err"
来源：http://jah.c1oappe.top

C#:   Console.Error.WriteLine("err")
来源：http://eih.zhongyouzk.top

[M07] 判断是否为主入口
来源：http://tjw.cqqwz.cn

Py:   if __name__ == "__main__":
来源：http://biy.zhixingplan.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://qpt.wangshuangyany.cn

JS:   require.main === module
来源：http://mui.ctjpmb.com

TS:   require.main === module
来源：http://vhm.aibaodan.cn

Java: public static void main(String[] args)
来源：http://lxi.chenzaomai.com

Go:   func main()
来源：http://rwb.vehdjk.com

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://aqj.wangshuangyany.cn

C#:   static void Main(string[] args)
来源：http://sdj.ydjk.org.cn

[M08] 获取系统与运行时信息
来源：http://uqk.shuidangran.top

Py:   platform.system();  platform.python_version()
来源：http://fzl.jinghuilouyu.cn

PHP:  PHP_OS;  phpversion();
来源：http://tkk.sysykeji.top

JS:   process.platform;  process.version
来源：http://mex.zycfv.cn

TS:   process.platform;  process.version
来源：http://vhr.jinqigfzy.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://eib.sufxvd.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://rdq.hcnkem.com

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://kyy.gotoacloud.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://ukj.sweek.top

================================================================================
来源：http://nkc.zhiwuduotai.top

N. 数据结构与算法
来源：http://oig.birdmap.top

================================================================================
来源：http://vjs.ybcxt.top

[N01] 二分查找（有序数组）
来源：http://fey.fktsv.cn

Py:   bisect.bisect_left(arr, x)
来源：http://yzw.ctjpmb.com

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ldr.yfazqb.com

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://zfm.52xcode.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://vus.xinyue.icu

Java: Arrays.binarySearch(arr, x)
来源：http://tgw.sxryk.cn

Go:   sort.SearchInts(arr, x)
来源：http://ebf.gzhubu.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://bkg.yueranfly.top

C#:   Array.BinarySearch(arr, x)
来源：http://jzd.zhiwuduotai.top

[N02] 排序（工程实践用内置实现）
来源：http://nhe.snrcjt.cn

Py:   sorted(arr);  arr.sort()
来源：http://bpp.yj202588.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://acw.zhiwuduotai.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://isl.smart0.xyz

TS:   [...arr].sort((a, b) => a - b)
来源：http://hpj.ivvv.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://asp.cqqwz.cn

Go:   slices.Sort(arr)
来源：http://gjx.fktsv.cn

Ruby: arr.sort
来源：http://chn.sxryk.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://qzg.hysaishi.cn

[N03] 快速排序（分治示例）
来源：http://wdk.andypj.xyz

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://oqu.nwbrower.top

PHP:  // 递归实现，或用 usort
来源：http://rnp.zhongyouzk.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ddm.c1oappe.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://yep.cqqwz.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://zns.snrcjt.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://xov.ydjk.org.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://rvn.jiagoushi.top

C#:   // 手写递归，或 Array.Sort
来源：http://iwf.yonumen.top

[N04] 斐波那契数列
来源：http://gax.quarkkingdee.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://evj.yuanzhike.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://tlo.kuanghao11.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://qgd.ydjk.org.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://qtz.svipenyu.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ahe.mhx1999.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ggm.fanxiaobao.xyz

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://oao.jinqigufen.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mvr.redwolf501.top

[N05] 最大公约数
来源：http://vda.yj20258888.top

Py:   math.gcd(a, b)
来源：http://oni.smart0.xyz

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://msy.yangfankeji.com

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hyj.shuidangran.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://jyc.havefunace.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://prm.snrcjt.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://knm.iojbl.cn

Ruby: a.gcd(b)
来源：http://irs.andypj.xyz

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://oam.iojbl.cn

[N06] 判断回文字符串
来源：http://eer.hongshengwenyu.top

Py:   s == s[::-1]
来源：http://ejk.tarul.cn

PHP:  $s === strrev($s);
来源：http://qej.fehbvm.com

JS:   s === [...s].reverse().join("")
来源：http://aob.jlsjyb.cn

TS:   s === [...s].reverse().join("")
来源：http://irm.zhongyouzk.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://aqt.bbcook.cn

Go:   // 双指针从两端比较
来源：http://ylq.redwolf501.top

Ruby: s == s.reverse
来源：http://mqc.hnqzz.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://rmw.jyoumei.cn

[N07] 两数之和（返回下标）
来源：http://cnz.jlsjyb.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://oeg.uphjek.com

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://rad.bjfxy.top

JS:   // 手写 Map：map.set(v, i)
来源：http://oan.hnxiangtu.top

TS:   // 手写 Map<string, number>
来源：http://hxu.cucudq.cn

Java: // 手写 HashMap
来源：http://mcb.hnqzz.top

Go:   // 手写 map[int]int
来源：http://kox.sysykeji.top

Ruby: // 手写 Hash
来源：http://uuk.andypj.xyz

C#:   // 手写 Dictionary<int, int>
来源：http://zum.shanyushiyangkeji.top

[N08] 生成全排列
来源：http://avq.pycfn.com

Py:   itertools.permutations(arr)
来源：http://mqs.cucudq.cn

PHP:  // 手写递归交换
来源：http://zit.redwolf501.top

JS:   // 手写回溯递归
来源：http://ugn.yueranfly.top

TS:   // 手写回溯递归
来源：http://uei.daxiang520.top

Java: // 手写回溯递归
来源：http://hgo.xylfe.cn

Go:   // 手写回溯递归
来源：http://evi.aibaodan.cn

Ruby: arr.permutation.to_a
来源：http://vbx.jianghu66.top

C#:   // 手写回溯递归
来源：http://cme.chenlongwang.top

[N09] 栈与队列
来源：http://yeu.hnxiangtu.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://erc.cashguo.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://yjl.xinyue.icu

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://xmi.fehbvm.com

TS:   arr.push(x) / arr.pop() 作栈
来源：http://qoq.jqgfzy.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://qwv.fengsongda.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://nei.cashguo.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://lit.jinqigfzy.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://vla.tianlin.xyz

[N10] 链表节点定义
来源：http://dou.316326.xyz

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://xxt.yongpay.top

PHP:  class Node { public $v; public $next = null; }
来源：http://xzi.ydjk.org.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://eip.shanyushiyangtech.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://iqn.sjlbkw.cn

Java: class Node { int v; Node next; }
来源：http://ihs.hnqzz.top

Go:   type Node struct { V int; Next *Node }
来源：http://slj.pengpengdd.cyou

Ruby: Node = Struct.new(:v, :next)
来源：http://kbg.ctjpmb.com

C#:   class Node { public int V; public Node? Next; }
来源：http://mzi.chenlongwang.top

[N11] 二叉树中序遍历
来源：http://dua.gaohongyu789.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://vpy.nwbrower.top

PHP:  // 手写递归函数
来源：http://bby.ppjwa.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://kcs.uphjek.com

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://gsq.yj202588.top

Java: // 手写递归
来源：http://mup.fengsongda.top

Go:   // 手写递归
来源：http://ahr.xingfuxueyuan.xyz

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mfr.jinghuilouyu.cn

C#:   // 手写递归
来源：http://arp.xingfuxueyuan.xyz

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://bsc.kuanghao11.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://nnl.jinqigfzy.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://zdm.xingfuxueyuan.xyz

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ikl.hnqzz.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://lpi.gotoacloud.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://koz.gogol.net.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wsc.dashuyun.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://dcf.svipenyu.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mti.tian-w.cn

================================================================================
来源：http://mjy.jqgfzy.top

O. 并发与异步
来源：http://jrx.daria6918.cn

================================================================================
来源：http://jca.fengsongda.top

[O01] 启动一个线程
来源：http://dgk.zycfv.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://lpd.gotoacloud.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mxg.snrcjt.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://svi.tianlin.xyz

TS:   // 同 JS
来源：http://rvf.jlsjyb.cn

Java: new Thread(() -> f()).start()
来源：http://pyp.tian-w.cn

Go:   go f()
来源：http://mef.cashguo.top

Ruby: Thread.new { f }
来源：http://fab.sweek.top

C#:   Task.Run(() => F());
来源：http://slc.yfazqb.com

[O02] 使用线程池
来源：http://fml.guowangkeji.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://lxf.svipenyu.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://nix.dashuyun.cn

JS:   // worker_threads 线程池
来源：http://urn.tanke756.top

TS:   // worker_threads 线程池
来源：http://tmt.bjfxy.top

Java: Executors.newFixedThreadPool(4)
来源：http://vfx.jianghu66.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://bav.52xcode.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://qtn.yueranfly.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://exq.gzhubu.top

[O03] 加锁保护共享数据
来源：http://nsk.tanke756.top

Py:   with lock: shared += 1
来源：http://sms.yfazqb.com

PHP:  // 用 flock() 做文件锁
来源：http://oic.bjfxy.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ott.hywenlv.cn

TS:   // 同 JS
来源：http://xlm.smart0.xyz

Java: synchronized (this) { shared++; }
来源：http://jqt.chenzaomai.com

Go:   mu.Lock();  defer mu.Unlock()
来源：http://lbu.guowangkeji.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://qqs.hysaishi.cn

C#:   lock (gate) { shared++; }
来源：http://rwz.yfazqb.com

[O04] 定义异步函数并等待
来源：http://noe.dianchejie.cn

Py:   async def f():⏎    await g()
来源：http://qpm.sufxvd.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ytz.vqdsnc.cn

JS:   async function f() { await g(); }
来源：http://xgf.9152youxi.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://xtb.jinqigufen.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://rbu.0kj1m.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://pjy.jqgfzy.top

Ruby: # 用 Fiber 或 async gem
来源：http://als.gotoacloud.top

C#:   async Task F() { await G(); }
来源：http://awk.zhijiandao.cn

[O05] 并发执行并等待全部完成
来源：http://nna.zhongyouzk.top

Py:   asyncio.gather(*tasks)
来源：http://bko.ybcxt.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://xej.jlsjyb.cn

JS:   await Promise.all(tasks)
来源：http://tfv.cheryme.top

TS:   await Promise.all(tasks)
来源：http://avx.fanxiaobao.xyz

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://xkp.c1oappe.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ndt.vehdjk.com

Ruby: threads.map(&:join)
来源：http://gmm.xylfe.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://hxk.yanxiufei.cn

[O06] 使用进程池
来源：http://hfy.uphjek.com

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://uue.svipenyu.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://wrc.c1oappe.top

JS:   // child_process / cluster 模块
来源：http://joc.guannengcc.top

TS:   // child_process / cluster 模块
来源：http://leg.dashuyun.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://njb.bbcook.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ghn.ydzc1.top

Ruby: // fork 块
来源：http://icd.yueranfly.top

C#:   Parallel.For
来源：http://xyd.ivvv.top

================================================================================
来源：http://oym.wangshuangyany.cn

P. 常用工具函数
来源：http://pkh.316326.xyz

================================================================================
来源：http://mwz.jianghu66.top

[P01] 生成 UUID
来源：http://pna.gogol.net.cn

Py:   str(uuid.uuid4())
来源：http://xyw.nanxuanxn.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://kgx.havefunace.top

JS:   crypto.randomUUID()
来源：http://wfc.ppjwa.cn

TS:   crypto.randomUUID()
来源：http://yfu.jinghuilouyu.cn

Java: UUID.randomUUID().toString()
来源：http://itq.bjfxy.top

Go:   // 用 github.com/google/uuid
来源：http://uoy.zhengqikj.top

Ruby: SecureRandom.uuid
来源：http://ktp.aibaodan.cn


<!-- 参考信息 -->