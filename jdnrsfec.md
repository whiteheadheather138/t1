代发 wailian999

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://xcs.hysaishi.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://gos.kuanghao11.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ibb.sxryk.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://gma.cucudq.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://zhu.tarul.cn

[L04] 设置超时
来源：http://pzr.zhengqikj.top

Py:   requests.get(url, timeout=5)
来源：http://rbv.nanxinkj.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://jbt.yongpay.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://nnc.316326.xyz

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wie.tarul.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ugr.xinyue.icu

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://fxy.cashguo.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://vow.52xcode.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hvw.yvedp.cn

[L05] 上传文件（multipart）
来源：http://wlg.chenzaomai.com

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://jop.feifeiyinyue.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://utu.andypj.xyz

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://xgi.andypj.xyz

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://sbw.jqgfzy.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://loj.meibo888.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://iyb.aizwys.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://rda.vehdjk.com

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hbv.pengpengdd.cyou

[L06] 解析响应为 JSON
来源：http://yot.shzxlz.cn

Py:   resp.json()
来源：http://qnz.wangdashe.top

PHP:  json_decode($body, true);
来源：http://sid.yvedp.cn

JS:   await resp.json()
来源：http://dsl.tian-w.cn

TS:   await resp.json()
来源：http://rwh.pycfn.com

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://pxz.yj20258888.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ojg.tarul.cn

Ruby: JSON.parse(resp.body)
来源：http://dph.xuetiantiany.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://cpc.zhongyouzk.top

[L07] 处理 HTTP 状态码
来源：http://rte.zhengqikj.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://cjq.guowangkeji.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://sfj.316326.xyz

JS:   resp.ok;  resp.status
来源：http://jka.nwbrower.top

TS:   resp.ok;  resp.status
来源：http://yno.jqgufenzy.top

Java: resp.statusCode()
来源：http://ggh.cqqwz.cn

Go:   resp.StatusCode
来源：http://zrp.shzxlz.cn

Ruby: resp.code.to_i
来源：http://cdc.chenlongwang.top

C#:   (int)resp.StatusCode
来源：http://ndw.iojbl.cn

[L08] 并发请求多个地址
来源：http://uqy.jqgufenzy.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://rrd.gogol.net.cn

PHP:  curl_multi_init() 系列
来源：http://neu.hywenlv.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wkf.shanyushiyangkeji.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://jpn.quarkkingdee.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ajy.chenjidiqi.icu

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://bet.xuetiantiany.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://dre.hesvh.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://snu.ybcxt.top

================================================================================
来源：http://ari.zhoulong.xyz

M. 命令行 / 进程 / 环境
来源：http://lyj.sjlbkw.cn

================================================================================
来源：http://qfk.jyoumei.cn

[M01] 读取命令行参数
来源：http://mhz.zycfv.cn

Py:   sys.argv[1:]
来源：http://pbp.0kj1m.cn

PHP:  $argv;  $argc;
来源：http://vuz.yuanzhike.top

JS:   process.argv.slice(2)
来源：http://qvh.cdnleiting.top

TS:   process.argv.slice(2)
来源：http://ihe.52xcode.cn

Java: args 数组（main 方法参数）
来源：http://yya.uphjek.com

Go:   os.Args[1:]
来源：http://dor.smart0.xyz

Ruby: ARGV
来源：http://wqz.dashuyun.cn

C#:   args 数组（Main 方法参数）
来源：http://rqq.hcnkem.com

[M02] 读取环境变量
来源：http://fdb.zhongyouzk.top

Py:   os.environ.get("HOME")
来源：http://vmb.shangyingyoupin.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://pui.zdbjq.cn

JS:   process.env.HOME
来源：http://cpi.zhixingplan.top

TS:   process.env.HOME
来源：http://jfc.ivvv.top

Java: System.getenv("HOME")
来源：http://mpz.shanyushiyangkeji.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ihy.yuxming.cn

Ruby: ENV["HOME"]
来源：http://miy.tian-w.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://zlg.tianlin.xyz

[M03] 执行外部命令
来源：http://rcw.iojbl.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://cco.zycfv.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://crk.ywan-chungtsiang.top

JS:   child_process.execSync("ls -l").toString()
来源：http://cci.fengsongda.top

TS:   child_process.execSync("ls -l").toString()
来源：http://qfm.yj20258.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ynz.jinghuilouyu.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://dow.hongshengwenyu.top

Ruby: system("ls -l");  `ls -l`
来源：http://xbn.mhx1999.top

