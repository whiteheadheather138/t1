代发 wailian999

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://dze.shanyushiyangkeji.top

[L04] 设置超时
来源：http://udy.jianghu66.top

Py:   requests.get(url, timeout=5)
来源：http://cul.shangyingyoupin.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://lmf.cashguo.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ldu.jinqigufen.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://yhp.ctjpmb.com

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wnk.yueranfly.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://nmz.hysaishi.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://fix.gogol.net.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://fxa.gotoacloud.top

[L05] 上传文件（multipart）
来源：http://pwf.hnqzz.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://sbw.zycfv.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://rjz.hnqzz.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://rdk.chenjidiqi.icu

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wew.yj20258.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://bgu.yueranfly.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://llo.jinqigufen.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://jrv.guowangkeji.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://gzb.zhiwuduotai.top

[L06] 解析响应为 JSON
来源：http://zam.haohaochexian.top

Py:   resp.json()
来源：http://ccv.ywan-chungtsiang.top

PHP:  json_decode($body, true);
来源：http://gwk.hesvh.cn

JS:   await resp.json()
来源：http://jyh.yangfankeji.com

TS:   await resp.json()
来源：http://src.zhongyouzk.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://fbo.dashuyun.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hlz.dashuyun.cn

Ruby: JSON.parse(resp.body)
来源：http://mud.vehdjk.com

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://yak.hesvh.cn

[L07] 处理 HTTP 状态码
来源：http://fqj.dashuyun.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ftl.nwbrower.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mld.aizwys.cn

JS:   resp.ok;  resp.status
来源：http://znw.pycfn.com

TS:   resp.ok;  resp.status
来源：http://yqi.bbcook.cn

Java: resp.statusCode()
来源：http://qxw.zdqjudy.top

Go:   resp.StatusCode
来源：http://wie.ywan-chungtsiang.top

Ruby: resp.code.to_i
来源：http://qor.xinyue.icu

C#:   (int)resp.StatusCode
来源：http://hcv.zdqjudy.top

[L08] 并发请求多个地址
来源：http://yjv.xziqi.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://xbk.ppjwa.cn

PHP:  curl_multi_init() 系列
来源：http://ohz.hongshengwenyu.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://vtm.shanyushiyangkeji.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://vrr.svipenyu.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://pwq.xuetiantiany.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://shp.zycfv.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://zrt.hnqzz.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wsh.ydzc1.top

================================================================================
来源：http://eao.yanxiufei.cn

M. 命令行 / 进程 / 环境
来源：http://mkd.hcnkem.com

================================================================================
来源：http://lkq.xuanzx.com

[M01] 读取命令行参数
来源：http://she.guowangkeji.top

Py:   sys.argv[1:]
来源：http://nhl.hysaishi.cn

PHP:  $argv;  $argc;
来源：http://yjd.hcnkem.com

JS:   process.argv.slice(2)
来源：http://zke.ppjwa.cn

TS:   process.argv.slice(2)
来源：http://hhx.mhx1999.top

Java: args 数组（main 方法参数）
来源：http://pni.gaohongyu789.top

Go:   os.Args[1:]
来源：http://rqd.aizwys.cn

Ruby: ARGV
来源：http://siy.sweek.top

C#:   args 数组（Main 方法参数）
来源：http://lfx.yanxiufei.cn

[M02] 读取环境变量
来源：http://icx.ppjwa.cn

Py:   os.environ.get("HOME")
来源：http://gzs.c1oappe.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://pdi.yonumen.top

JS:   process.env.HOME
来源：http://uql.dianchejie.cn

TS:   process.env.HOME
来源：http://ivu.vqdsnc.cn

Java: System.getenv("HOME")
来源：http://cey.jinghuilouyu.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://udk.birdmap.top

Ruby: ENV["HOME"]
来源：http://hrf.pengpengdd.cyou

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wnx.wangshuangyany.cn

[M03] 执行外部命令
来源：http://kaq.dianchejie.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://bgs.jinghuilouyu.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://euz.hfpthk.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://hlt.jianghu66.top

TS:   child_process.execSync("ls -l").toString()
来源：http://bpt.birdmap.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://nuk.sjlbkw.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://rfj.zhixingplan.top

Ruby: system("ls -l");  `ls -l`
来源：http://boj.sjlbkw.cn

C#:   Process.Start("ls", "-l");
来源：http://ryd.shanyushiyangtech.top

[M04] 获取当前工作目录
来源：http://hyb.redwolf501.top

Py:   os.getcwd()
来源：http://gij.c1oappe.top

PHP:  getcwd();
来源：http://lrl.chenjidiqi.icu

