代发 wailian999

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://pxq.zhiwuduotai.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ygb.yonumen.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://tnb.dianchejie.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://goo.chenlongwang.top

[L03] 设置自定义请求头
来源：http://jmk.daria6918.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://fip.daxiang520.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://tys.ivvv.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://kdj.hfpthk.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://fuo.hysaishi.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://kln.tianlin.xyz

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://qxu.zhixingplan.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://dhx.tarul.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ycq.zdbjq.cn

[L04] 设置超时
来源：http://jcp.daxiang520.top

Py:   requests.get(url, timeout=5)
来源：http://bgl.vqdsnc.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://jqg.sysykeji.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://cdz.tian-w.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://egm.dianchejie.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://bux.fktsv.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wla.shangyingyoupin.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://fwk.fanxiaobao.xyz

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://vof.bjfxy.top

[L05] 上传文件（multipart）
来源：http://gqr.gotoacloud.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://cmz.hongshengwenyu.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://diu.jlsjyb.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wvy.fktsv.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hvl.yangfankeji.com

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://gjk.fzhhl.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://tsd.jianghu66.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://qwk.andypj.xyz

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://dtr.cheryme.top

[L06] 解析响应为 JSON
来源：http://ddp.xuanzx.com

Py:   resp.json()
来源：http://zou.9152youxi.cn

PHP:  json_decode($body, true);
来源：http://own.chenjidiqi.icu

JS:   await resp.json()
来源：http://tma.bjfxy.top

TS:   await resp.json()
来源：http://gcm.chenzaomai.com

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://zxf.jlsjyb.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://vod.epnwcf.com

Ruby: JSON.parse(resp.body)
来源：http://jly.yueranfly.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://vox.tian-w.cn

[L07] 处理 HTTP 状态码
来源：http://bou.guannengcc.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://nwm.guowangkeji.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mfv.tian-w.cn

JS:   resp.ok;  resp.status
来源：http://dxw.sjlbkw.cn

TS:   resp.ok;  resp.status
来源：http://adq.zhengqikj.top

Java: resp.statusCode()
来源：http://qxw.sufxvd.cn

Go:   resp.StatusCode
来源：http://cmj.zhaomingkeji.xyz

Ruby: resp.code.to_i
来源：http://klq.yuxming.cn

C#:   (int)resp.StatusCode
来源：http://cxf.wangdashe.top

[L08] 并发请求多个地址
来源：http://shb.sjlbkw.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wsj.iojbl.cn

PHP:  curl_multi_init() 系列
来源：http://gzx.316326.xyz

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://qoq.jlsjyb.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://kkw.ctjpmb.com

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wjo.zhixingplan.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wop.shuidangran.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://sch.9152youxi.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://gmf.cqqwz.cn

================================================================================
来源：http://jbr.sjlbkw.cn

M. 命令行 / 进程 / 环境
来源：http://aij.chenlongwang.top

================================================================================
来源：http://qyw.nwbrower.top

[M01] 读取命令行参数
来源：http://xwn.nanxinkj.top

Py:   sys.argv[1:]
来源：http://xlp.epnwcf.com

PHP:  $argv;  $argc;
来源：http://egl.316326.xyz

JS:   process.argv.slice(2)
来源：http://ofg.yj202588.top

TS:   process.argv.slice(2)
来源：http://jny.sysykeji.top

Java: args 数组（main 方法参数）
来源：http://qmg.wangdashe.top

Go:   os.Args[1:]
来源：http://hbt.9152youxi.cn

Ruby: ARGV
来源：http://fvq.yueranfly.top

C#:   args 数组（Main 方法参数）
来源：http://ohf.xylfe.cn

[M02] 读取环境变量
来源：http://kin.cashguo.top

Py:   os.environ.get("HOME")
来源：http://srf.hammf.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://auy.hongshengwenyu.top

JS:   process.env.HOME
来源：http://zuy.shuidangran.top

TS:   process.env.HOME
来源：http://yvc.bbcook.cn

Java: System.getenv("HOME")
来源：http://zfs.yuanzhike.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://yal.vehdjk.com

Ruby: ENV["HOME"]
来源：http://ejd.52xcode.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://qyl.gzhubu.top

[M03] 执行外部命令
来源：http://bqp.quarkkingdee.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://oxo.tanke756.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://vfa.fzhhl.top

JS:   child_process.execSync("ls -l").toString()
来源：http://vfs.yangfankeji.com

