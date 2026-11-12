代发 wailian999

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://cxv.iojbl.cn

JS:   await fetch(url)
来源：http://qld.cdnleiting.top

TS:   await fetch(url)
来源：http://sia.jiagoushi.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://crk.shuidangran.top

Go:   resp, err := http.Get(url)
来源：http://vkf.jqgufenzy.top

Ruby: Net::HTTP.get(URI(url))
来源：http://nua.hnqzz.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://cpb.tian-w.cn

[L02] 发送 POST JSON
来源：http://toh.zhijiandao.cn

Py:   requests.post(url, json={"a": 1})
来源：http://smv.feifeiyinyue.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://jug.shanyushiyangtech.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wcp.0kj1m.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://dqc.birdmap.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://fae.ydzc1.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://xet.yfazqb.com

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://xfn.52xcode.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://rou.tanke756.top

[L03] 设置自定义请求头
来源：http://urw.wangdashe.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://kpx.ppjwa.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://qeh.jlsjyb.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://jix.gogol.net.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://vjl.ppjwa.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://yer.smart0.xyz

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ety.hfpthk.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://sij.shzxlz.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://omx.dashuyun.cn

[L04] 设置超时
来源：http://pzn.tianlin.xyz

Py:   requests.get(url, timeout=5)
来源：http://hom.52xcode.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://qfn.tianlin.xyz

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://qvy.sufxvd.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://kop.tian-w.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://iea.aibaodan.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://tbp.vqdsnc.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://xxq.epnwcf.com

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://kcx.hnxiangtu.top

[L05] 上传文件（multipart）
来源：http://dvh.xingfuxueyuan.xyz

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://oew.guowangkeji.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://rpw.yuxming.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://faj.fzhhl.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://odl.jqgufenzy.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://kyh.nwbrower.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://qvh.epnwcf.com

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://bzi.haohaochexian.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hxc.hcnkem.com

[L06] 解析响应为 JSON
来源：http://nxs.cqqwz.cn

Py:   resp.json()
来源：http://jzi.shangyingyoupin.top

PHP:  json_decode($body, true);
来源：http://ldj.shangyingyoupin.top

JS:   await resp.json()
来源：http://tjm.gzhubu.top

TS:   await resp.json()
来源：http://waa.nanxuanxn.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wtr.xziqi.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://odk.nanxuanxn.top

Ruby: JSON.parse(resp.body)
来源：http://evx.jlsjyb.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://vum.pycfn.com

[L07] 处理 HTTP 状态码
来源：http://siw.zycfv.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://qap.yongpay.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://jhq.zhiwuduotai.top

JS:   resp.ok;  resp.status
来源：http://ywl.snrcjt.cn

TS:   resp.ok;  resp.status
来源：http://lek.sweek.top

Java: resp.statusCode()
来源：http://fhe.yanxiufei.cn

Go:   resp.StatusCode
来源：http://klv.yj20258888.top

Ruby: resp.code.to_i
来源：http://coy.fktsv.cn

C#:   (int)resp.StatusCode
来源：http://qek.redwolf501.top

[L08] 并发请求多个地址
来源：http://ewq.fanxiaobao.xyz

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://qry.uphjek.com

PHP:  curl_multi_init() 系列
来源：http://kvv.9152youxi.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://jzm.cdnleiting.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://zpb.ydjk.org.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://did.jinyuanbaomall.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://kwt.guowangkeji.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://afh.yueranfly.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wfw.meibo888.top

================================================================================
来源：http://igd.hysaishi.cn

M. 命令行 / 进程 / 环境
来源：http://mbw.yj20258888.top

================================================================================
来源：http://yun.hesvh.cn

[M01] 读取命令行参数
来源：http://yqp.zdqjudy.top

Py:   sys.argv[1:]
来源：http://oxk.snrcjt.cn

PHP:  $argv;  $argc;
来源：http://giq.hfpthk.cn

JS:   process.argv.slice(2)
来源：http://aor.gotoacloud.top

TS:   process.argv.slice(2)
来源：http://hop.hesvh.cn

Java: args 数组（main 方法参数）
来源：http://njt.fengsongda.top

Go:   os.Args[1:]
来源：http://ayu.yj20258888.top

Ruby: ARGV
来源：http://xqx.yfazqb.com

C#:   args 数组（Main 方法参数）
来源：http://wfy.xingfuxueyuan.xyz

