代发 wailian999

[L03] 设置自定义请求头
来源：http://azb.hywenlv.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://muo.wangdashe.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://gom.sxryk.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://evu.xylfe.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://tdz.gotoacloud.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ffq.ywan-chungtsiang.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hqd.aizwys.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://xdn.kuanghao11.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://eje.cdnleiting.top

[L04] 设置超时
来源：http://gaa.guannengcc.top

Py:   requests.get(url, timeout=5)
来源：http://qsy.epnwcf.com

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://vxg.tianlin.xyz

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://kim.hywenlv.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ksj.yj20258888.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://egx.jyoumei.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mbt.fengsongda.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://myl.jiagoushi.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://qvw.tarul.cn

[L05] 上传文件（multipart）
来源：http://wdj.fehbvm.com

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ufo.daria6918.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://frh.pycfn.com

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ikb.jyoumei.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://iln.daria6918.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://szq.dashuyun.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://kik.jyoumei.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://rtm.sjlbkw.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://del.jinyuanbaomall.cn

[L06] 解析响应为 JSON
来源：http://eie.9152youxi.cn

Py:   resp.json()
来源：http://uks.yangfankeji.com

PHP:  json_decode($body, true);
来源：http://ihr.guannengcc.top

JS:   await resp.json()
来源：http://tma.haohaochexian.top

TS:   await resp.json()
来源：http://kjl.svipenyu.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wim.iojbl.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://fdl.hnqzz.top

Ruby: JSON.parse(resp.body)
来源：http://ncd.316326.xyz

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://rrh.birdmap.top

[L07] 处理 HTTP 状态码
来源：http://ybj.yfazqb.com

Py:   resp.status_code;  resp.raise_for_status()
来源：http://utq.fanxiaobao.xyz

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ziq.ybcxt.top

JS:   resp.ok;  resp.status
来源：http://hne.ydzc1.top

TS:   resp.ok;  resp.status
来源：http://zxt.snrcjt.cn

Java: resp.statusCode()
来源：http://jyw.52xcode.cn

Go:   resp.StatusCode
来源：http://hwk.quarkkingdee.top

Ruby: resp.code.to_i
来源：http://tvl.ydjk.org.cn

C#:   (int)resp.StatusCode
来源：http://hmk.wangdashe.top

[L08] 并发请求多个地址
来源：http://wso.haohaochexian.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://spv.jiagoushi.top

PHP:  curl_multi_init() 系列
来源：http://twu.bbcook.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://xfo.xuanzx.com

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ahz.sxryk.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://kuu.fehbvm.com

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://xbk.zhiwuduotai.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://rpj.nwbrower.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://qie.bbcook.cn

================================================================================
来源：http://exo.316326.xyz

M. 命令行 / 进程 / 环境
来源：http://cwk.jinqigfzy.top

================================================================================
来源：http://lpp.tarul.cn

[M01] 读取命令行参数
来源：http://zsc.pengpengdd.cyou

Py:   sys.argv[1:]
来源：http://gik.dianchejie.cn

PHP:  $argv;  $argc;
来源：http://zet.jiagoushi.top

JS:   process.argv.slice(2)
来源：http://pmv.pycfn.com

TS:   process.argv.slice(2)
来源：http://ujh.hywenlv.cn

Java: args 数组（main 方法参数）
来源：http://eyy.yj202588.top

Go:   os.Args[1:]
来源：http://gsa.guowangkeji.top

Ruby: ARGV
来源：http://byv.aibaodan.cn

C#:   args 数组（Main 方法参数）
来源：http://cso.jinghuilouyu.cn

[M02] 读取环境变量
来源：http://vsu.yuanzhike.top

Py:   os.environ.get("HOME")
来源：http://irw.nwbrower.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://sdw.316326.xyz

JS:   process.env.HOME
来源：http://umb.gzhubu.top

TS:   process.env.HOME
来源：http://mzt.daxiang520.top

Java: System.getenv("HOME")
来源：http://qks.fehbvm.com

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wji.yangfankeji.com

Ruby: ENV["HOME"]
来源：http://fik.tanke756.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wui.meibo888.top

[M03] 执行外部命令
来源：http://vgz.pycfn.com

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://nbb.0kj1m.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hhw.zhixingplan.top

JS:   child_process.execSync("ls -l").toString()
来源：http://fna.wangdashe.top

TS:   child_process.execSync("ls -l").toString()
来源：http://fxa.pycfn.com

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wjl.daxiang520.top