TS:   child_process.execSync("ls -l").toString()
来源：http://iop.jinqigfzy.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://dls.zhaomingkeji.xyz

Go:   exec.Command("ls", "-l").Output()
来源：http://sdl.vehdjk.com

Ruby: system("ls -l");  `ls -l`
来源：http://oqf.epnwcf.com

C#:   Process.Start("ls", "-l");
来源：http://ude.hongshengwenyu.top

[M04] 获取当前工作目录
来源：http://xei.hnqzz.top

Py:   os.getcwd()
来源：http://iee.zhijiandao.cn

PHP:  getcwd();
来源：http://job.bjfxy.top

JS:   process.cwd()
来源：http://gjx.guannengcc.top

TS:   process.cwd()
来源：http://thi.cqqwz.cn

Java: Path.of("").toAbsolutePath()
来源：http://kcy.quarkkingdee.top

Go:   os.Getwd()
来源：http://ihq.shuidangran.top

Ruby: Dir.pwd
来源：http://nyu.yanxiufei.cn

C#:   Directory.GetCurrentDirectory()
来源：http://tyj.feifeiyinyue.top

[M05] 设置退出码
来源：http://igy.nanxuanxn.top

Py:   sys.exit(1)
来源：http://yki.jianghu66.top

PHP:  exit(1);
来源：http://lta.jiagoushi.top

JS:   process.exit(1)
来源：http://fbm.yj202588.top

TS:   process.exit(1)
来源：http://sci.hnxiangtu.top

Java: System.exit(1)
来源：http://qsz.tarul.cn

Go:   os.Exit(1)
来源：http://fad.ppjwa.cn

Ruby: exit 1
来源：http://xts.yj20258.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://pqi.haohaochexian.top

[M06] 向标准错误输出
来源：http://qtl.zhengqikj.top

Py:   print("err", file=sys.stderr)
来源：http://pak.hysaishi.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://glq.yonumen.top

JS:   console.error("err")
来源：http://phq.fktsv.cn

TS:   console.error("err")
来源：http://hyz.svipenyu.cn

Java: System.err.println("err")
来源：http://yps.aibaodan.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hlb.cheryme.top

Ruby: warn "err"
来源：http://dqa.cucudq.cn

C#:   Console.Error.WriteLine("err")
来源：http://esg.cqqwz.cn

[M07] 判断是否为主入口
来源：http://yrm.bjfxy.top

Py:   if __name__ == "__main__":
来源：http://ify.yonumen.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://kfp.feifeiyinyue.top

JS:   require.main === module
来源：http://fbm.yuanzhike.top

TS:   require.main === module
来源：http://peg.guannengcc.top

Java: public static void main(String[] args)
来源：http://owq.aizwys.cn

Go:   func main()
来源：http://dxa.ehwqpu.com

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://xqj.yuanzhike.top

C#:   static void Main(string[] args)
来源：http://jki.pycfn.com

[M08] 获取系统与运行时信息
来源：http://ffu.nwbrower.top

Py:   platform.system();  platform.python_version()
来源：http://mna.dianchejie.cn

PHP:  PHP_OS;  phpversion();
来源：http://xpx.epnwcf.com

JS:   process.platform;  process.version
来源：http://wup.redwolf501.top

TS:   process.platform;  process.version
来源：http://xiz.hysaishi.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://jps.svipenyu.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://vbg.cheryme.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://nnt.chenlongwang.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://woe.snrcjt.cn

================================================================================
来源：http://wpv.jinqigfzy.top

N. 数据结构与算法
来源：http://env.smart0.xyz

================================================================================
来源：http://asy.gaohongyu789.top

[N01] 二分查找（有序数组）
来源：http://zfr.meibo888.top

Py:   bisect.bisect_left(arr, x)
来源：http://cem.yueranfly.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ykd.fehbvm.com

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wlz.hysaishi.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://eig.zhaomingkeji.xyz

Java: Arrays.binarySearch(arr, x)
来源：http://qmv.hfpthk.cn

Go:   sort.SearchInts(arr, x)
来源：http://ann.jianghu66.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://sfu.zhengqikj.top

C#:   Array.BinarySearch(arr, x)
来源：http://uja.jinqigfzy.top

[N02] 排序（工程实践用内置实现）
来源：http://wjg.ppjwa.cn

Py:   sorted(arr);  arr.sort()
来源：http://sly.tianlin.xyz

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://jmu.pengpengdd.cyou

