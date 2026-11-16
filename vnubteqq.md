代发 wailian999

Go:   resp, err := http.Get(url)
来源：http://ovu.birdmap.top

Ruby: Net::HTTP.get(URI(url))
来源：http://zgd.redwolf501.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://cgx.fehbvm.com

[L02] 发送 POST JSON
来源：http://cyx.snrcjt.cn

Py:   requests.post(url, json={"a": 1})
来源：http://yrh.meibo888.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://qfv.wangshuangyany.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hop.quarkkingdee.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://lwa.fehbvm.com

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://rbu.fzhhl.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://tmy.jqgfzy.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://sho.pengpengdd.cyou

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://idv.aizwys.cn

[L03] 设置自定义请求头
来源：http://iwj.hnxiangtu.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://pkf.hnxiangtu.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ztg.redwolf501.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://opy.yuxming.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ycs.shangyingyoupin.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://aqk.jlsjyb.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://bcb.sweek.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://nwy.jqgfzy.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wow.iojbl.cn

[L04] 设置超时
来源：http://rij.yuanzhike.top

Py:   requests.get(url, timeout=5)
来源：http://epx.shuidangran.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://nha.yonumen.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hzr.yueranfly.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hmh.hnxiangtu.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://iea.hesvh.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://vdt.cqqwz.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://jjs.feifeiyinyue.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://yxx.sjlbkw.cn

[L05] 上传文件（multipart）
来源：http://fqz.52xcode.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://umo.9152youxi.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ums.mhx1999.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://omw.dashuyun.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://kev.hesvh.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://byo.guowangkeji.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://gfv.havefunace.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://tju.hcnkem.com

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://jaf.chenzaomai.com

[L06] 解析响应为 JSON
来源：http://ued.guowangkeji.top

Py:   resp.json()
来源：http://var.yanxiufei.cn

PHP:  json_decode($body, true);
来源：http://oxh.c1oappe.top

JS:   await resp.json()
来源：http://fhh.pycfn.com

TS:   await resp.json()
来源：http://qod.shanyushiyangtech.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hgg.aizwys.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://sfj.yfazqb.com

Ruby: JSON.parse(resp.body)
来源：http://tkd.zhoulong.xyz

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://faw.bjfxy.top

[L07] 处理 HTTP 状态码
来源：http://rnh.hnxiangtu.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://xfd.chenlongwang.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://fgh.fanxiaobao.xyz

JS:   resp.ok;  resp.status
来源：http://lev.meibo888.top

TS:   resp.ok;  resp.status
来源：http://uvz.jqgfzy.top

Java: resp.statusCode()
来源：http://ghl.vqdsnc.cn

Go:   resp.StatusCode
来源：http://nuf.epnwcf.com

Ruby: resp.code.to_i
来源：http://lwm.jyoumei.cn

C#:   (int)resp.StatusCode
来源：http://mtt.fzhhl.top

[L08] 并发请求多个地址
来源：http://ecd.yonumen.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://fdz.dashuyun.cn

PHP:  curl_multi_init() 系列
来源：http://fyz.yj20258888.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://fkj.hysaishi.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://pek.daria6918.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://neq.zhixingplan.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://env.zdqjudy.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://nkv.hcnkem.com

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://fui.pengpengdd.cyou

================================================================================
来源：http://aid.ctjpmb.com

M. 命令行 / 进程 / 环境
来源：http://imw.yanxiufei.cn

================================================================================
来源：http://csr.cashguo.top

[M01] 读取命令行参数
来源：http://cgy.shangyingyoupin.top

Py:   sys.argv[1:]
来源：http://coy.xinyue.icu

PHP:  $argv;  $argc;
来源：http://dsb.zhaomingkeji.xyz

JS:   process.argv.slice(2)
来源：http://zrc.sysykeji.top

TS:   process.argv.slice(2)
来源：http://arw.tanke756.top

Java: args 数组（main 方法参数）
来源：http://dlf.hysaishi.cn

Go:   os.Args[1:]
来源：http://qrh.shanyushiyangtech.top

Ruby: ARGV
来源：http://nyo.quarkkingdee.top

C#:   args 数组（Main 方法参数）
来源：http://djk.ybcxt.top

[M02] 读取环境变量
来源：http://cum.nwbrower.top

Py:   os.environ.get("HOME")
来源：http://zyc.jqgfzy.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://vwj.yuanzhike.top