Go:   exec.Command("ls", "-l").Output()
来源：http://gih.gotoacloud.top

Ruby: system("ls -l");  `ls -l`
来源：http://uga.jqgfzy.top

C#:   Process.Start("ls", "-l");
来源：http://dzc.cqqwz.cn

[M04] 获取当前工作目录
来源：http://dep.sufxvd.cn

Py:   os.getcwd()
来源：http://eam.aibaodan.cn

PHP:  getcwd();
来源：http://ald.tarul.cn

JS:   process.cwd()
来源：http://tid.shzxlz.cn

TS:   process.cwd()
来源：http://bgx.meibo888.top

Java: Path.of("").toAbsolutePath()
来源：http://bji.svipenyu.cn

Go:   os.Getwd()
来源：http://ixv.xylfe.cn

Ruby: Dir.pwd
来源：http://ivz.pycfn.com

C#:   Directory.GetCurrentDirectory()
来源：http://uqy.nwbrower.top

[M05] 设置退出码
来源：http://jev.vehdjk.com

Py:   sys.exit(1)
来源：http://mhb.hongshengwenyu.top

PHP:  exit(1);
来源：http://dwl.dashuyun.cn

JS:   process.exit(1)
来源：http://qad.hammf.cn

TS:   process.exit(1)
来源：http://ifa.yfazqb.com

Java: System.exit(1)
来源：http://hwr.cashguo.top

Go:   os.Exit(1)
来源：http://dip.jiagoushi.top

Ruby: exit 1
来源：http://fml.chenjidiqi.icu

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://gxg.shuidangran.top

[M06] 向标准错误输出
来源：http://hdj.cheryme.top

Py:   print("err", file=sys.stderr)
来源：http://wiy.zdqjudy.top

PHP:  fwrite(STDERR, "err\n");
来源：http://gfd.zhongyouzk.top

JS:   console.error("err")
来源：http://dcc.chenzaomai.com

TS:   console.error("err")
来源：http://vrq.nanxuanxn.top

Java: System.err.println("err")
来源：http://pbs.ydjk.org.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hhy.zhiwuduotai.top

Ruby: warn "err"
来源：http://jgs.ybcxt.top

C#:   Console.Error.WriteLine("err")
来源：http://mcn.jinqigufen.top

[M07] 判断是否为主入口
来源：http://iqc.tianlin.xyz

Py:   if __name__ == "__main__":
来源：http://xok.sjlbkw.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mri.52xcode.cn

JS:   require.main === module
来源：http://lyc.meibo888.top

TS:   require.main === module
来源：http://ilk.zhaomingkeji.xyz

Java: public static void main(String[] args)
来源：http://qro.bbcook.cn

Go:   func main()
来源：http://dvb.zhongyouzk.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://tde.ywan-chungtsiang.top

C#:   static void Main(string[] args)
来源：http://fos.dashuyun.cn

[M08] 获取系统与运行时信息
来源：http://frg.52xcode.cn

Py:   platform.system();  platform.python_version()
来源：http://fxh.havefunace.top

PHP:  PHP_OS;  phpversion();
来源：http://qvx.52xcode.cn

JS:   process.platform;  process.version
来源：http://jig.zhiwuduotai.top

TS:   process.platform;  process.version
来源：http://rct.chenzaomai.com

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://kkr.ydjk.org.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://uin.xuanzx.com

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://klm.hongshengwenyu.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://jxs.hesvh.cn

================================================================================
来源：http://djc.jinyuanbaomall.cn

N. 数据结构与算法
来源：http://vpa.sjlbkw.cn

================================================================================
来源：http://jpp.zhixingplan.top

[N01] 二分查找（有序数组）
来源：http://yny.chenzaomai.com

Py:   bisect.bisect_left(arr, x)
来源：http://erk.ybcxt.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://jsi.uphjek.com

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://icp.xuanzx.com

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://uig.nwbrower.top

Java: Arrays.binarySearch(arr, x)
来源：http://awg.yanxiufei.cn

Go:   sort.SearchInts(arr, x)
来源：http://guo.chenzaomai.com

Ruby: arr.bsearch { |e| e >= x }
来源：http://gme.tarul.cn

C#:   Array.BinarySearch(arr, x)
来源：http://eft.xuetiantiany.cn

[N02] 排序（工程实践用内置实现）
来源：http://hqt.shanyushiyangtech.top

Py:   sorted(arr);  arr.sort()
来源：http://kvs.jinqigufen.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://gwq.hammf.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://uqc.andypj.xyz

