代发 wailian999

L. 网络请求
来源：http://xkd.sysykeji.top

================================================================================
来源：http://duf.hammf.cn

[L01] 发送 GET 请求
来源：http://lmv.hywenlv.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wzv.pycfn.com

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://kqq.tarul.cn

JS:   await fetch(url)
来源：http://egd.birdmap.top

TS:   await fetch(url)
来源：http://brm.yvedp.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://kko.wangdashe.top

Go:   resp, err := http.Get(url)
来源：http://bpo.jinghuilouyu.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://qem.yangfankeji.com

C#:   await new HttpClient().GetStringAsync(url)
来源：http://sre.hesvh.cn

[L02] 发送 POST JSON
来源：http://sts.daxiang520.top

Py:   requests.post(url, json={"a": 1})
来源：http://xvp.yuxming.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ygp.hywenlv.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://xad.yuxming.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ouw.jianghu66.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wsi.yj202588.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://evz.chenjidiqi.icu

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://rlr.gzhubu.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://kxb.fanxiaobao.xyz

[L03] 设置自定义请求头
来源：http://fqp.xingfuxueyuan.xyz

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://iis.ydzc1.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mys.52xcode.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://rub.jyoumei.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://xcc.gotoacloud.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ama.birdmap.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://uju.zhengqikj.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://qby.jiagoushi.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://odh.gogol.net.cn

[L04] 设置超时
来源：http://eco.hesvh.cn

Py:   requests.get(url, timeout=5)
来源：http://fcm.hongshengwenyu.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://atp.sufxvd.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://otq.wangdashe.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://kww.redwolf501.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://pva.ehwqpu.com

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://rvs.guowangkeji.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://pch.dianchejie.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://zky.ybcxt.top

[L05] 上传文件（multipart）
来源：http://ege.zdbjq.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://lkn.ctjpmb.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://vjs.jinghuilouyu.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mip.chenjidiqi.icu

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://zfv.meibo888.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://xlk.jlsjyb.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://rzm.dashuyun.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://gha.jianghu66.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://yuo.zhongyouzk.top

[L06] 解析响应为 JSON
来源：http://bfq.snrcjt.cn

Py:   resp.json()
来源：http://qcr.shanyushiyangkeji.top

PHP:  json_decode($body, true);
来源：http://rux.hfpthk.cn

JS:   await resp.json()
来源：http://qbf.ehwqpu.com

TS:   await resp.json()
来源：http://aiw.hammf.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hau.pengpengdd.cyou

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ynv.sysykeji.top

Ruby: JSON.parse(resp.body)
来源：http://ohc.meibo888.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ixr.ywan-chungtsiang.top

[L07] 处理 HTTP 状态码
来源：http://kzo.fzhhl.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://lks.hywenlv.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://pfc.hnqzz.top

JS:   resp.ok;  resp.status
来源：http://wwa.yfazqb.com

TS:   resp.ok;  resp.status
来源：http://wze.cheryme.top

Java: resp.statusCode()
来源：http://dep.ppjwa.cn

Go:   resp.StatusCode
来源：http://cpu.yj20258888.top

Ruby: resp.code.to_i
来源：http://ufo.zdbjq.cn

C#:   (int)resp.StatusCode
来源：http://wxi.gogol.net.cn

[L08] 并发请求多个地址
来源：http://apr.nwbrower.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://pst.gotoacloud.top

PHP:  curl_multi_init() 系列
来源：http://bda.cqqwz.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://qkx.zhixingplan.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://cwc.cucudq.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://rbk.chenzaomai.com

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://qqd.xuanzx.com

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mmv.ehwqpu.com

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ngt.ybcxt.top

================================================================================
来源：http://ied.fehbvm.com

M. 命令行 / 进程 / 环境
来源：http://cow.fzhhl.top

================================================================================
来源：http://dzt.hysaishi.cn

[M01] 读取命令行参数
来源：http://irk.birdmap.top

Py:   sys.argv[1:]
来源：http://bqf.aibaodan.cn

PHP:  $argv;  $argc;
来源：http://gla.jqgfzy.top

JS:   process.argv.slice(2)
来源：http://fza.zycfv.cn

TS:   process.argv.slice(2)
来源：http://fiq.nanxinkj.top

Java: args 数组（main 方法参数）
来源：http://sxw.ydzc1.top

