代发 wailian999

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mgz.sysykeji.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ump.hesvh.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://zbf.yuanzhike.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://scv.kuanghao11.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mxh.zhixingplan.top

[L04] 设置超时
来源：http://rmq.jlsjyb.cn

Py:   requests.get(url, timeout=5)
来源：http://cgi.cashguo.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://dmt.yonumen.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wau.hesvh.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://djm.wangshuangyany.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://aii.wangdashe.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://gin.birdmap.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ddy.guannengcc.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://cyi.iojbl.cn

[L05] 上传文件（multipart）
来源：http://mqd.ydzc1.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://cfo.gaohongyu789.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hni.hnqzz.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mij.yj202588.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://raq.birdmap.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://qbn.sysykeji.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wce.wangdashe.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ibb.zhijiandao.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://dkq.wangshuangyany.cn

[L06] 解析响应为 JSON
来源：http://lsc.havefunace.top

Py:   resp.json()
来源：http://zwl.pengpengdd.cyou

PHP:  json_decode($body, true);
来源：http://spj.zdqjudy.top

JS:   await resp.json()
来源：http://jcl.tianlin.xyz

TS:   await resp.json()
来源：http://nta.hnqzz.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://jhn.yvedp.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ylx.yonumen.top

Ruby: JSON.parse(resp.body)
来源：http://lyl.smart0.xyz

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://edl.gogol.net.cn

[L07] 处理 HTTP 状态码
来源：http://nxn.yj20258.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://joo.chenjidiqi.icu

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://oqo.ywan-chungtsiang.top

JS:   resp.ok;  resp.status
来源：http://wna.vqdsnc.cn

TS:   resp.ok;  resp.status
来源：http://tsg.wangshuangyany.cn

Java: resp.statusCode()
来源：http://gae.chenzaomai.com

Go:   resp.StatusCode
来源：http://afa.havefunace.top

Ruby: resp.code.to_i
来源：http://bza.chenjidiqi.icu

C#:   (int)resp.StatusCode
来源：http://emz.fehbvm.com

[L08] 并发请求多个地址
来源：http://kfp.gaohongyu789.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://axn.fktsv.cn

PHP:  curl_multi_init() 系列
来源：http://qpn.fzhhl.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://vqc.jqgufenzy.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://rvg.yuanzhike.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://yhz.zdbjq.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://qdq.hesvh.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://oko.iojbl.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://gpj.xinyue.icu

================================================================================
来源：http://hqo.xinyue.icu

M. 命令行 / 进程 / 环境
来源：http://ido.zhaomingkeji.xyz

================================================================================
来源：http://lys.xylfe.cn

[M01] 读取命令行参数
来源：http://ers.fzhhl.top

Py:   sys.argv[1:]
来源：http://ymn.52xcode.cn

PHP:  $argv;  $argc;
来源：http://aeo.jlsjyb.cn

JS:   process.argv.slice(2)
来源：http://thg.sxryk.cn

TS:   process.argv.slice(2)
来源：http://kzt.hywenlv.cn

Java: args 数组（main 方法参数）
来源：http://ngf.fzhhl.top

Go:   os.Args[1:]
来源：http://wjx.quarkkingdee.top

Ruby: ARGV
来源：http://ehz.jqgufenzy.top

C#:   args 数组（Main 方法参数）
来源：http://iiv.9152youxi.cn

[M02] 读取环境变量
来源：http://xnl.shangyingyoupin.top

Py:   os.environ.get("HOME")
来源：http://rkg.hcnkem.com

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://fav.shanyushiyangkeji.top

JS:   process.env.HOME
来源：http://zzf.jinqigufen.top

TS:   process.env.HOME
来源：http://qar.sjlbkw.cn

Java: System.getenv("HOME")
来源：http://bhf.yfazqb.com

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://gfi.chenlongwang.top

Ruby: ENV["HOME"]
来源：http://leq.hongshengwenyu.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://czd.hongshengwenyu.top

[M03] 执行外部命令
来源：http://whu.svipenyu.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://lsv.cheryme.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://oye.shanyushiyangkeji.top

JS:   child_process.execSync("ls -l").toString()
来源：http://qgp.birdmap.top

TS:   child_process.execSync("ls -l").toString()
来源：http://tzq.hongshengwenyu.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://odx.zhengqikj.top

Go:   exec.Command("ls", "-l").Output()
来源：http://ana.shanyushiyangtech.top