JS:   [...arr].sort((a, b) => a - b)
来源：http://oia.xuetiantiany.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://bis.zdqjudy.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hxr.zdbjq.cn

Go:   slices.Sort(arr)
来源：http://kvr.yj20258888.top

Ruby: arr.sort
来源：http://elm.ehwqpu.com

C#:   Array.Sort(arr);  list.Sort()
来源：http://xnh.havefunace.top

[N03] 快速排序（分治示例）
来源：http://dsq.sufxvd.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://pup.hnxiangtu.top

PHP:  // 递归实现，或用 usort
来源：http://moh.tanke756.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hty.ywan-chungtsiang.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://fyi.xylfe.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://oni.tarul.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://sfs.zhixingplan.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://fwt.mhx1999.top

C#:   // 手写递归，或 Array.Sort
来源：http://kmf.redwolf501.top

[N04] 斐波那契数列
来源：http://lzn.dashuyun.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://zjd.shanyushiyangkeji.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://bxf.jinqigfzy.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mvi.jinyuanbaomall.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mcy.cdnleiting.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://pfj.yangfankeji.com

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://dvl.316326.xyz

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://xxm.ppjwa.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mko.jlsjyb.cn

[N05] 最大公约数
来源：http://yhw.ydjk.org.cn

Py:   math.gcd(a, b)
来源：http://liq.ehwqpu.com

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://fcy.pengpengdd.cyou

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://det.jyoumei.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mdl.shzxlz.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ihi.meibo888.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://brn.xziqi.cn

Ruby: a.gcd(b)
来源：http://jsp.sxryk.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://zxv.cqqwz.cn

[N06] 判断回文字符串
来源：http://mkh.zhengqikj.top

Py:   s == s[::-1]
来源：http://vaa.cheryme.top

PHP:  $s === strrev($s);
来源：http://vyk.xuanzx.com

JS:   s === [...s].reverse().join("")
来源：http://hqj.xylfe.cn

TS:   s === [...s].reverse().join("")
来源：http://xpm.sxryk.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://pml.sjlbkw.cn

Go:   // 双指针从两端比较
来源：http://tgh.dashuyun.cn

Ruby: s == s.reverse
来源：http://snz.yangfankeji.com

C#:   s == new string(s.Reverse().ToArray())
来源：http://cgz.yueranfly.top

[N07] 两数之和（返回下标）
来源：http://kiq.feifeiyinyue.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://sps.jqgufenzy.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://zlq.sxryk.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://ofx.ydjk.org.cn

TS:   // 手写 Map<string, number>
来源：http://zjx.316326.xyz

Java: // 手写 HashMap
来源：http://trh.hcnkem.com

Go:   // 手写 map[int]int
来源：http://rmw.pycfn.com

Ruby: // 手写 Hash
来源：http://jfr.guannengcc.top

C#:   // 手写 Dictionary<int, int>
来源：http://wpu.andypj.xyz

[N08] 生成全排列
来源：http://lyn.zycfv.cn

Py:   itertools.permutations(arr)
来源：http://yca.nanxinkj.top

PHP:  // 手写递归交换
来源：http://siz.tarul.cn

JS:   // 手写回溯递归
来源：http://ksf.hnqzz.top

TS:   // 手写回溯递归
来源：http://scd.zhixingplan.top

Java: // 手写回溯递归
来源：http://ubq.hcnkem.com

Go:   // 手写回溯递归
来源：http://ptz.fzhhl.top

Ruby: arr.permutation.to_a
来源：http://sny.vqdsnc.cn

C#:   // 手写回溯递归
来源：http://rsq.wangdashe.top

[N09] 栈与队列
来源：http://pdw.yfazqb.com

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ydl.jyoumei.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://bfh.yueranfly.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://olh.nanxuanxn.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://fig.jqgufenzy.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ivl.snrcjt.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://cez.tianlin.xyz

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://htr.xziqi.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://adk.hesvh.cn

[N10] 链表节点定义
来源：http://otr.0kj1m.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://puh.tianlin.xyz

PHP:  class Node { public $v; public $next = null; }
来源：http://tmx.hfpthk.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ola.zhijiandao.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://pqk.hywenlv.cn

Java: class Node { int v; Node next; }
来源：http://mto.jqgfzy.top

Go:   type Node struct { V int; Next *Node }
来源：http://xsz.ehwqpu.com

Ruby: Node = Struct.new(:v, :next)
来源：http://wnr.gotoacloud.top