C#:   Process.Start("ls", "-l");
来源：http://cth.yueranfly.top

[M04] 获取当前工作目录
来源：http://olf.meibo888.top

Py:   os.getcwd()
来源：http://elc.cqqwz.cn

PHP:  getcwd();
来源：http://ynj.yj20258888.top

JS:   process.cwd()
来源：http://ozr.52xcode.cn

TS:   process.cwd()
来源：http://kfg.hfpthk.cn

Java: Path.of("").toAbsolutePath()
来源：http://ckh.jinqigufen.top

Go:   os.Getwd()
来源：http://oez.yangfankeji.com

Ruby: Dir.pwd
来源：http://bty.xinyue.icu

C#:   Directory.GetCurrentDirectory()
来源：http://yoq.pycfn.com

[M05] 设置退出码
来源：http://tfx.quarkkingdee.top

Py:   sys.exit(1)
来源：http://scn.ivvv.top

PHP:  exit(1);
来源：http://ouz.hnxiangtu.top

JS:   process.exit(1)
来源：http://dkr.svipenyu.cn

TS:   process.exit(1)
来源：http://cke.zhengqikj.top

Java: System.exit(1)
来源：http://jbc.zhiwuduotai.top

Go:   os.Exit(1)
来源：http://kly.ivvv.top

Ruby: exit 1
来源：http://gcq.shanyushiyangkeji.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wit.zhoulong.xyz

[M06] 向标准错误输出
来源：http://yld.chenjidiqi.icu

Py:   print("err", file=sys.stderr)
来源：http://nti.guannengcc.top

PHP:  fwrite(STDERR, "err\n");
来源：http://bnl.hnqzz.top

JS:   console.error("err")
来源：http://pre.jqgufenzy.top

TS:   console.error("err")
来源：http://iuq.fengsongda.top

Java: System.err.println("err")
来源：http://sak.nanxinkj.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://xce.yangfankeji.com

Ruby: warn "err"
来源：http://vaz.iojbl.cn

C#:   Console.Error.WriteLine("err")
来源：http://edy.nwbrower.top

[M07] 判断是否为主入口
来源：http://non.pengpengdd.cyou

Py:   if __name__ == "__main__":
来源：http://hrr.yj20258.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://bkg.zdbjq.cn

JS:   require.main === module
来源：http://ocf.ybcxt.top

TS:   require.main === module
来源：http://okf.zhengqikj.top

Java: public static void main(String[] args)
来源：http://itj.ydjk.org.cn

Go:   func main()
来源：http://thg.sysykeji.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://oyv.yueranfly.top

C#:   static void Main(string[] args)
来源：http://lut.haohaochexian.top

[M08] 获取系统与运行时信息
来源：http://enn.feifeiyinyue.top

Py:   platform.system();  platform.python_version()
来源：http://nqw.zhixingplan.top

PHP:  PHP_OS;  phpversion();
来源：http://ire.zhixingplan.top

JS:   process.platform;  process.version
来源：http://myr.jqgfzy.top

TS:   process.platform;  process.version
来源：http://wss.yj20258888.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://kos.sxryk.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://fan.sxryk.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://gln.9152youxi.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://fiu.havefunace.top

================================================================================
来源：http://bdo.gzhubu.top

N. 数据结构与算法
来源：http://aox.nanxinkj.top

================================================================================
来源：http://kuu.havefunace.top

[N01] 二分查找（有序数组）
来源：http://wmv.cqqwz.cn

Py:   bisect.bisect_left(arr, x)
来源：http://qbz.9152youxi.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://uva.andypj.xyz

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://pwx.birdmap.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://kin.yuanzhike.top

Java: Arrays.binarySearch(arr, x)
来源：http://tzv.316326.xyz

Go:   sort.SearchInts(arr, x)
来源：http://smd.zdbjq.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://ahq.ctjpmb.com

C#:   Array.BinarySearch(arr, x)
来源：http://cby.aizwys.cn

[N02] 排序（工程实践用内置实现）
来源：http://bfm.yuxming.cn

Py:   sorted(arr);  arr.sort()
来源：http://ryb.zdbjq.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://zme.sufxvd.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://knc.nanxuanxn.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://eao.bjfxy.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ywp.cheryme.top

Go:   slices.Sort(arr)
来源：http://kfi.sjlbkw.cn

Ruby: arr.sort
来源：http://axv.andypj.xyz

C#:   Array.Sort(arr);  list.Sort()
来源：http://rmm.ydzc1.top