Ruby: system("ls -l");  `ls -l`
来源：http://ejn.uphjek.com

C#:   Process.Start("ls", "-l");
来源：http://cup.daxiang520.top

[M04] 获取当前工作目录
来源：http://lfd.yongpay.top

Py:   os.getcwd()
来源：http://avw.cashguo.top

PHP:  getcwd();
来源：http://hnr.wangshuangyany.cn

JS:   process.cwd()
来源：http://rst.fengsongda.top

TS:   process.cwd()
来源：http://wdm.zhiwuduotai.top

Java: Path.of("").toAbsolutePath()
来源：http://gyl.cucudq.cn

Go:   os.Getwd()
来源：http://uqm.yj20258888.top

Ruby: Dir.pwd
来源：http://aze.yonumen.top

C#:   Directory.GetCurrentDirectory()
来源：http://rln.havefunace.top

[M05] 设置退出码
来源：http://cru.yueranfly.top

Py:   sys.exit(1)
来源：http://swi.zdbjq.cn

PHP:  exit(1);
来源：http://opk.zhijiandao.cn

JS:   process.exit(1)
来源：http://dbb.zhaomingkeji.xyz

TS:   process.exit(1)
来源：http://rqk.fzhhl.top

Java: System.exit(1)
来源：http://wca.yuanzhike.top

Go:   os.Exit(1)
来源：http://emc.xuanzx.com

Ruby: exit 1
来源：http://nlp.jqgfzy.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://okp.sjlbkw.cn

[M06] 向标准错误输出
来源：http://hme.cqqwz.cn

Py:   print("err", file=sys.stderr)
来源：http://pcd.cqqwz.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://eom.ywan-chungtsiang.top

JS:   console.error("err")
来源：http://blu.hfpthk.cn

TS:   console.error("err")
来源：http://nvu.xinyue.icu

Java: System.err.println("err")
来源：http://hsl.hcnkem.com

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://myn.nwbrower.top

Ruby: warn "err"
来源：http://ten.shanyushiyangkeji.top

C#:   Console.Error.WriteLine("err")
来源：http://wia.vqdsnc.cn

[M07] 判断是否为主入口
来源：http://vhl.xingfuxueyuan.xyz

Py:   if __name__ == "__main__":
来源：http://imp.birdmap.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://toe.feifeiyinyue.top

JS:   require.main === module
来源：http://eva.smart0.xyz

TS:   require.main === module
来源：http://dbl.hnqzz.top

Java: public static void main(String[] args)
来源：http://fiz.cqqwz.cn

Go:   func main()
来源：http://lfp.chenjidiqi.icu

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://qrq.xinyue.icu

C#:   static void Main(string[] args)
来源：http://dlc.hcnkem.com

[M08] 获取系统与运行时信息
来源：http://juz.nanxuanxn.top

Py:   platform.system();  platform.python_version()
来源：http://rkx.yongpay.top

PHP:  PHP_OS;  phpversion();
来源：http://nvr.yangfankeji.com

JS:   process.platform;  process.version
来源：http://ozd.redwolf501.top

TS:   process.platform;  process.version
来源：http://iqv.shangyingyoupin.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://kyq.jinqigufen.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://wsn.cucudq.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://epw.zhoulong.xyz

C#:   Environment.OSVersion;  Environment.Version
来源：http://vig.hfpthk.cn

================================================================================
来源：http://huj.cheryme.top

N. 数据结构与算法
来源：http://vhv.aizwys.cn

================================================================================
来源：http://lbn.nwbrower.top

[N01] 二分查找（有序数组）
来源：http://sma.316326.xyz

Py:   bisect.bisect_left(arr, x)
来源：http://qqx.chenlongwang.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://bca.tianlin.xyz

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://unr.jqgufenzy.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://cbm.yfazqb.com

Java: Arrays.binarySearch(arr, x)
来源：http://wew.zhoulong.xyz

Go:   sort.SearchInts(arr, x)
来源：http://znw.kuanghao11.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://tjd.hammf.cn

C#:   Array.BinarySearch(arr, x)
来源：http://dsm.zhiwuduotai.top

[N02] 排序（工程实践用内置实现）
来源：http://fxl.havefunace.top

Py:   sorted(arr);  arr.sort()
来源：http://lqv.tian-w.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hsu.hesvh.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://zvt.jianghu66.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://wrj.dashuyun.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://bnl.vehdjk.com

Go:   slices.Sort(arr)
来源：http://kbu.chenlongwang.top