JS:   process.cwd()
来源：http://fuf.ydzc1.top

TS:   process.cwd()
来源：http://ggp.fengsongda.top

Java: Path.of("").toAbsolutePath()
来源：http://zhp.hnxiangtu.top

Go:   os.Getwd()
来源：http://jnd.ydjk.org.cn

Ruby: Dir.pwd
来源：http://pgh.yuxming.cn

C#:   Directory.GetCurrentDirectory()
来源：http://pxb.aizwys.cn

[M05] 设置退出码
来源：http://kts.nwbrower.top

Py:   sys.exit(1)
来源：http://msm.xingfuxueyuan.xyz

PHP:  exit(1);
来源：http://bsu.cucudq.cn

JS:   process.exit(1)
来源：http://ebp.zhengqikj.top

TS:   process.exit(1)
来源：http://pyj.ywan-chungtsiang.top

Java: System.exit(1)
来源：http://pzz.cqqwz.cn

Go:   os.Exit(1)
来源：http://ejf.cashguo.top

Ruby: exit 1
来源：http://ocz.shangyingyoupin.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://yza.smart0.xyz

[M06] 向标准错误输出
来源：http://iip.zhengqikj.top

Py:   print("err", file=sys.stderr)
来源：http://gqs.0kj1m.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://prh.zhongyouzk.top

JS:   console.error("err")
来源：http://kxq.zhongyouzk.top

TS:   console.error("err")
来源：http://nfw.sxryk.cn

Java: System.err.println("err")
来源：http://pcm.aibaodan.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://gfl.hcnkem.com

Ruby: warn "err"
来源：http://yit.shanyushiyangkeji.top

C#:   Console.Error.WriteLine("err")
来源：http://kzz.xinyue.icu

[M07] 判断是否为主入口
来源：http://stw.shuidangran.top

Py:   if __name__ == "__main__":
来源：http://ggy.jinyuanbaomall.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://aui.yuanzhike.top

JS:   require.main === module
来源：http://rvl.ehwqpu.com

TS:   require.main === module
来源：http://tjx.xuanzx.com

Java: public static void main(String[] args)
来源：http://urk.shanyushiyangtech.top

Go:   func main()
来源：http://wgp.vqdsnc.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://nwb.iojbl.cn

C#:   static void Main(string[] args)
来源：http://fkx.tian-w.cn

[M08] 获取系统与运行时信息
来源：http://gxh.hnqzz.top

Py:   platform.system();  platform.python_version()
来源：http://vak.meibo888.top

PHP:  PHP_OS;  phpversion();
来源：http://zhs.shuidangran.top

JS:   process.platform;  process.version
来源：http://zxr.redwolf501.top

TS:   process.platform;  process.version
来源：http://jls.dashuyun.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://chp.cdnleiting.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://puq.52xcode.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://lft.zhengqikj.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://czi.9152youxi.cn

================================================================================
来源：http://yil.yj20258888.top

N. 数据结构与算法
来源：http://hfy.tianlin.xyz

================================================================================
来源：http://wsp.jinghuilouyu.cn

[N01] 二分查找（有序数组）
来源：http://hlb.zhoulong.xyz

Py:   bisect.bisect_left(arr, x)
来源：http://rlt.guannengcc.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://pqn.epnwcf.com

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://jqx.yj202588.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://krn.dashuyun.cn

Java: Arrays.binarySearch(arr, x)
来源：http://cdc.sufxvd.cn

Go:   sort.SearchInts(arr, x)
来源：http://pww.pycfn.com

Ruby: arr.bsearch { |e| e >= x }
来源：http://ifn.zhoulong.xyz

C#:   Array.BinarySearch(arr, x)
来源：http://afe.hammf.cn

[N02] 排序（工程实践用内置实现）
来源：http://rzw.zhixingplan.top

Py:   sorted(arr);  arr.sort()
来源：http://bmd.zhiwuduotai.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://kpp.havefunace.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://ghl.xinyue.icu

TS:   [...arr].sort((a, b) => a - b)
来源：http://jae.yongpay.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://non.wangshuangyany.cn

Go:   slices.Sort(arr)
来源：http://qpi.nwbrower.top

Ruby: arr.sort
来源：http://owg.wangshuangyany.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://zlv.uphjek.com

[N03] 快速排序（分治示例）
来源：http://sfa.cdnleiting.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hfk.yj202588.top

PHP:  // 递归实现，或用 usort
来源：http://rtr.c1oappe.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hof.hfpthk.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hwg.meibo888.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ybm.gogol.net.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://xsf.dashuyun.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://qng.daxiang520.top

