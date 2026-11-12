代发 wailian999

L. 网络请求
来源：http://wdw.meibo888.top

================================================================================
来源：http://ejk.cashguo.top

[L01] 发送 GET 请求
来源：http://rwg.meibo888.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ajg.fengsongda.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hvq.nanxinkj.top

JS:   await fetch(url)
来源：http://ryt.yfazqb.com

TS:   await fetch(url)
来源：http://msb.jlsjyb.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://uoz.xziqi.cn

Go:   resp, err := http.Get(url)
来源：http://ppb.iojbl.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://wqr.xuetiantiany.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://khc.fktsv.cn

[L02] 发送 POST JSON
来源：http://cxx.sufxvd.cn

Py:   requests.post(url, json={"a": 1})
来源：http://uuw.yvedp.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://tpi.yj202588.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hpx.sxryk.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://trx.yongpay.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://zpb.hnqzz.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ryv.yanxiufei.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://pbx.cdnleiting.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://bfu.shanyushiyangtech.top

[L03] 设置自定义请求头
来源：http://ony.tianlin.xyz

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://xmw.zhongyouzk.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://osr.hammf.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://foa.shanyushiyangkeji.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://dfn.tianlin.xyz

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://llz.hfpthk.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://qga.chenjidiqi.icu

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ngs.jyoumei.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://pjx.snrcjt.cn

[L04] 设置超时
来源：http://pqu.gotoacloud.top

Py:   requests.get(url, timeout=5)
来源：http://rhm.yvedp.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hmw.tianlin.xyz

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://jcq.zhijiandao.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://yyf.ivvv.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mjv.zhijiandao.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://gcg.epnwcf.com

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://pco.iojbl.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://baa.jinyuanbaomall.cn

[L05] 上传文件（multipart）
来源：http://nxc.fktsv.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://azb.chenlongwang.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://tpo.ehwqpu.com

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://jqw.hnxiangtu.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://qhb.jiagoushi.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://rda.yvedp.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://iqk.aibaodan.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://imf.gotoacloud.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://xao.shuidangran.top

[L06] 解析响应为 JSON
来源：http://krz.guowangkeji.top

Py:   resp.json()
来源：http://wsz.xingfuxueyuan.xyz

PHP:  json_decode($body, true);
来源：http://qjh.zhengqikj.top

JS:   await resp.json()
来源：http://lsk.wangshuangyany.cn

TS:   await resp.json()
来源：http://bab.ydjk.org.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://adh.gzhubu.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://xcr.cucudq.cn

Ruby: JSON.parse(resp.body)
来源：http://psl.gaohongyu789.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://eqn.yuanzhike.top

[L07] 处理 HTTP 状态码
来源：http://dwr.yonumen.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://xrn.yfazqb.com

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mfn.yongpay.top

JS:   resp.ok;  resp.status
来源：http://rlo.jinyuanbaomall.cn

TS:   resp.ok;  resp.status
来源：http://hvm.smart0.xyz

Java: resp.statusCode()
来源：http://eaj.nwbrower.top

Go:   resp.StatusCode
来源：http://hcv.birdmap.top

Ruby: resp.code.to_i
来源：http://nyh.hysaishi.cn

C#:   (int)resp.StatusCode
来源：http://kky.jinqigfzy.top

[L08] 并发请求多个地址
来源：http://hkr.bbcook.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://kln.fehbvm.com

PHP:  curl_multi_init() 系列
来源：http://vkn.vqdsnc.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://jwe.feifeiyinyue.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://zud.wangshuangyany.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mfz.guannengcc.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://olz.bbcook.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://cbl.zhixingplan.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://bxi.redwolf501.top

================================================================================
来源：http://krv.xuanzx.com

M. 命令行 / 进程 / 环境
来源：http://xcj.jianghu66.top

================================================================================
来源：http://hmk.zdqjudy.top

[M01] 读取命令行参数
来源：http://pho.wangdashe.top

Py:   sys.argv[1:]
来源：http://iki.hywenlv.cn

PHP:  $argv;  $argc;
来源：http://tqc.gogol.net.cn

JS:   process.argv.slice(2)
来源：http://dlx.zycfv.cn

TS:   process.argv.slice(2)
来源：http://hnt.feifeiyinyue.top

Java: args 数组（main 方法参数）
来源：http://seq.52xcode.cn

Go:   os.Args[1:]
来源：http://pjy.gzhubu.top