Go:   os.Args[1:]
来源：http://xsn.fanxiaobao.xyz

Ruby: ARGV
来源：http://zjv.ydjk.org.cn

C#:   args 数组（Main 方法参数）
来源：http://fvm.hysaishi.cn

[M02] 读取环境变量
来源：http://qav.ctjpmb.com

Py:   os.environ.get("HOME")
来源：http://usi.yj202588.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://qbb.zhixingplan.top

JS:   process.env.HOME
来源：http://gzq.yangfankeji.com

TS:   process.env.HOME
来源：http://rli.hammf.cn

Java: System.getenv("HOME")
来源：http://jso.nwbrower.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://xmx.ydzc1.top

Ruby: ENV["HOME"]
来源：http://std.ywan-chungtsiang.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://aad.shanyushiyangkeji.top

[M03] 执行外部命令
来源：http://pcf.fengsongda.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://rdc.ydzc1.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hnx.gzhubu.top

JS:   child_process.execSync("ls -l").toString()
来源：http://rwt.sweek.top

TS:   child_process.execSync("ls -l").toString()
来源：http://ukj.sjlbkw.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://anq.nwbrower.top

Go:   exec.Command("ls", "-l").Output()
来源：http://gii.tanke756.top

Ruby: system("ls -l");  `ls -l`
来源：http://ore.nanxuanxn.top

C#:   Process.Start("ls", "-l");
来源：http://omy.yanxiufei.cn

[M04] 获取当前工作目录
来源：http://flg.zdbjq.cn

Py:   os.getcwd()
来源：http://pvq.zhixingplan.top

PHP:  getcwd();
来源：http://atj.jinghuilouyu.cn

JS:   process.cwd()
来源：http://pmx.guannengcc.top

TS:   process.cwd()
来源：http://cro.ehwqpu.com

Java: Path.of("").toAbsolutePath()
来源：http://jkz.bjfxy.top

Go:   os.Getwd()
来源：http://vaw.yangfankeji.com

Ruby: Dir.pwd
来源：http://xor.jinqigufen.top

C#:   Directory.GetCurrentDirectory()
来源：http://swa.shanyushiyangtech.top

[M05] 设置退出码
来源：http://ueq.andypj.xyz

Py:   sys.exit(1)
来源：http://ksu.cdnleiting.top

PHP:  exit(1);
来源：http://aje.kuanghao11.cn

JS:   process.exit(1)
来源：http://nrj.aizwys.cn

TS:   process.exit(1)
来源：http://dnu.sxryk.cn

Java: System.exit(1)
来源：http://ioo.fengsongda.top

Go:   os.Exit(1)
来源：http://exy.jqgufenzy.top

Ruby: exit 1
来源：http://zmq.gaohongyu789.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://xho.hywenlv.cn

[M06] 向标准错误输出
来源：http://rut.fzhhl.top

Py:   print("err", file=sys.stderr)
来源：http://ogw.yj20258.top

PHP:  fwrite(STDERR, "err\n");
来源：http://cea.ivvv.top

JS:   console.error("err")
来源：http://uzi.quarkkingdee.top

TS:   console.error("err")
来源：http://rzn.hongshengwenyu.top

Java: System.err.println("err")
来源：http://cel.dianchejie.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://fdg.hcnkem.com

Ruby: warn "err"
来源：http://hhx.gaohongyu789.top

C#:   Console.Error.WriteLine("err")
来源：http://btk.shuidangran.top

[M07] 判断是否为主入口
来源：http://iym.pengpengdd.cyou

Py:   if __name__ == "__main__":
来源：http://onw.snrcjt.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ehc.sysykeji.top

JS:   require.main === module
来源：http://pbk.316326.xyz

TS:   require.main === module
来源：http://dor.gzhubu.top

Java: public static void main(String[] args)
来源：http://eev.cdnleiting.top

Go:   func main()
来源：http://wjy.fengsongda.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://sdc.sjlbkw.cn

C#:   static void Main(string[] args)
来源：http://buc.pengpengdd.cyou

[M08] 获取系统与运行时信息
来源：http://myn.gotoacloud.top

Py:   platform.system();  platform.python_version()
来源：http://rho.yj202588.top

PHP:  PHP_OS;  phpversion();
来源：http://qss.smart0.xyz