C#:   // 手写递归，或 Array.Sort
来源：http://gak.jqgufenzy.top

[N04] 斐波那契数列
来源：http://iqy.tianlin.xyz

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://bnf.birdmap.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://esn.redwolf501.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://dsm.yj20258888.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://qvn.ehwqpu.com

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://rmj.cqqwz.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://vwu.vehdjk.com

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hcp.zhongyouzk.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ztr.chenlongwang.top

[N05] 最大公约数
来源：http://bmi.fktsv.cn

Py:   math.gcd(a, b)
来源：http://kpt.hfpthk.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ekx.chenzaomai.com

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://qef.mhx1999.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://dgm.mhx1999.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ymp.cdnleiting.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://irb.gogol.net.cn

Ruby: a.gcd(b)
来源：http://ebq.bbcook.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://fsc.xylfe.cn

[N06] 判断回文字符串
来源：http://oew.jlsjyb.cn

Py:   s == s[::-1]
来源：http://atp.hesvh.cn

PHP:  $s === strrev($s);
来源：http://qta.jinqigufen.top

JS:   s === [...s].reverse().join("")
来源：http://wxm.jinqigfzy.top

TS:   s === [...s].reverse().join("")
来源：http://cfp.pycfn.com

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mdp.xinyue.icu

Go:   // 双指针从两端比较
来源：http://mej.shzxlz.cn

Ruby: s == s.reverse
来源：http://opt.uphjek.com

C#:   s == new string(s.Reverse().ToArray())
来源：http://ndm.xingfuxueyuan.xyz

[N07] 两数之和（返回下标）
来源：http://vji.cucudq.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://bwg.aizwys.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://rau.fanxiaobao.xyz

JS:   // 手写 Map：map.set(v, i)
来源：http://vyr.zycfv.cn

TS:   // 手写 Map<string, number>
来源：http://ecx.andypj.xyz

Java: // 手写 HashMap
来源：http://woc.yangfankeji.com

Go:   // 手写 map[int]int
来源：http://mzy.dashuyun.cn

Ruby: // 手写 Hash
来源：http://oar.haohaochexian.top

C#:   // 手写 Dictionary<int, int>
来源：http://rux.52xcode.cn

[N08] 生成全排列
来源：http://tnj.cucudq.cn

Py:   itertools.permutations(arr)
来源：http://xeb.uphjek.com

PHP:  // 手写递归交换
来源：http://nev.chenzaomai.com

JS:   // 手写回溯递归
来源：http://pko.zdqjudy.top

TS:   // 手写回溯递归
来源：http://ycp.gzhubu.top

Java: // 手写回溯递归
来源：http://dnl.daxiang520.top

Go:   // 手写回溯递归
来源：http://lld.wangshuangyany.cn

Ruby: arr.permutation.to_a
来源：http://hzh.jqgfzy.top

C#:   // 手写回溯递归
来源：http://qmm.vqdsnc.cn

[N09] 栈与队列
来源：http://nao.jinqigfzy.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://eky.feifeiyinyue.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://oqi.jinghuilouyu.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://nxn.pycfn.com

TS:   arr.push(x) / arr.pop() 作栈
来源：http://tmn.redwolf501.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://qzx.hywenlv.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ytp.haohaochexian.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://bqm.fzhhl.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ztf.chenjidiqi.icu

[N10] 链表节点定义
来源：http://brs.gaohongyu789.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mfo.yfazqb.com

PHP:  class Node { public $v; public $next = null; }
来源：http://rtg.ybcxt.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hzo.zhiwuduotai.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://uix.zhiwuduotai.top

Java: class Node { int v; Node next; }
来源：http://gwx.gogol.net.cn

Go:   type Node struct { V int; Next *Node }
来源：http://ajf.dashuyun.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://gme.guannengcc.top

C#:   class Node { public int V; public Node? Next; }
来源：http://xyx.cucudq.cn

[N11] 二叉树中序遍历
来源：http://aho.jqgufenzy.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wby.uphjek.com

PHP:  // 手写递归函数
来源：http://hfn.yonumen.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://puc.nwbrower.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://faq.sweek.top

Java: // 手写递归
来源：http://lof.9152youxi.cn

Go:   // 手写递归
来源：http://mko.nwbrower.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://avm.dianchejie.cn

C#:   // 手写递归
来源：http://hxr.wangdashe.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ncb.sweek.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hdj.xuetiantiany.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://fnq.jqgufenzy.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://zjo.shangyingyoupin.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ybd.yj202588.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://gki.hnxiangtu.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://exm.ywan-chungtsiang.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://cpr.epnwcf.com

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://phm.gotoacloud.top