TS:   [...arr].sort((a, b) => a - b)
来源：http://jpk.0kj1m.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://nax.zdbjq.cn

Go:   slices.Sort(arr)
来源：http://awp.smart0.xyz

Ruby: arr.sort
来源：http://iuv.wangdashe.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://dvh.vqdsnc.cn

[N03] 快速排序（分治示例）
来源：http://zcj.sufxvd.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://jmj.ehwqpu.com

PHP:  // 递归实现，或用 usort
来源：http://kxz.tarul.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://bwb.zhoulong.xyz

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://aev.sysykeji.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://txi.xuanzx.com

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://lhc.zhengqikj.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ttt.ctjpmb.com

C#:   // 手写递归，或 Array.Sort
来源：http://aea.zhengqikj.top

[N04] 斐波那契数列
来源：http://clq.9152youxi.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://xsl.gaohongyu789.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://bld.yfazqb.com

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mif.guowangkeji.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ygh.shzxlz.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wdv.feifeiyinyue.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wda.yueranfly.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://soe.meibo888.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://iwn.tian-w.cn

[N05] 最大公约数
来源：http://dkl.ctjpmb.com

Py:   math.gcd(a, b)
来源：http://zzo.nanxinkj.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://fns.xinyue.icu

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://dof.xingfuxueyuan.xyz

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://daj.sufxvd.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://pfq.jiagoushi.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://prb.pengpengdd.cyou

Ruby: a.gcd(b)
来源：http://cbo.havefunace.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://sqb.0kj1m.cn

[N06] 判断回文字符串
来源：http://krp.jinqigfzy.top

Py:   s == s[::-1]
来源：http://tpa.yj20258888.top

PHP:  $s === strrev($s);
来源：http://cel.ivvv.top

JS:   s === [...s].reverse().join("")
来源：http://uoe.jianghu66.top

TS:   s === [...s].reverse().join("")
来源：http://bkk.52xcode.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://fla.andypj.xyz

Go:   // 双指针从两端比较
来源：http://tdr.shzxlz.cn

Ruby: s == s.reverse
来源：http://wsv.zhongyouzk.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://vsw.jyoumei.cn

[N07] 两数之和（返回下标）
来源：http://gco.kuanghao11.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://vud.zhiwuduotai.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://uej.vehdjk.com

JS:   // 手写 Map：map.set(v, i)
来源：http://cfn.ybcxt.top

TS:   // 手写 Map<string, number>
来源：http://qxf.xuanzx.com

Java: // 手写 HashMap
来源：http://afd.fktsv.cn

Go:   // 手写 map[int]int
来源：http://sgb.yonumen.top

Ruby: // 手写 Hash
来源：http://sbs.iojbl.cn

C#:   // 手写 Dictionary<int, int>
来源：http://pbp.yueranfly.top

[N08] 生成全排列
来源：http://pdv.zhongyouzk.top

Py:   itertools.permutations(arr)
来源：http://xzz.uphjek.com

PHP:  // 手写递归交换
来源：http://ied.zhixingplan.top

JS:   // 手写回溯递归
来源：http://jvg.shangyingyoupin.top

TS:   // 手写回溯递归
来源：http://ilj.ydjk.org.cn

Java: // 手写回溯递归
来源：http://sid.yuxming.cn

Go:   // 手写回溯递归
来源：http://xxk.bbcook.cn

Ruby: arr.permutation.to_a
来源：http://ori.jinqigufen.top

C#:   // 手写回溯递归
来源：http://oki.shanyushiyangkeji.top

[N09] 栈与队列
来源：http://lne.jqgufenzy.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://bpq.guowangkeji.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://bzc.gzhubu.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://cij.zycfv.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ogj.fzhhl.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://zqu.kuanghao11.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ycz.jianghu66.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://bvj.chenlongwang.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://tbj.quarkkingdee.top

[N10] 链表节点定义
来源：http://brw.sxryk.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://dyi.vqdsnc.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://leu.feifeiyinyue.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ixy.zhaomingkeji.xyz

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://aza.hywenlv.cn

Java: class Node { int v; Node next; }
来源：http://pgo.uphjek.com

Go:   type Node struct { V int; Next *Node }
来源：http://uic.xingfuxueyuan.xyz

Ruby: Node = Struct.new(:v, :next)
来源：http://vau.xylfe.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://iug.gaohongyu789.top

[N11] 二叉树中序遍历
来源：http://jjy.pengpengdd.cyou

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://tqz.zhengqikj.top