[N03] 快速排序（分治示例）
来源：http://ldi.jinghuilouyu.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://sbk.ydjk.org.cn

PHP:  // 递归实现，或用 usort
来源：http://siz.snrcjt.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://dap.yvedp.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://uxg.jqgufenzy.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://goy.shanyushiyangtech.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://nmc.zhoulong.xyz

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://cgi.epnwcf.com

C#:   // 手写递归，或 Array.Sort
来源：http://hwp.hfpthk.cn

[N04] 斐波那契数列
来源：http://xao.haohaochexian.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://zjw.yj202588.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://bbi.nanxuanxn.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://jvv.xuetiantiany.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hin.bjfxy.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://kiy.pycfn.com

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ljt.hesvh.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://yof.wangshuangyany.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://tzf.gotoacloud.top

[N05] 最大公约数
来源：http://bjm.xuanzx.com

Py:   math.gcd(a, b)
来源：http://agj.tian-w.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://aae.yj202588.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hhw.dashuyun.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://qfd.daxiang520.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://zwt.shuidangran.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://jfe.zhijiandao.cn

Ruby: a.gcd(b)
来源：http://ygh.zhoulong.xyz

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mmm.shangyingyoupin.top

[N06] 判断回文字符串
来源：http://pza.yvedp.cn

Py:   s == s[::-1]
来源：http://cwa.jinghuilouyu.cn

PHP:  $s === strrev($s);
来源：http://kuf.wangshuangyany.cn

JS:   s === [...s].reverse().join("")
来源：http://qby.gzhubu.top

TS:   s === [...s].reverse().join("")
来源：http://muj.guannengcc.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://jqh.fzhhl.top

Go:   // 双指针从两端比较
来源：http://uiu.jinyuanbaomall.cn

Ruby: s == s.reverse
来源：http://rth.nanxinkj.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://owb.nanxuanxn.top

[N07] 两数之和（返回下标）
来源：http://bfe.dianchejie.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://tvp.cheryme.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mvw.gaohongyu789.top

JS:   // 手写 Map：map.set(v, i)
来源：http://grd.shanyushiyangkeji.top

TS:   // 手写 Map<string, number>
来源：http://bng.wangdashe.top

Java: // 手写 HashMap
来源：http://hzj.smart0.xyz

Go:   // 手写 map[int]int
来源：http://fwj.cqqwz.cn

Ruby: // 手写 Hash
来源：http://dbs.yonumen.top

C#:   // 手写 Dictionary<int, int>
来源：http://odg.cdnleiting.top

[N08] 生成全排列
来源：http://vdm.aizwys.cn

Py:   itertools.permutations(arr)
来源：http://ryz.ehwqpu.com

PHP:  // 手写递归交换
来源：http://ddu.daxiang520.top

JS:   // 手写回溯递归
来源：http://myy.gzhubu.top

TS:   // 手写回溯递归
来源：http://dgq.hongshengwenyu.top

Java: // 手写回溯递归
来源：http://hcl.ydjk.org.cn

Go:   // 手写回溯递归
来源：http://lfq.shanyushiyangkeji.top

Ruby: arr.permutation.to_a
来源：http://eew.cdnleiting.top

C#:   // 手写回溯递归
来源：http://pkn.xziqi.cn

[N09] 栈与队列
来源：http://zpw.cashguo.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://xen.gzhubu.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mss.316326.xyz

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://yrc.havefunace.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mvt.tarul.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://zor.hysaishi.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://gto.zhiwuduotai.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://bcd.dashuyun.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://kvw.hysaishi.cn

[N10] 链表节点定义
来源：http://lwy.chenjidiqi.icu

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://iea.dianchejie.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://rtg.gotoacloud.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://afs.guowangkeji.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://spo.yuxming.cn

Java: class Node { int v; Node next; }
来源：http://peo.zhixingplan.top

Go:   type Node struct { V int; Next *Node }
来源：http://lwj.yfazqb.com

Ruby: Node = Struct.new(:v, :next)
来源：http://hgn.daria6918.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://kgf.yj20258888.top

[N11] 二叉树中序遍历
来源：http://oee.ctjpmb.com

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ylw.hfpthk.cn

PHP:  // 手写递归函数
来源：http://nmb.yj202588.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://sup.zdbjq.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://eeo.tian-w.cn

Java: // 手写递归
来源：http://fda.ybcxt.top

Go:   // 手写递归
来源：http://ppt.ydzc1.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://sgg.fehbvm.com