JS:   process.platform;  process.version
来源：http://jad.yueranfly.top

TS:   process.platform;  process.version
来源：http://adw.andypj.xyz

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://fnc.sxryk.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://vng.9152youxi.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://oxh.jinghuilouyu.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://whi.dashuyun.cn

================================================================================
来源：http://hjs.ybcxt.top

N. 数据结构与算法
来源：http://hpr.nwbrower.top

================================================================================
来源：http://wzb.jianghu66.top

[N01] 二分查找（有序数组）
来源：http://lhw.meibo888.top

Py:   bisect.bisect_left(arr, x)
来源：http://qxk.hnqzz.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://sse.zhixingplan.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://jov.feifeiyinyue.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://bus.jqgufenzy.top

Java: Arrays.binarySearch(arr, x)
来源：http://gcb.bjfxy.top

Go:   sort.SearchInts(arr, x)
来源：http://sjv.redwolf501.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://bri.zycfv.cn

C#:   Array.BinarySearch(arr, x)
来源：http://hdp.meibo888.top

[N02] 排序（工程实践用内置实现）
来源：http://wop.havefunace.top

Py:   sorted(arr);  arr.sort()
来源：http://ahz.zhengqikj.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mlv.jlsjyb.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://rcg.aizwys.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://trj.yj202588.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://svb.zdqjudy.top

Go:   slices.Sort(arr)
来源：http://pre.aizwys.cn

Ruby: arr.sort
来源：http://dkg.cheryme.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://ara.hnqzz.top

[N03] 快速排序（分治示例）
来源：http://gai.shanyushiyangtech.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://dcl.xziqi.cn

PHP:  // 递归实现，或用 usort
来源：http://jgl.ctjpmb.com

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://upk.jinqigufen.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://myi.ydjk.org.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://exs.pycfn.com

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://gcr.xingfuxueyuan.xyz

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://fvr.aizwys.cn

C#:   // 手写递归，或 Array.Sort
来源：http://clk.gogol.net.cn

[N04] 斐波那契数列
来源：http://ssd.zhixingplan.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://xrw.tianlin.xyz

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://iis.shangyingyoupin.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://psn.kuanghao11.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://rnj.hfpthk.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://vwv.cucudq.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://qph.yueranfly.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://lry.fehbvm.com

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://kpn.cashguo.top

[N05] 最大公约数
来源：http://izz.tianlin.xyz

Py:   math.gcd(a, b)
来源：http://zbh.fengsongda.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ecv.gzhubu.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://jan.jianghu66.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://vqx.xinyue.icu

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mas.jlsjyb.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ukc.hywenlv.cn

Ruby: a.gcd(b)
来源：http://rhp.zhixingplan.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://gut.daxiang520.top

[N06] 判断回文字符串
来源：http://zet.andypj.xyz

Py:   s == s[::-1]
来源：http://pae.jinqigufen.top

PHP:  $s === strrev($s);
来源：http://qyv.tarul.cn

JS:   s === [...s].reverse().join("")
来源：http://hko.zhijiandao.cn

TS:   s === [...s].reverse().join("")
来源：http://umo.xinyue.icu

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://yry.fehbvm.com

Go:   // 双指针从两端比较
来源：http://gar.gotoacloud.top

Ruby: s == s.reverse
来源：http://hqn.dianchejie.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://scd.feifeiyinyue.top

[N07] 两数之和（返回下标）
来源：http://ptm.cdnleiting.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://uwe.yangfankeji.com

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://rjr.sjlbkw.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://xus.bjfxy.top

TS:   // 手写 Map<string, number>
来源：http://xya.0kj1m.cn

Java: // 手写 HashMap
来源：http://gve.daxiang520.top

Go:   // 手写 map[int]int
来源：http://vxh.ydzc1.top

Ruby: // 手写 Hash
来源：http://zkt.cheryme.top

C#:   // 手写 Dictionary<int, int>
来源：http://tcw.kuanghao11.cn

[N08] 生成全排列
来源：http://fph.shanyushiyangtech.top

Py:   itertools.permutations(arr)
来源：http://ewz.316326.xyz

PHP:  // 手写递归交换
来源：http://gik.xinyue.icu

JS:   // 手写回溯递归
来源：http://ucv.shuidangran.top

TS:   // 手写回溯递归
来源：http://sbl.yj20258.top