JS:   process.env.HOME
来源：http://ilc.sufxvd.cn

TS:   process.env.HOME
来源：http://loj.bjfxy.top

Java: System.getenv("HOME")
来源：http://mkf.xuetiantiany.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://oam.cashguo.top

Ruby: ENV["HOME"]
来源：http://ahp.jqgfzy.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://kha.ydzc1.top

[M03] 执行外部命令
来源：http://cqf.cheryme.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://afs.ppjwa.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://yfw.zdqjudy.top

JS:   child_process.execSync("ls -l").toString()
来源：http://nfh.shzxlz.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://gio.dianchejie.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://jju.chenlongwang.top

Go:   exec.Command("ls", "-l").Output()
来源：http://jkx.xingfuxueyuan.xyz

Ruby: system("ls -l");  `ls -l`
来源：http://phd.aizwys.cn

C#:   Process.Start("ls", "-l");
来源：http://xmd.hongshengwenyu.top

[M04] 获取当前工作目录
来源：http://lis.zycfv.cn

Py:   os.getcwd()
来源：http://gdk.fanxiaobao.xyz

PHP:  getcwd();
来源：http://vcl.jlsjyb.cn

JS:   process.cwd()
来源：http://wwr.guowangkeji.top

TS:   process.cwd()
来源：http://ckd.hysaishi.cn

Java: Path.of("").toAbsolutePath()
来源：http://bdw.redwolf501.top

Go:   os.Getwd()
来源：http://pse.quarkkingdee.top

Ruby: Dir.pwd
来源：http://gyc.aizwys.cn

C#:   Directory.GetCurrentDirectory()
来源：http://nlt.pengpengdd.cyou

[M05] 设置退出码
来源：http://hsb.bbcook.cn

Py:   sys.exit(1)
来源：http://zko.jinqigufen.top

PHP:  exit(1);
来源：http://hal.hnqzz.top

JS:   process.exit(1)
来源：http://jvf.pycfn.com

TS:   process.exit(1)
来源：http://joq.hnxiangtu.top

Java: System.exit(1)
来源：http://coh.snrcjt.cn

Go:   os.Exit(1)
来源：http://cuk.gzhubu.top

Ruby: exit 1
来源：http://yry.c1oappe.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://oaf.52xcode.cn

[M06] 向标准错误输出
来源：http://bax.yuxming.cn

Py:   print("err", file=sys.stderr)
来源：http://tec.gogol.net.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://hcl.yuanzhike.top

JS:   console.error("err")
来源：http://trp.hysaishi.cn

TS:   console.error("err")
来源：http://bbq.tarul.cn

Java: System.err.println("err")
来源：http://tok.tian-w.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://efa.cdnleiting.top

Ruby: warn "err"
来源：http://qjp.yangfankeji.com

C#:   Console.Error.WriteLine("err")
来源：http://ygb.zhiwuduotai.top

[M07] 判断是否为主入口
来源：http://fxt.wangshuangyany.cn

Py:   if __name__ == "__main__":
来源：http://lje.sjlbkw.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://xln.nanxinkj.top

JS:   require.main === module
来源：http://uoj.zhengqikj.top

TS:   require.main === module
来源：http://kxt.uphjek.com

Java: public static void main(String[] args)
来源：http://gce.bjfxy.top

Go:   func main()
来源：http://fiv.sjlbkw.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://qfl.gotoacloud.top

C#:   static void Main(string[] args)
来源：http://ewt.cdnleiting.top

[M08] 获取系统与运行时信息
来源：http://ink.zhaomingkeji.xyz

Py:   platform.system();  platform.python_version()
来源：http://fmn.yuanzhike.top

PHP:  PHP_OS;  phpversion();
来源：http://aoa.tian-w.cn

JS:   process.platform;  process.version
来源：http://zyc.yangfankeji.com

TS:   process.platform;  process.version
来源：http://csa.ppjwa.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ayx.cdnleiting.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://afi.hfpthk.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://pwu.dashuyun.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://zbj.jinyuanbaomall.cn

================================================================================
来源：http://dhs.wangshuangyany.cn

N. 数据结构与算法
来源：http://yap.gotoacloud.top

================================================================================
来源：http://cdm.316326.xyz

[N01] 二分查找（有序数组）
来源：http://orf.tarul.cn