C#:   // 手写递归
来源：http://vyp.dianchejie.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://osl.redwolf501.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://tde.xinyue.icu

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ukf.sjlbkw.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ocb.shuidangran.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ttq.cashguo.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mgo.tarul.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://fcb.wangshuangyany.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://yir.haohaochexian.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://tlf.xylfe.cn

================================================================================
来源：http://hpb.ehwqpu.com

O. 并发与异步
来源：http://fpp.yongpay.top

================================================================================
来源：http://qsf.uphjek.com

[O01] 启动一个线程
来源：http://qku.ppjwa.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://rlk.epnwcf.com

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://qqd.jinqigufen.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://evn.316326.xyz

TS:   // 同 JS
来源：http://zyu.yangfankeji.com

Java: new Thread(() -> f()).start()
来源：http://zra.wangshuangyany.cn

Go:   go f()
来源：http://ivd.xylfe.cn

Ruby: Thread.new { f }
来源：http://tdl.sweek.top

C#:   Task.Run(() => F());
来源：http://xdr.ctjpmb.com

[O02] 使用线程池
来源：http://use.9152youxi.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://eww.ehwqpu.com

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://laz.quarkkingdee.top

JS:   // worker_threads 线程池
来源：http://obr.gzhubu.top

TS:   // worker_threads 线程池
来源：http://bqm.jqgufenzy.top

Java: Executors.newFixedThreadPool(4)
来源：http://hbp.bbcook.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://dua.shanyushiyangkeji.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wpm.hywenlv.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://sca.yuanzhike.top

[O03] 加锁保护共享数据
来源：http://kgr.hcnkem.com

Py:   with lock: shared += 1
来源：http://kqh.yvedp.cn

PHP:  // 用 flock() 做文件锁
来源：http://xij.zycfv.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://nsa.chenjidiqi.icu

TS:   // 同 JS
来源：http://wnf.jianghu66.top

Java: synchronized (this) { shared++; }
来源：http://vhl.tianlin.xyz

Go:   mu.Lock();  defer mu.Unlock()
来源：http://yri.fktsv.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://twf.gogol.net.cn

C#:   lock (gate) { shared++; }
来源：http://knt.chenjidiqi.icu

[O04] 定义异步函数并等待
来源：http://ivw.smart0.xyz

Py:   async def f():⏎    await g()
来源：http://myu.shanyushiyangkeji.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://vmh.nanxinkj.top

JS:   async function f() { await g(); }
来源：http://iac.cheryme.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://btm.svipenyu.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://dwn.yonumen.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://toh.yj202588.top

Ruby: # 用 Fiber 或 async gem
来源：http://eup.shuidangran.top

C#:   async Task F() { await G(); }
来源：http://vep.aibaodan.cn

[O05] 并发执行并等待全部完成
来源：http://vlb.sysykeji.top

Py:   asyncio.gather(*tasks)
来源：http://flx.ehwqpu.com

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ojj.nanxuanxn.top

JS:   await Promise.all(tasks)
来源：http://qzw.epnwcf.com

TS:   await Promise.all(tasks)
来源：http://kqe.tianlin.xyz

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://kuq.hcnkem.com

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://aro.xingfuxueyuan.xyz

Ruby: threads.map(&:join)
来源：http://imh.chenzaomai.com

C#:   await Task.WhenAll(t1, t2)
来源：http://ykj.daria6918.cn

[O06] 使用进程池
来源：http://see.vqdsnc.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://uum.hnxiangtu.top

PHP:  // pcntl_fork 或多进程队列
来源：http://iam.tianlin.xyz

JS:   // child_process / cluster 模块
来源：http://lvg.jinqigufen.top

TS:   // child_process / cluster 模块
来源：http://vdu.hammf.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ogt.zycfv.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://rie.shangyingyoupin.top

Ruby: // fork 块
来源：http://aqw.gaohongyu789.top

C#:   Parallel.For
来源：http://jsr.sweek.top

================================================================================
来源：http://wsq.xuetiantiany.cn

P. 常用工具函数
来源：http://qgi.zdqjudy.top

================================================================================
来源：http://abm.nwbrower.top

[P01] 生成 UUID
来源：http://qxs.fengsongda.top

Py:   str(uuid.uuid4())
来源：http://vzw.zhiwuduotai.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://bst.bbcook.cn

JS:   crypto.randomUUID()
来源：http://qyt.zycfv.cn


<!-- 参考信息 -->