Java: // 手写回溯递归
来源：http://ogn.nwbrower.top

Go:   // 手写回溯递归
来源：http://hjh.316326.xyz

Ruby: arr.permutation.to_a
来源：http://hhi.gogol.net.cn

C#:   // 手写回溯递归
来源：http://itx.cqqwz.cn

[N09] 栈与队列
来源：http://oek.aibaodan.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://beb.redwolf501.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://eqt.wangshuangyany.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://uea.nanxuanxn.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://nni.guannengcc.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ibn.yuxming.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://sbl.sweek.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://kkc.shanyushiyangtech.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://fex.birdmap.top

[N10] 链表节点定义
来源：http://kmc.jlsjyb.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://dgn.ppjwa.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://cak.yfazqb.com

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mzd.tianlin.xyz

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ozh.ydzc1.top

Java: class Node { int v; Node next; }
来源：http://qtp.jqgufenzy.top

Go:   type Node struct { V int; Next *Node }
来源：http://jnk.yangfankeji.com

Ruby: Node = Struct.new(:v, :next)
来源：http://wyi.0kj1m.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://adm.bjfxy.top

[N11] 二叉树中序遍历
来源：http://fdf.redwolf501.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://dqh.chenlongwang.top

PHP:  // 手写递归函数
来源：http://ahx.bbcook.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://gqp.guannengcc.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wux.jiagoushi.top

Java: // 手写递归
来源：http://qij.yueranfly.top

Go:   // 手写递归
来源：http://agn.meibo888.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://btr.hcnkem.com

C#:   // 手写递归
来源：http://bxq.hesvh.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://vyw.iojbl.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ebt.cashguo.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://vfb.316326.xyz

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ddn.sjlbkw.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://otb.gzhubu.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ugm.epnwcf.com

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://qei.sysykeji.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://twq.sjlbkw.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://pyj.chenzaomai.com

================================================================================
来源：http://aem.chenlongwang.top

O. 并发与异步
来源：http://krq.cheryme.top

================================================================================
来源：http://yza.tian-w.cn

[O01] 启动一个线程
来源：http://kzc.yvedp.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://vbu.shangyingyoupin.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://gwf.9152youxi.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://kgb.bbcook.cn

TS:   // 同 JS
来源：http://nej.9152youxi.cn

Java: new Thread(() -> f()).start()
来源：http://wot.snrcjt.cn

Go:   go f()
来源：http://wqd.yj20258888.top

Ruby: Thread.new { f }
来源：http://sqm.ehwqpu.com

C#:   Task.Run(() => F());
来源：http://ped.ppjwa.cn

[O02] 使用线程池
来源：http://ozz.jyoumei.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://fex.daria6918.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mid.fehbvm.com

JS:   // worker_threads 线程池
来源：http://mmr.xingfuxueyuan.xyz

TS:   // worker_threads 线程池
来源：http://cif.sweek.top

Java: Executors.newFixedThreadPool(4)
来源：http://eyh.nanxuanxn.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://xpf.nanxinkj.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://xrf.ctjpmb.com

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://gaz.316326.xyz

[O03] 加锁保护共享数据
来源：http://thr.hcnkem.com

Py:   with lock: shared += 1
来源：http://xom.52xcode.cn

PHP:  // 用 flock() 做文件锁
来源：http://frz.xylfe.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://eqr.yj202588.top

TS:   // 同 JS
来源：http://lsh.shangyingyoupin.top

Java: synchronized (this) { shared++; }
来源：http://tmh.yueranfly.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://vvq.xylfe.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://tpg.yueranfly.top

C#:   lock (gate) { shared++; }
来源：http://voe.yonumen.top

[O04] 定义异步函数并等待
来源：http://avi.ydzc1.top

Py:   async def f():⏎    await g()
来源：http://udw.andypj.xyz

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://nmq.tarul.cn

JS:   async function f() { await g(); }
来源：http://ypy.guowangkeji.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://kde.dianchejie.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://yub.ydzc1.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://kad.meibo888.top

Ruby: # 用 Fiber 或 async gem
来源：http://koe.svipenyu.cn

C#:   async Task F() { await G(); }
来源：http://qvz.yongpay.top

[O05] 并发执行并等待全部完成
来源：http://oyc.birdmap.top


<!-- 参考信息 -->