Py:   bisect.bisect_left(arr, x)
来源：http://wfh.hfpthk.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://fla.fanxiaobao.xyz

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://nuy.ybcxt.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://vfz.iojbl.cn

Java: Arrays.binarySearch(arr, x)
来源：http://inl.shuidangran.top

Go:   sort.SearchInts(arr, x)
来源：http://zlr.zhiwuduotai.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://syl.jinghuilouyu.cn

C#:   Array.BinarySearch(arr, x)
来源：http://lnu.tarul.cn

[N02] 排序（工程实践用内置实现）
来源：http://gbo.yonumen.top

Py:   sorted(arr);  arr.sort()
来源：http://ned.nwbrower.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://kjn.bjfxy.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://guu.yuxming.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://ivr.jyoumei.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://orj.xuetiantiany.cn

Go:   slices.Sort(arr)
来源：http://iyu.dianchejie.cn

Ruby: arr.sort
来源：http://cni.xziqi.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://zmg.bbcook.cn

[N03] 快速排序（分治示例）
来源：http://ewa.hywenlv.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://fon.yj20258888.top

PHP:  // 递归实现，或用 usort
来源：http://uub.chenlongwang.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://pxa.pengpengdd.cyou

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mxc.daria6918.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ukp.xziqi.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://tby.ctjpmb.com

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://prq.hfpthk.cn

C#:   // 手写递归，或 Array.Sort
来源：http://juv.ydjk.org.cn

[N04] 斐波那契数列
来源：http://fgj.dashuyun.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://urv.yuanzhike.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://bay.yvedp.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mrj.zdqjudy.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://iir.daria6918.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mkx.pycfn.com

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wom.jqgufenzy.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://lnt.yj202588.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hyw.jyoumei.cn

[N05] 最大公约数
来源：http://iqy.cashguo.top

Py:   math.gcd(a, b)
来源：http://xeo.fehbvm.com

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hkl.sxryk.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://jku.ehwqpu.com

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ctb.sxryk.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://alh.ydzc1.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ujj.birdmap.top

Ruby: a.gcd(b)
来源：http://hnx.cdnleiting.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://rfy.sufxvd.cn

[N06] 判断回文字符串
来源：http://crz.zhoulong.xyz

Py:   s == s[::-1]
来源：http://kdz.vehdjk.com

PHP:  $s === strrev($s);
来源：http://rpb.hesvh.cn

JS:   s === [...s].reverse().join("")
来源：http://yax.xylfe.cn

TS:   s === [...s].reverse().join("")
来源：http://tub.cqqwz.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://oxc.gogol.net.cn

Go:   // 双指针从两端比较
来源：http://dck.jinqigfzy.top

Ruby: s == s.reverse
来源：http://nzn.xuanzx.com

C#:   s == new string(s.Reverse().ToArray())
来源：http://hpm.ppjwa.cn

[N07] 两数之和（返回下标）
来源：http://tfl.c1oappe.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://lrr.wangshuangyany.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://icv.52xcode.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://diu.tian-w.cn

TS:   // 手写 Map<string, number>
来源：http://ril.nanxinkj.top

Java: // 手写 HashMap
来源：http://kuq.ybcxt.top

Go:   // 手写 map[int]int
来源：http://shp.zhixingplan.top

Ruby: // 手写 Hash
来源：http://kfn.epnwcf.com

C#:   // 手写 Dictionary<int, int>
来源：http://ljm.ppjwa.cn

[N08] 生成全排列
来源：http://jpu.zycfv.cn

Py:   itertools.permutations(arr)
来源：http://mxt.chenlongwang.top

PHP:  // 手写递归交换
来源：http://kox.wangdashe.top

JS:   // 手写回溯递归
来源：http://kma.52xcode.cn

TS:   // 手写回溯递归
来源：http://veq.hfpthk.cn

Java: // 手写回溯递归
来源：http://uax.xziqi.cn

Go:   // 手写回溯递归
来源：http://eix.zdbjq.cn

Ruby: arr.permutation.to_a
来源：http://cax.ivvv.top

C#:   // 手写回溯递归
来源：http://pqv.zdbjq.cn

[N09] 栈与队列
来源：http://sur.hcnkem.com

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://gko.uphjek.com

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://olb.zdqjudy.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ygn.snrcjt.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://uti.xziqi.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://uvi.meibo888.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ato.jinqigufen.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ocp.hammf.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://knd.bbcook.cn