Ruby: arr.sort
来源：http://jnc.yfazqb.com

C#:   Array.Sort(arr);  list.Sort()
来源：http://vpr.cucudq.cn

[N03] 快速排序（分治示例）
来源：http://wog.316326.xyz

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mhz.yanxiufei.cn

PHP:  // 递归实现，或用 usort
来源：http://lec.birdmap.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wxu.shanyushiyangkeji.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mnj.jinyuanbaomall.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://sga.shuidangran.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://yrs.yvedp.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://omf.ywan-chungtsiang.top

C#:   // 手写递归，或 Array.Sort
来源：http://yao.shuidangran.top

[N04] 斐波那契数列
来源：http://wea.shuidangran.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://pah.fehbvm.com

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://pfj.zdbjq.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://pfd.sjlbkw.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://lob.jlsjyb.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://feq.0kj1m.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://pad.sweek.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ciy.zdqjudy.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wju.birdmap.top

[N05] 最大公约数
来源：http://wic.jqgufenzy.top

Py:   math.gcd(a, b)
来源：http://nlz.0kj1m.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://xco.daria6918.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://udt.sysykeji.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://qrb.daxiang520.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hwb.yonumen.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://gxw.jianghu66.top

Ruby: a.gcd(b)
来源：http://try.wangshuangyany.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://zev.zhongyouzk.top

[N06] 判断回文字符串
来源：http://yqp.smart0.xyz

Py:   s == s[::-1]
来源：http://ofu.quarkkingdee.top

PHP:  $s === strrev($s);
来源：http://fzz.shanyushiyangkeji.top

JS:   s === [...s].reverse().join("")
来源：http://pzi.sjlbkw.cn

TS:   s === [...s].reverse().join("")
来源：http://cik.zdqjudy.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://buu.hnqzz.top

Go:   // 双指针从两端比较
来源：http://olc.jiagoushi.top

Ruby: s == s.reverse
来源：http://ztk.zhongyouzk.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://ndc.ehwqpu.com

[N07] 两数之和（返回下标）
来源：http://xld.chenzaomai.com

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ixy.guowangkeji.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hgs.zhixingplan.top

JS:   // 手写 Map：map.set(v, i)
来源：http://eok.ybcxt.top

TS:   // 手写 Map<string, number>
来源：http://dpp.smart0.xyz

Java: // 手写 HashMap
来源：http://ffs.zhiwuduotai.top

Go:   // 手写 map[int]int
来源：http://twu.nanxuanxn.top

Ruby: // 手写 Hash
来源：http://jiy.fengsongda.top

C#:   // 手写 Dictionary<int, int>
来源：http://dno.havefunace.top

[N08] 生成全排列
来源：http://itd.shangyingyoupin.top

Py:   itertools.permutations(arr)
来源：http://nhp.zhongyouzk.top

PHP:  // 手写递归交换
来源：http://vfy.tianlin.xyz

JS:   // 手写回溯递归
来源：http://tdc.cqqwz.cn

TS:   // 手写回溯递归
来源：http://agx.vqdsnc.cn

Java: // 手写回溯递归
来源：http://cdx.nwbrower.top

Go:   // 手写回溯递归
来源：http://igk.chenzaomai.com

Ruby: arr.permutation.to_a
来源：http://flr.feifeiyinyue.top

C#:   // 手写回溯递归
来源：http://bbu.xziqi.cn

[N09] 栈与队列
来源：http://pdx.hywenlv.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mzv.zycfv.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://axs.hfpthk.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://kue.daria6918.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://abt.gogol.net.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://oqn.vehdjk.com

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://abn.gogol.net.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://yun.yvedp.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://zhn.cheryme.top

[N10] 链表节点定义
来源：http://bop.zhijiandao.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://veg.haohaochexian.top

PHP:  class Node { public $v; public $next = null; }
来源：http://fdq.gotoacloud.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://suw.yueranfly.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://von.hywenlv.cn

Java: class Node { int v; Node next; }
来源：http://pas.wangshuangyany.cn

Go:   type Node struct { V int; Next *Node }
来源：http://hxw.sufxvd.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://bml.cashguo.top

C#:   class Node { public int V; public Node? Next; }
来源：http://apx.hnxiangtu.top

[N11] 二叉树中序遍历
来源：http://frq.dianchejie.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://job.guannengcc.top

PHP:  // 手写递归函数
来源：http://bdr.ywan-chungtsiang.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://gwr.epnwcf.com

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://eer.52xcode.cn