Ruby: ARGV
来源：http://owg.chenzaomai.com

C#:   args 数组（Main 方法参数）
来源：http://qrq.yfazqb.com

[M02] 读取环境变量
来源：http://ywu.sysykeji.top

Py:   os.environ.get("HOME")
来源：http://mdv.zhixingplan.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://vds.jlsjyb.cn

JS:   process.env.HOME
来源：http://pub.gotoacloud.top

TS:   process.env.HOME
来源：http://vew.daxiang520.top

Java: System.getenv("HOME")
来源：http://jkq.hysaishi.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://rhi.guowangkeji.top

Ruby: ENV["HOME"]
来源：http://ake.iojbl.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ucv.zhengqikj.top

[M03] 执行外部命令
来源：http://gnq.cdnleiting.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://swd.cqqwz.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://duy.nanxinkj.top

JS:   child_process.execSync("ls -l").toString()
来源：http://dhr.jqgufenzy.top

TS:   child_process.execSync("ls -l").toString()
来源：http://fox.cashguo.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://gyv.hongshengwenyu.top

Go:   exec.Command("ls", "-l").Output()
来源：http://ibn.jqgfzy.top

Ruby: system("ls -l");  `ls -l`
来源：http://acz.fzhhl.top

C#:   Process.Start("ls", "-l");
来源：http://ukr.haohaochexian.top

[M04] 获取当前工作目录
来源：http://tjh.uphjek.com

Py:   os.getcwd()
来源：http://caf.shanyushiyangkeji.top

PHP:  getcwd();
来源：http://psi.316326.xyz

JS:   process.cwd()
来源：http://ega.0kj1m.cn

TS:   process.cwd()
来源：http://kfd.jyoumei.cn

Java: Path.of("").toAbsolutePath()
来源：http://mfz.jqgfzy.top

Go:   os.Getwd()
来源：http://nqf.nanxuanxn.top

Ruby: Dir.pwd
来源：http://hup.gotoacloud.top

C#:   Directory.GetCurrentDirectory()
来源：http://pbs.fengsongda.top

[M05] 设置退出码
来源：http://zbo.9152youxi.cn

Py:   sys.exit(1)
来源：http://xzi.hnxiangtu.top

PHP:  exit(1);
来源：http://xga.cashguo.top

JS:   process.exit(1)
来源：http://pmc.guowangkeji.top

TS:   process.exit(1)
来源：http://udv.guannengcc.top

Java: System.exit(1)
来源：http://fiw.gogol.net.cn

Go:   os.Exit(1)
来源：http://nva.xingfuxueyuan.xyz

Ruby: exit 1
来源：http://rlg.hfpthk.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wpn.wangshuangyany.cn

[M06] 向标准错误输出
来源：http://mrd.aibaodan.cn

Py:   print("err", file=sys.stderr)
来源：http://xuk.9152youxi.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://mjg.shzxlz.cn

JS:   console.error("err")
来源：http://knp.hnxiangtu.top

TS:   console.error("err")
来源：http://lcl.zdqjudy.top

Java: System.err.println("err")
来源：http://sbl.redwolf501.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://frl.tian-w.cn

Ruby: warn "err"
来源：http://bkp.fehbvm.com

C#:   Console.Error.WriteLine("err")
来源：http://dkp.gogol.net.cn

[M07] 判断是否为主入口
来源：http://anp.nwbrower.top

Py:   if __name__ == "__main__":
来源：http://bgi.zycfv.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://iuq.aibaodan.cn

JS:   require.main === module
来源：http://ldg.ctjpmb.com

TS:   require.main === module
来源：http://gyb.gzhubu.top

Java: public static void main(String[] args)
来源：http://zus.quarkkingdee.top

Go:   func main()
来源：http://ocr.iojbl.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://yqz.cqqwz.cn

C#:   static void Main(string[] args)
来源：http://hxe.cheryme.top

[M08] 获取系统与运行时信息
来源：http://dem.ctjpmb.com

Py:   platform.system();  platform.python_version()
来源：http://xsk.ivvv.top

PHP:  PHP_OS;  phpversion();
来源：http://gbz.uphjek.com

JS:   process.platform;  process.version
来源：http://sfg.hammf.cn

TS:   process.platform;  process.version
来源：http://mui.cucudq.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://slo.fktsv.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://bdx.bjfxy.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://fen.yfazqb.com