PHP:  // 手写递归函数
来源：http://pzm.chenjidiqi.icu

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wpr.fanxiaobao.xyz

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://lfr.ydzc1.top

Java: // 手写递归
来源：http://dte.cucudq.cn

Go:   // 手写递归
来源：http://ezc.xylfe.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hkx.meibo888.top

C#:   // 手写递归
来源：http://gkm.yuanzhike.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://vqr.ywan-chungtsiang.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://llk.cheryme.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://okv.birdmap.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://eih.52xcode.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://fjt.wangdashe.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://gqu.birdmap.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mja.havefunace.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://eeb.shanyushiyangtech.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ono.jinqigfzy.top

================================================================================
来源：http://bwy.bjfxy.top

O. 并发与异步
来源：http://jri.tanke756.top

================================================================================
来源：http://ded.52xcode.cn

[O01] 启动一个线程
来源：http://yvq.yanxiufei.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://vag.ywan-chungtsiang.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://tjz.ivvv.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://yuo.hongshengwenyu.top

TS:   // 同 JS
来源：http://sdy.jinyuanbaomall.cn

Java: new Thread(() -> f()).start()
来源：http://csz.0kj1m.cn

Go:   go f()
来源：http://emq.0kj1m.cn

Ruby: Thread.new { f }
来源：http://yat.c1oappe.top

C#:   Task.Run(() => F());
来源：http://hjv.yongpay.top

[O02] 使用线程池
来源：http://eoc.gogol.net.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://iwx.zhengqikj.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hnr.jiagoushi.top

JS:   // worker_threads 线程池
来源：http://ols.jqgufenzy.top

TS:   // worker_threads 线程池
来源：http://vwy.zhijiandao.cn

Java: Executors.newFixedThreadPool(4)
来源：http://arw.fzhhl.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://xmx.snrcjt.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://lxp.chenzaomai.com

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://han.ydzc1.top

[O03] 加锁保护共享数据
来源：http://tnl.yuxming.cn

Py:   with lock: shared += 1
来源：http://xdo.wangshuangyany.cn

PHP:  // 用 flock() 做文件锁
来源：http://uzm.yueranfly.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mgc.guowangkeji.top

TS:   // 同 JS
来源：http://hqa.hnxiangtu.top

Java: synchronized (this) { shared++; }
来源：http://csj.fktsv.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mat.yanxiufei.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://vyz.xuetiantiany.cn

C#:   lock (gate) { shared++; }
来源：http://tks.hnqzz.top

[O04] 定义异步函数并等待
来源：http://dwk.jqgfzy.top

Py:   async def f():⏎    await g()
来源：http://vay.ctjpmb.com

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mpr.sxryk.cn

JS:   async function f() { await g(); }
来源：http://exa.gogol.net.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://myv.tianlin.xyz

Java: // 用 CompletableFuture 或虚拟线程
来源：http://fpw.c1oappe.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ogq.sjlbkw.cn

Ruby: # 用 Fiber 或 async gem
来源：http://peo.zhengqikj.top

C#:   async Task F() { await G(); }
来源：http://scy.bbcook.cn

[O05] 并发执行并等待全部完成
来源：http://uzf.daxiang520.top

Py:   asyncio.gather(*tasks)
来源：http://cgx.ydjk.org.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ixl.meibo888.top

JS:   await Promise.all(tasks)
来源：http://zyp.cdnleiting.top

TS:   await Promise.all(tasks)
来源：http://ksq.vqdsnc.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hdh.shanyushiyangkeji.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://orz.fzhhl.top

Ruby: threads.map(&:join)
来源：http://hyp.tian-w.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://let.zhoulong.xyz

[O06] 使用进程池
来源：http://hvp.zhaomingkeji.xyz

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://erf.cashguo.top

PHP:  // pcntl_fork 或多进程队列
来源：http://hoa.ehwqpu.com

JS:   // child_process / cluster 模块
来源：http://fhv.jinqigfzy.top

TS:   // child_process / cluster 模块
来源：http://nhp.shanyushiyangkeji.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://klm.uphjek.com

Go:   // goroutine 已占用多核，直接并发即可
来源：http://lly.jianghu66.top

Ruby: // fork 块
来源：http://yta.zdqjudy.top

C#:   Parallel.For
来源：http://ukt.gotoacloud.top

================================================================================
来源：http://fxk.nwbrower.top

P. 常用工具函数
来源：http://xzd.yvedp.cn

================================================================================
来源：http://oyl.daxiang520.top


<!-- 参考信息 -->