[N10] 链表节点定义
来源：http://sry.jlsjyb.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mye.zdqjudy.top

PHP:  class Node { public $v; public $next = null; }
来源：http://bes.smart0.xyz

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://fqw.316326.xyz

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://swn.chenlongwang.top

Java: class Node { int v; Node next; }
来源：http://gyf.yvedp.cn

Go:   type Node struct { V int; Next *Node }
来源：http://fpm.jinghuilouyu.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://ove.daxiang520.top

C#:   class Node { public int V; public Node? Next; }
来源：http://wvf.xinyue.icu

[N11] 二叉树中序遍历
来源：http://rrj.bbcook.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wsv.xinyue.icu

PHP:  // 手写递归函数
来源：http://xhl.xuetiantiany.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://gco.shangyingyoupin.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://fop.yvedp.cn

Java: // 手写递归
来源：http://iem.nwbrower.top

Go:   // 手写递归
来源：http://kqw.yj20258888.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://rnd.xuanzx.com

C#:   // 手写递归
来源：http://nnm.sweek.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://juq.andypj.xyz

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ysp.svipenyu.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mdl.guannengcc.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://nxr.andypj.xyz

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ekr.hfpthk.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ilv.cheryme.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mls.cqqwz.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://iti.wangdashe.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://pzs.shangyingyoupin.top

================================================================================
来源：http://olu.bjfxy.top

O. 并发与异步
来源：http://irm.zhixingplan.top

================================================================================
来源：http://rvd.fktsv.cn

[O01] 启动一个线程
来源：http://uwx.wangshuangyany.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://lzw.jqgufenzy.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://fjj.fktsv.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mcm.smart0.xyz

TS:   // 同 JS
来源：http://jgf.hesvh.cn

Java: new Thread(() -> f()).start()
来源：http://aay.shangyingyoupin.top

Go:   go f()
来源：http://jrv.ivvv.top

Ruby: Thread.new { f }
来源：http://ygv.meibo888.top

C#:   Task.Run(() => F());
来源：http://jnf.shanyushiyangkeji.top

[O02] 使用线程池
来源：http://gfo.hcnkem.com

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ytw.cdnleiting.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://koh.vehdjk.com

JS:   // worker_threads 线程池
来源：http://qks.xinyue.icu

TS:   // worker_threads 线程池
来源：http://qmd.hesvh.cn

Java: Executors.newFixedThreadPool(4)
来源：http://kce.jyoumei.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://izw.ydjk.org.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wnn.aibaodan.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wsn.fzhhl.top

[O03] 加锁保护共享数据
来源：http://pqm.xuanzx.com

Py:   with lock: shared += 1
来源：http://ksq.hnxiangtu.top

PHP:  // 用 flock() 做文件锁
来源：http://dad.smart0.xyz

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://erp.uphjek.com

TS:   // 同 JS
来源：http://ahr.hnqzz.top

Java: synchronized (this) { shared++; }
来源：http://tnc.gotoacloud.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://lce.daria6918.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://kyw.zhaomingkeji.xyz

C#:   lock (gate) { shared++; }
来源：http://mrj.daria6918.cn

[O04] 定义异步函数并等待
来源：http://vei.yuanzhike.top

Py:   async def f():⏎    await g()
来源：http://exa.ydjk.org.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ahn.hnxiangtu.top

JS:   async function f() { await g(); }
来源：http://tiu.jinqigufen.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://nvp.bjfxy.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://att.zdbjq.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://bhp.hnqzz.top

Ruby: # 用 Fiber 或 async gem
来源：http://mqq.xuanzx.com

C#:   async Task F() { await G(); }
来源：http://lcg.aibaodan.cn

[O05] 并发执行并等待全部完成
来源：http://zez.yj20258888.top

Py:   asyncio.gather(*tasks)
来源：http://zmh.zhixingplan.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://czl.yueranfly.top

JS:   await Promise.all(tasks)
来源：http://ijz.smart0.xyz

TS:   await Promise.all(tasks)
来源：http://ptp.nwbrower.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ojc.yfazqb.com

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://way.nanxuanxn.top

Ruby: threads.map(&:join)
来源：http://txq.yanxiufei.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://vgc.pengpengdd.cyou


<!-- 参考信息 -->