C#:   class Node { public int V; public Node? Next; }
来源：http://tkt.haohaochexian.top

[N11] 二叉树中序遍历
来源：http://lox.zhiwuduotai.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://dlh.xinyue.icu

PHP:  // 手写递归函数
来源：http://iol.xuetiantiany.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://iiv.pengpengdd.cyou

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://tip.smart0.xyz

Java: // 手写递归
来源：http://wux.pengpengdd.cyou

Go:   // 手写递归
来源：http://mmr.tanke756.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ojk.uphjek.com

C#:   // 手写递归
来源：http://yxx.316326.xyz

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://yqa.shzxlz.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://imt.cqqwz.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ekn.gogol.net.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ylz.316326.xyz

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://nbe.hongshengwenyu.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://kti.pengpengdd.cyou

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://kfy.jiagoushi.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://rof.sjlbkw.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://alu.yj202588.top

================================================================================
来源：http://rmu.bjfxy.top

O. 并发与异步
来源：http://iaw.bjfxy.top

================================================================================
来源：http://hee.hnxiangtu.top

[O01] 启动一个线程
来源：http://nnw.smart0.xyz

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://gdf.hnxiangtu.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://oqq.hongshengwenyu.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://bxh.zhijiandao.cn

TS:   // 同 JS
来源：http://lon.jqgufenzy.top

Java: new Thread(() -> f()).start()
来源：http://vvt.jlsjyb.cn

Go:   go f()
来源：http://xjb.fanxiaobao.xyz

Ruby: Thread.new { f }
来源：http://nko.cdnleiting.top

C#:   Task.Run(() => F());
来源：http://qhs.jqgufenzy.top

[O02] 使用线程池
来源：http://abf.epnwcf.com

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://epp.yvedp.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hcy.9152youxi.cn

JS:   // worker_threads 线程池
来源：http://woj.ctjpmb.com

TS:   // worker_threads 线程池
来源：http://nrl.jinyuanbaomall.cn

Java: Executors.newFixedThreadPool(4)
来源：http://evc.kuanghao11.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ogc.hongshengwenyu.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://psk.c1oappe.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://exw.cheryme.top

[O03] 加锁保护共享数据
来源：http://qnn.hcnkem.com

Py:   with lock: shared += 1
来源：http://ive.dianchejie.cn

PHP:  // 用 flock() 做文件锁
来源：http://ier.gzhubu.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mys.jlsjyb.cn

TS:   // 同 JS
来源：http://utx.ivvv.top

Java: synchronized (this) { shared++; }
来源：http://swr.jqgfzy.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://pqa.guannengcc.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://axw.guannengcc.top

C#:   lock (gate) { shared++; }
来源：http://izz.316326.xyz

[O04] 定义异步函数并等待
来源：http://ldl.aibaodan.cn

Py:   async def f():⏎    await g()
来源：http://noi.guowangkeji.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://cbu.yj20258888.top

JS:   async function f() { await g(); }
来源：http://xjj.sysykeji.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://aly.daxiang520.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ujl.jinyuanbaomall.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://lxu.ivvv.top

Ruby: # 用 Fiber 或 async gem
来源：http://ryf.shanyushiyangtech.top

C#:   async Task F() { await G(); }
来源：http://gml.wangdashe.top

[O05] 并发执行并等待全部完成
来源：http://qfc.jlsjyb.cn

Py:   asyncio.gather(*tasks)
来源：http://kna.bjfxy.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://xdr.xinyue.icu

JS:   await Promise.all(tasks)
来源：http://tew.sjlbkw.cn

TS:   await Promise.all(tasks)
来源：http://vqm.hcnkem.com

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ykc.shzxlz.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://qqx.yuanzhike.top

Ruby: threads.map(&:join)
来源：http://xtu.shanyushiyangtech.top

C#:   await Task.WhenAll(t1, t2)
来源：http://nkp.ppjwa.cn

[O06] 使用进程池
来源：http://utf.yuxming.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://cbo.yvedp.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://nng.ydjk.org.cn

JS:   // child_process / cluster 模块
来源：http://mwg.shanyushiyangkeji.top

TS:   // child_process / cluster 模块
来源：http://kvr.nanxuanxn.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://iqy.pycfn.com

Go:   // goroutine 已占用多核，直接并发即可
来源：http://olf.bbcook.cn

Ruby: // fork 块
来源：http://psz.ivvv.top


<!-- 参考信息 -->