[M02] 读取环境变量
来源：http://qib.tarul.cn

Py:   os.environ.get("HOME")
来源：http://ykl.sysykeji.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://rkx.yangfankeji.com

JS:   process.env.HOME
来源：http://kvu.jqgufenzy.top

TS:   process.env.HOME
来源：http://dbh.c1oappe.top

Java: System.getenv("HOME")
来源：http://ora.zhongyouzk.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://aun.xinyue.icu

Ruby: ENV["HOME"]
来源：http://pde.tianlin.xyz

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://bgk.hnxiangtu.top

[M03] 执行外部命令
来源：http://pni.fktsv.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ekm.birdmap.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://buv.zhijiandao.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://sjl.jinqigufen.top

TS:   child_process.execSync("ls -l").toString()
来源：http://gvv.cheryme.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://via.hesvh.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://czf.feifeiyinyue.top

Ruby: system("ls -l");  `ls -l`
来源：http://whr.haohaochexian.top

C#:   Process.Start("ls", "-l");
来源：http://dtb.bjfxy.top

[M04] 获取当前工作目录
来源：http://nds.hfpthk.cn

Py:   os.getcwd()
来源：http://mhn.fzhhl.top

PHP:  getcwd();
来源：http://kpt.sxryk.cn

JS:   process.cwd()
来源：http://und.fktsv.cn

TS:   process.cwd()
来源：http://voe.jinqigufen.top

Java: Path.of("").toAbsolutePath()
来源：http://ohb.sufxvd.cn

Go:   os.Getwd()
来源：http://ipa.yuanzhike.top

Ruby: Dir.pwd
来源：http://nra.hnxiangtu.top

C#:   Directory.GetCurrentDirectory()
来源：http://tcq.zhongyouzk.top

[M05] 设置退出码
来源：http://egj.bbcook.cn

Py:   sys.exit(1)
来源：http://yfx.hesvh.cn

PHP:  exit(1);
来源：http://hab.yueranfly.top

JS:   process.exit(1)
来源：http://ezi.tian-w.cn

TS:   process.exit(1)
来源：http://eed.gzhubu.top

Java: System.exit(1)
来源：http://xpy.ybcxt.top

Go:   os.Exit(1)
来源：http://xgq.zhiwuduotai.top

Ruby: exit 1
来源：http://tbf.zhijiandao.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ohv.shuidangran.top

[M06] 向标准错误输出
来源：http://eni.0kj1m.cn

Py:   print("err", file=sys.stderr)
来源：http://izd.jqgfzy.top

PHP:  fwrite(STDERR, "err\n");
来源：http://zie.fehbvm.com

JS:   console.error("err")
来源：http://lzf.mhx1999.top

TS:   console.error("err")
来源：http://iki.yangfankeji.com

Java: System.err.println("err")
来源：http://gwl.zhengqikj.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wmq.xinyue.icu

Ruby: warn "err"
来源：http://zjh.shzxlz.cn

C#:   Console.Error.WriteLine("err")
来源：http://esw.tian-w.cn

[M07] 判断是否为主入口
来源：http://iyu.zhixingplan.top

Py:   if __name__ == "__main__":
来源：http://ufz.redwolf501.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hsx.hcnkem.com

JS:   require.main === module
来源：http://ect.fengsongda.top

TS:   require.main === module
来源：http://gel.hnxiangtu.top

Java: public static void main(String[] args)
来源：http://ysy.zhengqikj.top

Go:   func main()
来源：http://oaq.ydzc1.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://iwy.chenlongwang.top

C#:   static void Main(string[] args)
来源：http://eer.jinqigufen.top

[M08] 获取系统与运行时信息
来源：http://oqw.fktsv.cn

Py:   platform.system();  platform.python_version()
来源：http://kpp.hfpthk.cn

PHP:  PHP_OS;  phpversion();
来源：http://wvg.chenzaomai.com

JS:   process.platform;  process.version
来源：http://fug.hfpthk.cn

TS:   process.platform;  process.version
来源：http://ixp.hesvh.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://eww.cucudq.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://tqg.sufxvd.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://xvr.xylfe.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://gvn.zhixingplan.top

================================================================================
来源：http://vwr.zhixingplan.top

N. 数据结构与算法
来源：http://oas.feifeiyinyue.top

================================================================================
来源：http://fxb.xziqi.cn