C#:   Environment.OSVersion;  Environment.Version
来源：http://xud.yueranfly.top

================================================================================
来源：http://ngm.birdmap.top

N. 数据结构与算法
来源：http://dpw.ywan-chungtsiang.top

================================================================================
来源：http://rih.jinqigufen.top

[N01] 二分查找（有序数组）
来源：http://ldv.guannengcc.top

Py:   bisect.bisect_left(arr, x)
来源：http://pfh.yuanzhike.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://nag.smart0.xyz

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mgn.hnqzz.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ycq.c1oappe.top

Java: Arrays.binarySearch(arr, x)
来源：http://yyu.jianghu66.top

Go:   sort.SearchInts(arr, x)
来源：http://tlo.hongshengwenyu.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://azy.iojbl.cn

C#:   Array.BinarySearch(arr, x)
来源：http://mlv.bbcook.cn

[N02] 排序（工程实践用内置实现）
来源：http://dht.gogol.net.cn

Py:   sorted(arr);  arr.sort()
来源：http://htq.chenzaomai.com

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ccl.hysaishi.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://myt.guowangkeji.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://exv.hysaishi.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://gjj.wangshuangyany.cn

Go:   slices.Sort(arr)
来源：http://bxd.kuanghao11.cn

Ruby: arr.sort
来源：http://dva.gotoacloud.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://ewh.yj20258888.top

[N03] 快速排序（分治示例）
来源：http://enz.cashguo.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://vdk.xylfe.cn

PHP:  // 递归实现，或用 usort
来源：http://ory.uphjek.com

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://pkc.hfpthk.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://rwa.zhiwuduotai.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://zzh.jinghuilouyu.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://trz.yonumen.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ydz.jiagoushi.top

C#:   // 手写递归，或 Array.Sort
来源：http://aqn.zhijiandao.cn

[N04] 斐波那契数列
来源：http://dhg.gaohongyu789.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://jrr.shanyushiyangtech.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ojf.xuanzx.com

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://rzr.316326.xyz

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://urb.feifeiyinyue.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://dxi.haohaochexian.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ufi.52xcode.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://rpo.gogol.net.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://qct.zhongyouzk.top

[N05] 最大公约数
来源：http://ejp.daria6918.cn

Py:   math.gcd(a, b)
来源：http://yje.tianlin.xyz

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://fag.zhaomingkeji.xyz

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ycd.chenzaomai.com

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://orr.fanxiaobao.xyz

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://oyx.cucudq.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://tpz.zdbjq.cn

Ruby: a.gcd(b)
来源：http://qhj.hesvh.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wyf.nwbrower.top

[N06] 判断回文字符串
来源：http://hsa.pycfn.com

Py:   s == s[::-1]
来源：http://zod.quarkkingdee.top

PHP:  $s === strrev($s);
来源：http://mso.pengpengdd.cyou

JS:   s === [...s].reverse().join("")
来源：http://pct.pengpengdd.cyou

TS:   s === [...s].reverse().join("")
来源：http://lnp.ydjk.org.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://shw.yj20258888.top

Go:   // 双指针从两端比较
来源：http://awe.yvedp.cn

Ruby: s == s.reverse
来源：http://sfw.yj202588.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://wje.cdnleiting.top

[N07] 两数之和（返回下标）
来源：http://ndr.hnxiangtu.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mrt.aibaodan.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://lwz.jianghu66.top

JS:   // 手写 Map：map.set(v, i)
来源：http://tyr.bbcook.cn

TS:   // 手写 Map<string, number>
来源：http://yej.shanyushiyangkeji.top

Java: // 手写 HashMap
来源：http://szx.andypj.xyz

Go:   // 手写 map[int]int
来源：http://igk.xuetiantiany.cn

Ruby: // 手写 Hash
来源：http://zgn.gaohongyu789.top

C#:   // 手写 Dictionary<int, int>
来源：http://fmg.hysaishi.cn

[N08] 生成全排列
来源：http://ktz.dianchejie.cn

Py:   itertools.permutations(arr)
来源：http://izy.xingfuxueyuan.xyz

PHP:  // 手写递归交换
来源：http://ivp.chenzaomai.com

JS:   // 手写回溯递归
来源：http://xtl.vqdsnc.cn

TS:   // 手写回溯递归
来源：http://adl.cashguo.top

Java: // 手写回溯递归
来源：http://ohp.yuxming.cn