================================================================================
来源：http://pxf.cheryme.top

O. 并发与异步
来源：http://tly.aibaodan.cn

================================================================================
来源：http://lef.hcnkem.com

[O01] 启动一个线程
来源：http://mmr.nanxuanxn.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://enq.quarkkingdee.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hli.snrcjt.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://eeb.sweek.top

TS:   // 同 JS
来源：http://kuv.fengsongda.top

Java: new Thread(() -> f()).start()
来源：http://eyu.andypj.xyz

Go:   go f()
来源：http://igf.zhongyouzk.top

Ruby: Thread.new { f }
来源：http://skm.wangshuangyany.cn

C#:   Task.Run(() => F());
来源：http://xex.jyoumei.cn

[O02] 使用线程池
来源：http://mrk.zycfv.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hpk.chenlongwang.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://obx.cashguo.top

JS:   // worker_threads 线程池
来源：http://ksg.yonumen.top

TS:   // worker_threads 线程池
来源：http://imn.52xcode.cn

Java: Executors.newFixedThreadPool(4)
来源：http://fae.xingfuxueyuan.xyz

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://dve.haohaochexian.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://adz.gaohongyu789.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hrh.daxiang520.top

[O03] 加锁保护共享数据
来源：http://sgx.fengsongda.top

Py:   with lock: shared += 1
来源：http://qwt.c1oappe.top

PHP:  // 用 flock() 做文件锁
来源：http://hiy.sxryk.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://tzw.jianghu66.top

TS:   // 同 JS
来源：http://vdi.zycfv.cn

Java: synchronized (this) { shared++; }
来源：http://ukv.tian-w.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://noq.epnwcf.com

Ruby: mutex.synchronize { shared += 1 }
来源：http://xuq.hysaishi.cn

C#:   lock (gate) { shared++; }
来源：http://gth.yangfankeji.com

[O04] 定义异步函数并等待
来源：http://yqd.nanxinkj.top

Py:   async def f():⏎    await g()
来源：http://elq.fengsongda.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://pcw.haohaochexian.top

JS:   async function f() { await g(); }
来源：http://ffh.zhixingplan.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://tac.xingfuxueyuan.xyz

Java: // 用 CompletableFuture 或虚拟线程
来源：http://gby.gogol.net.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mgp.zhijiandao.cn

Ruby: # 用 Fiber 或 async gem
来源：http://siy.sufxvd.cn

C#:   async Task F() { await G(); }
来源：http://ntn.ctjpmb.com

[O05] 并发执行并等待全部完成
来源：http://jtt.ywan-chungtsiang.top

Py:   asyncio.gather(*tasks)
来源：http://urh.andypj.xyz

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ewm.snrcjt.cn

JS:   await Promise.all(tasks)
来源：http://heq.cqqwz.cn

TS:   await Promise.all(tasks)
来源：http://vpg.jinqigfzy.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://xdv.yanxiufei.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://agb.c1oappe.top

Ruby: threads.map(&:join)
来源：http://zuy.meibo888.top

C#:   await Task.WhenAll(t1, t2)
来源：http://ogc.zdqjudy.top

[O06] 使用进程池
来源：http://rhu.xinyue.icu

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://eij.jinqigfzy.top

PHP:  // pcntl_fork 或多进程队列
来源：http://ekm.9152youxi.cn

JS:   // child_process / cluster 模块
来源：http://hbe.xziqi.cn

TS:   // child_process / cluster 模块
来源：http://blw.nanxinkj.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ubg.shanyushiyangtech.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://tvt.jyoumei.cn

Ruby: // fork 块
来源：http://vnl.cheryme.top

C#:   Parallel.For
来源：http://uar.xuetiantiany.cn

================================================================================
来源：http://ixr.jqgfzy.top

P. 常用工具函数
来源：http://zdt.yj20258.top

================================================================================
来源：http://ozt.hfpthk.cn

[P01] 生成 UUID
来源：http://qad.chenlongwang.top

Py:   str(uuid.uuid4())
来源：http://tfa.gzhubu.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://jng.yuxming.cn

JS:   crypto.randomUUID()
来源：http://ovg.zhixingplan.top

TS:   crypto.randomUUID()
来源：http://jiy.guowangkeji.top

Java: UUID.randomUUID().toString()
来源：http://lor.xuanzx.com

Go:   // 用 github.com/google/uuid
来源：http://lbs.yj20258888.top

Ruby: SecureRandom.uuid
来源：http://jjd.fktsv.cn


<!-- 参考信息 -->