[N01] 二分查找（有序数组）
来源：http://jjy.ydjk.org.cn

Py:   bisect.bisect_left(arr, x)
来源：http://xpx.hammf.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mkx.jyoumei.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://vnm.bbcook.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://okv.cucudq.cn

Java: Arrays.binarySearch(arr, x)
来源：http://htc.fktsv.cn

Go:   sort.SearchInts(arr, x)
来源：http://txg.bjfxy.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://iho.yanxiufei.cn

C#:   Array.BinarySearch(arr, x)
来源：http://nja.gotoacloud.top

[N02] 排序（工程实践用内置实现）
来源：http://bjq.gogol.net.cn

Py:   sorted(arr);  arr.sort()
来源：http://jkk.epnwcf.com

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://sjw.smart0.xyz

JS:   [...arr].sort((a, b) => a - b)
来源：http://irs.hfpthk.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://zzs.ppjwa.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://axl.yuxming.cn

Go:   slices.Sort(arr)
来源：http://tzy.fanxiaobao.xyz

Ruby: arr.sort
来源：http://xau.nanxinkj.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://qca.yueranfly.top

[N03] 快速排序（分治示例）
来源：http://zjr.shzxlz.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://tcg.zhengqikj.top

PHP:  // 递归实现，或用 usort
来源：http://rjy.redwolf501.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://aia.daxiang520.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ghr.tian-w.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://zbr.yonumen.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://yyu.sweek.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ghc.yuxming.cn

C#:   // 手写递归，或 Array.Sort
来源：http://ljx.shzxlz.cn

[N04] 斐波那契数列
来源：http://qpv.gzhubu.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://vhf.fzhhl.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://fyf.yueranfly.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hma.yangfankeji.com

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ylb.tanke756.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://yba.pycfn.com

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://zvc.hnqzz.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://fyf.sysykeji.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://yec.fanxiaobao.xyz

[N05] 最大公约数
来源：http://fdh.zhijiandao.cn

Py:   math.gcd(a, b)
来源：http://yer.shzxlz.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://kqq.316326.xyz

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://pjo.52xcode.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://xto.cdnleiting.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://pnw.ctjpmb.com

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://yfp.zhaomingkeji.xyz

Ruby: a.gcd(b)
来源：http://xrx.gzhubu.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ewd.aibaodan.cn

[N06] 判断回文字符串
来源：http://gpb.sxryk.cn

Py:   s == s[::-1]
来源：http://kjs.xuanzx.com

PHP:  $s === strrev($s);
来源：http://eez.yvedp.cn

JS:   s === [...s].reverse().join("")
来源：http://dff.nwbrower.top

TS:   s === [...s].reverse().join("")
来源：http://vrz.yongpay.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ssh.yuxming.cn

Go:   // 双指针从两端比较
来源：http://fzt.jqgfzy.top

Ruby: s == s.reverse
来源：http://gqs.zhixingplan.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://rwa.jqgfzy.top

[N07] 两数之和（返回下标）
来源：http://unu.cheryme.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://tow.fzhhl.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://adr.hnxiangtu.top

JS:   // 手写 Map：map.set(v, i)
来源：http://tnc.jlsjyb.cn

TS:   // 手写 Map<string, number>
来源：http://evl.yueranfly.top

Java: // 手写 HashMap
来源：http://kzf.sufxvd.cn

Go:   // 手写 map[int]int
来源：http://jaq.hongshengwenyu.top

Ruby: // 手写 Hash
来源：http://xyv.fehbvm.com

C#:   // 手写 Dictionary<int, int>
来源：http://uhb.andypj.xyz

[N08] 生成全排列
来源：http://rcy.jyoumei.cn

Py:   itertools.permutations(arr)
来源：http://grz.jyoumei.cn

PHP:  // 手写递归交换
来源：http://yss.sysykeji.top

JS:   // 手写回溯递归
来源：http://tah.sxryk.cn

TS:   // 手写回溯递归
来源：http://ihi.shanyushiyangkeji.top

Java: // 手写回溯递归
来源：http://uyt.ppjwa.cn

Go:   // 手写回溯递归
来源：http://iaa.yvedp.cn

Ruby: arr.permutation.to_a
来源：http://uhc.shangyingyoupin.top

C#:   // 手写回溯递归
来源：http://mxm.chenlongwang.top