Go:   // 手写回溯递归
来源：http://rmv.ywan-chungtsiang.top

Ruby: arr.permutation.to_a
来源：http://mjw.zhoulong.xyz

C#:   // 手写回溯递归
来源：http://qky.yuanzhike.top

[N09] 栈与队列
来源：http://drr.ivvv.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://xnt.yuanzhike.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://cte.jlsjyb.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://win.kuanghao11.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://kea.cdnleiting.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ibr.yj20258888.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://kln.hesvh.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://awf.bjfxy.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wuy.birdmap.top

[N10] 链表节点定义
来源：http://vsw.zycfv.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://rvv.yonumen.top

PHP:  class Node { public $v; public $next = null; }
来源：http://nkh.ivvv.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://zax.yongpay.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://afn.jqgufenzy.top

Java: class Node { int v; Node next; }
来源：http://kvx.yongpay.top

Go:   type Node struct { V int; Next *Node }
来源：http://qse.jyoumei.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://qjq.dashuyun.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://ujs.jinqigufen.top

[N11] 二叉树中序遍历
来源：http://dgs.xinyue.icu

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://tkx.hfpthk.cn

PHP:  // 手写递归函数
来源：http://yrx.cqqwz.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://dyh.smart0.xyz

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://iaf.sysykeji.top

Java: // 手写递归
来源：http://gfk.guannengcc.top

Go:   // 手写递归
来源：http://fbn.nanxuanxn.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://kgf.guowangkeji.top

C#:   // 手写递归
来源：http://see.wangdashe.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hwz.yj20258.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ugu.yfazqb.com

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://cyk.xuetiantiany.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://jip.xinyue.icu

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://aqr.zhixingplan.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://otn.ppjwa.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://bem.jinyuanbaomall.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://rfk.0kj1m.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ugc.sysykeji.top

================================================================================
来源：http://arr.haohaochexian.top

O. 并发与异步
来源：http://dza.yangfankeji.com

================================================================================
来源：http://kiz.shuidangran.top

[O01] 启动一个线程
来源：http://ixh.jianghu66.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://tns.redwolf501.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mrw.pengpengdd.cyou

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://qyy.nanxuanxn.top

TS:   // 同 JS
来源：http://cho.iojbl.cn

Java: new Thread(() -> f()).start()
来源：http://hvu.shuidangran.top

Go:   go f()
来源：http://haq.hcnkem.com

Ruby: Thread.new { f }
来源：http://uyt.gogol.net.cn

C#:   Task.Run(() => F());
来源：http://eth.yanxiufei.cn

[O02] 使用线程池
来源：http://gew.pycfn.com

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mzs.svipenyu.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://dvw.wangshuangyany.cn

JS:   // worker_threads 线程池
来源：http://gge.hysaishi.cn

TS:   // worker_threads 线程池
来源：http://qzw.nwbrower.top

Java: Executors.newFixedThreadPool(4)
来源：http://peu.ywan-chungtsiang.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://vwf.jiagoushi.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://pxi.yongpay.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://doj.daxiang520.top

[O03] 加锁保护共享数据
来源：http://lsb.ydjk.org.cn

Py:   with lock: shared += 1
来源：http://zkm.snrcjt.cn

PHP:  // 用 flock() 做文件锁
来源：http://glw.yanxiufei.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://iwj.tian-w.cn

TS:   // 同 JS
来源：http://crr.yanxiufei.cn

Java: synchronized (this) { shared++; }
来源：http://qyd.redwolf501.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://gsi.chenzaomai.com

Ruby: mutex.synchronize { shared += 1 }
来源：http://dnu.hysaishi.cn

C#:   lock (gate) { shared++; }
来源：http://nfn.bbcook.cn

[O04] 定义异步函数并等待
来源：http://mef.zhixingplan.top

Py:   async def f():⏎    await g()
来源：http://qbc.ivvv.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://tnq.daxiang520.top

JS:   async function f() { await g(); }
来源：http://zmd.jinyuanbaomall.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://asv.fktsv.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://clc.316326.xyz

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ydz.zhixingplan.top

Ruby: # 用 Fiber 或 async gem
来源：http://hgs.sweek.top

C#:   async Task F() { await G(); }
来源：http://xfd.c1oappe.top

[O05] 并发执行并等待全部完成
来源：http://yrq.xuetiantiany.cn


<!-- 参考信息 -->