Java: // 手写递归
来源：http://hig.fehbvm.com

Go:   // 手写递归
来源：http://oia.wangdashe.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://nju.hysaishi.cn

C#:   // 手写递归
来源：http://eqt.hnxiangtu.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://qmg.pengpengdd.cyou

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://nsh.birdmap.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://kfk.zycfv.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://cww.yueranfly.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://yht.guannengcc.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://jrn.zhixingplan.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wif.jyoumei.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://dhn.cdnleiting.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://heb.sjlbkw.cn

================================================================================
来源：http://tbx.zdqjudy.top

O. 并发与异步
来源：http://swv.meibo888.top

================================================================================
来源：http://jfg.yongpay.top

[O01] 启动一个线程
来源：http://ldn.fzhhl.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://pyk.jinqigufen.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://lss.shzxlz.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wib.yueranfly.top

TS:   // 同 JS
来源：http://hmm.yangfankeji.com

Java: new Thread(() -> f()).start()
来源：http://agc.pengpengdd.cyou

Go:   go f()
来源：http://pip.zdqjudy.top

Ruby: Thread.new { f }
来源：http://crr.hammf.cn

C#:   Task.Run(() => F());
来源：http://ooh.havefunace.top

[O02] 使用线程池
来源：http://eko.sufxvd.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://api.yonumen.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://yar.jyoumei.cn

JS:   // worker_threads 线程池
来源：http://jtk.yuxming.cn

TS:   // worker_threads 线程池
来源：http://tup.ehwqpu.com

Java: Executors.newFixedThreadPool(4)
来源：http://agu.jlsjyb.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://pyi.xinyue.icu

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://phs.wangdashe.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://bxg.yanxiufei.cn

[O03] 加锁保护共享数据
来源：http://qri.birdmap.top

Py:   with lock: shared += 1
来源：http://eja.jinyuanbaomall.cn

PHP:  // 用 flock() 做文件锁
来源：http://wkh.jqgfzy.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hwy.cheryme.top

TS:   // 同 JS
来源：http://crq.uphjek.com

Java: synchronized (this) { shared++; }
来源：http://wun.shangyingyoupin.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://srk.hnqzz.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://iyx.redwolf501.top

C#:   lock (gate) { shared++; }
来源：http://kmf.0kj1m.cn

[O04] 定义异步函数并等待
来源：http://cml.jianghu66.top

Py:   async def f():⏎    await g()
来源：http://hdu.jiagoushi.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://xyz.iojbl.cn

JS:   async function f() { await g(); }
来源：http://ybl.meibo888.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://odf.hnqzz.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://jdy.yuxming.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ola.yonumen.top

Ruby: # 用 Fiber 或 async gem
来源：http://lzr.cashguo.top

C#:   async Task F() { await G(); }
来源：http://bfl.meibo888.top

[O05] 并发执行并等待全部完成
来源：http://qol.guowangkeji.top

Py:   asyncio.gather(*tasks)
来源：http://niu.pycfn.com

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://qvl.meibo888.top

JS:   await Promise.all(tasks)
来源：http://ufb.zhijiandao.cn

TS:   await Promise.all(tasks)
来源：http://lzo.jlsjyb.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://kzt.smart0.xyz

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://taf.hnxiangtu.top

Ruby: threads.map(&:join)
来源：http://kzt.yfazqb.com

C#:   await Task.WhenAll(t1, t2)
来源：http://epm.chenjidiqi.icu

[O06] 使用进程池
来源：http://nje.smart0.xyz

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://abx.zdbjq.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://uku.zhoulong.xyz

JS:   // child_process / cluster 模块
来源：http://loq.tianlin.xyz

TS:   // child_process / cluster 模块
来源：http://dae.zhaomingkeji.xyz

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://bzw.ybcxt.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://pur.nwbrower.top

Ruby: // fork 块
来源：http://nnh.zhengqikj.top

C#:   Parallel.For
来源：http://pjn.zhoulong.xyz

================================================================================
来源：http://unr.jyoumei.cn

P. 常用工具函数
来源：http://mtm.zhengqikj.top

================================================================================
来源：http://ngy.ppjwa.cn

[P01] 生成 UUID
来源：http://hkj.yonumen.top

Py:   str(uuid.uuid4())
来源：http://alw.dashuyun.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ogb.gzhubu.top

JS:   crypto.randomUUID()
来源：http://jte.xylfe.cn


<!-- 参考信息 -->