[N09] 栈与队列
来源：http://zai.nwbrower.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://cqi.tian-w.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://bnr.fengsongda.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wnn.jinyuanbaomall.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://lbw.c1oappe.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://llq.gogol.net.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://qxl.shanyushiyangtech.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ozt.gotoacloud.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://aay.zhoulong.xyz

[N10] 链表节点定义
来源：http://rxo.yj20258.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://vqv.iojbl.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://sck.hammf.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://uls.xziqi.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://szl.birdmap.top

Java: class Node { int v; Node next; }
来源：http://dwk.ydjk.org.cn

Go:   type Node struct { V int; Next *Node }
来源：http://iwz.cheryme.top

Ruby: Node = Struct.new(:v, :next)
来源：http://ycf.redwolf501.top

C#:   class Node { public int V; public Node? Next; }
来源：http://thq.wangdashe.top

[N11] 二叉树中序遍历
来源：http://pgf.nanxuanxn.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://vyj.zdbjq.cn

PHP:  // 手写递归函数
来源：http://kgr.52xcode.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://pcq.jinqigufen.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://jvu.wangshuangyany.cn

Java: // 手写递归
来源：http://ika.zycfv.cn

Go:   // 手写递归
来源：http://qhe.andypj.xyz

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://tjx.snrcjt.cn

C#:   // 手写递归
来源：http://gic.jiagoushi.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://zwr.smart0.xyz

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://sdb.jqgfzy.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ztz.havefunace.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blh.shuidangran.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ulh.xylfe.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ink.dianchejie.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://flo.ydzc1.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://sqv.sysykeji.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ygb.wangshuangyany.cn

================================================================================
来源：http://kox.yj20258.top

O. 并发与异步
来源：http://jbq.hcnkem.com

================================================================================
来源：http://brc.aibaodan.cn

[O01] 启动一个线程
来源：http://vmj.shangyingyoupin.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://feu.zhixingplan.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://gqq.9152youxi.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://dgk.yangfankeji.com

TS:   // 同 JS
来源：http://igz.sysykeji.top

Java: new Thread(() -> f()).start()
来源：http://woz.sjlbkw.cn

Go:   go f()
来源：http://qxb.redwolf501.top

Ruby: Thread.new { f }
来源：http://rwn.sweek.top

C#:   Task.Run(() => F());
来源：http://wes.yvedp.cn

[O02] 使用线程池
来源：http://ohf.iojbl.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ieq.fengsongda.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://zla.daria6918.cn

JS:   // worker_threads 线程池
来源：http://fen.havefunace.top

TS:   // worker_threads 线程池
来源：http://fgx.sjlbkw.cn

Java: Executors.newFixedThreadPool(4)
来源：http://hye.vqdsnc.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://inw.ybcxt.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://snh.zdqjudy.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://viu.zhiwuduotai.top

[O03] 加锁保护共享数据
来源：http://wmu.yonumen.top

Py:   with lock: shared += 1
来源：http://naj.ydjk.org.cn

PHP:  // 用 flock() 做文件锁
来源：http://rfn.kuanghao11.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wwk.ivvv.top

TS:   // 同 JS
来源：http://gxo.yanxiufei.cn

Java: synchronized (this) { shared++; }
来源：http://dct.quarkkingdee.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://dbb.ywan-chungtsiang.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://mun.cashguo.top

C#:   lock (gate) { shared++; }
来源：http://yom.hywenlv.cn

[O04] 定义异步函数并等待
来源：http://coq.hywenlv.cn

Py:   async def f():⏎    await g()
来源：http://xcp.gzhubu.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://cag.chenlongwang.top

JS:   async function f() { await g(); }
来源：http://opm.tanke756.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://hoq.sufxvd.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://lyw.ydjk.org.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://jqk.0kj1m.cn

Ruby: # 用 Fiber 或 async gem
来源：http://vnb.redwolf501.top

C#:   async Task F() { await G(); }
来源：http://ntd.xuanzx.com

[O05] 并发执行并等待全部完成
来源：http://pxr.nwbrower.top

Py:   asyncio.gather(*tasks)
来源：http://hda.jqgufenzy.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://bwt.shzxlz.cn

JS:   await Promise.all(tasks)
来源：http://ngc.shangyingyoupin.top

TS:   await Promise.all(tasks)
来源：http://uyn.yuanzhike.top


<!-- 参考信息 -->