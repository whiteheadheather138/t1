代发 wailian999

Go:   encoding/gob
来源：http://ebl.yangfankeji.com

Ruby: Marshal.dump(obj)
来源：http://qvu.zdqjudy.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ypy.nanxinkj.top

================================================================================
来源：http://rwx.quarkkingdee.top

L. 网络请求
来源：http://pox.ctjpmb.com

================================================================================
来源：http://mvf.jyoumei.cn

[L01] 发送 GET 请求
来源：http://xvc.yonumen.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://gsi.yj20258.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://gup.zhongyouzk.top

JS:   await fetch(url)
来源：http://pbp.52xcode.cn

TS:   await fetch(url)
来源：http://ops.guannengcc.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mhy.nanxuanxn.top

Go:   resp, err := http.Get(url)
来源：http://lzq.fehbvm.com

Ruby: Net::HTTP.get(URI(url))
来源：http://bed.chenzaomai.com

C#:   await new HttpClient().GetStringAsync(url)
来源：http://etp.daxiang520.top

[L02] 发送 POST JSON
来源：http://ylz.daria6918.cn

Py:   requests.post(url, json={"a": 1})
来源：http://ozn.jlsjyb.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ctn.hongshengwenyu.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://feo.yuanzhike.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://yly.epnwcf.com

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://xsr.316326.xyz

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://pxj.snrcjt.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://qus.yongpay.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://qgh.daxiang520.top

[L03] 设置自定义请求头
来源：http://zlt.zycfv.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://rok.sjlbkw.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://bsl.xziqi.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://tbc.jinqigfzy.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://eii.dashuyun.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://nop.zhixingplan.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ooh.cdnleiting.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://lwr.tarul.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://osy.jyoumei.cn

[L04] 设置超时
来源：http://iyk.chenlongwang.top

Py:   requests.get(url, timeout=5)
来源：http://lfa.yuanzhike.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mtj.bjfxy.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://iql.yanxiufei.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://alh.bjfxy.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wqo.quarkkingdee.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://nur.zhoulong.xyz

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mrl.yanxiufei.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mcf.meibo888.top

[L05] 上传文件（multipart）
来源：http://eef.shanyushiyangtech.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://phn.tarul.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://dtv.nanxuanxn.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mar.zhoulong.xyz

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://tnq.cdnleiting.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://bwd.ybcxt.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hdu.kuanghao11.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://pqu.jqgufenzy.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://lqr.svipenyu.cn

[L06] 解析响应为 JSON
来源：http://dlt.fktsv.cn

Py:   resp.json()
来源：http://sfa.shzxlz.cn

PHP:  json_decode($body, true);
来源：http://cal.52xcode.cn

JS:   await resp.json()
来源：http://tbw.havefunace.top

TS:   await resp.json()
来源：http://rxn.chenzaomai.com

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://bvc.quarkkingdee.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://uye.fktsv.cn

Ruby: JSON.parse(resp.body)
来源：http://ncx.hongshengwenyu.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ifg.guannengcc.top

[L07] 处理 HTTP 状态码
来源：http://gmv.chenlongwang.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hes.xziqi.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ldc.epnwcf.com

JS:   resp.ok;  resp.status
来源：http://akx.shanyushiyangtech.top

TS:   resp.ok;  resp.status
来源：http://xfo.hcnkem.com

Java: resp.statusCode()
来源：http://ouo.zhixingplan.top

Go:   resp.StatusCode
来源：http://age.nanxinkj.top

Ruby: resp.code.to_i
来源：http://pbx.vehdjk.com

C#:   (int)resp.StatusCode
来源：http://kxf.xziqi.cn

[L08] 并发请求多个地址
来源：http://rfv.gogol.net.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://tuf.hywenlv.cn

PHP:  curl_multi_init() 系列
来源：http://qnh.ehwqpu.com

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://fyu.gogol.net.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ngc.jqgufenzy.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://xbg.yfazqb.com

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://sko.uphjek.com

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://htf.ctjpmb.com

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://maa.andypj.xyz

================================================================================
来源：http://wic.hesvh.cn

M. 命令行 / 进程 / 环境
来源：http://aie.dashuyun.cn

================================================================================
来源：http://zur.zhengqikj.top

[M01] 读取命令行参数
来源：http://ihz.shuidangran.top

Py:   sys.argv[1:]
来源：http://gvz.fktsv.cn

PHP:  $argv;  $argc;
来源：http://gef.yj20258888.top

JS:   process.argv.slice(2)
来源：http://pto.mhx1999.top

TS:   process.argv.slice(2)
来源：http://ypu.yongpay.top

Java: args 数组（main 方法参数）
来源：http://usc.tanke756.top

Go:   os.Args[1:]
来源：http://kxv.fzhhl.top

Ruby: ARGV
来源：http://exw.jinyuanbaomall.cn

C#:   args 数组（Main 方法参数）
来源：http://xlv.gaohongyu789.top

[M02] 读取环境变量
来源：http://nje.daxiang520.top

Py:   os.environ.get("HOME")
来源：http://reb.zdqjudy.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://foj.shuidangran.top

JS:   process.env.HOME
来源：http://qit.yanxiufei.cn

TS:   process.env.HOME
来源：http://qox.sufxvd.cn

Java: System.getenv("HOME")
来源：http://grv.ybcxt.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://twm.wangshuangyany.cn

Ruby: ENV["HOME"]
来源：http://kxl.zhiwuduotai.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://bnn.jlsjyb.cn

[M03] 执行外部命令
来源：http://hxv.birdmap.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://bhr.yonumen.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wvo.hammf.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://rlr.0kj1m.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://sop.cqqwz.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://yoa.nwbrower.top

Go:   exec.Command("ls", "-l").Output()
来源：http://oro.jinyuanbaomall.cn

Ruby: system("ls -l");  `ls -l`
来源：http://rjp.316326.xyz

C#:   Process.Start("ls", "-l");
来源：http://csm.zdqjudy.top

[M04] 获取当前工作目录
来源：http://zlg.cashguo.top

Py:   os.getcwd()
来源：http://zxa.aibaodan.cn

PHP:  getcwd();
来源：http://ceq.pycfn.com

JS:   process.cwd()
来源：http://not.dashuyun.cn

TS:   process.cwd()
来源：http://net.hammf.cn

Java: Path.of("").toAbsolutePath()
来源：http://dwo.yongpay.top

Go:   os.Getwd()
来源：http://shi.shuidangran.top

Ruby: Dir.pwd
来源：http://ewg.cashguo.top

C#:   Directory.GetCurrentDirectory()
来源：http://gfa.jiagoushi.top

[M05] 设置退出码
来源：http://stt.hnqzz.top

Py:   sys.exit(1)
来源：http://blo.sxryk.cn

PHP:  exit(1);
来源：http://wao.havefunace.top

JS:   process.exit(1)
来源：http://lwq.dianchejie.cn

TS:   process.exit(1)
来源：http://gtd.dianchejie.cn

Java: System.exit(1)
来源：http://hls.9152youxi.cn

Go:   os.Exit(1)
来源：http://uvn.yvedp.cn

Ruby: exit 1
来源：http://sdk.fehbvm.com

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://iwo.zdqjudy.top

[M06] 向标准错误输出
来源：http://kxm.pycfn.com

Py:   print("err", file=sys.stderr)
来源：http://mfu.daxiang520.top

PHP:  fwrite(STDERR, "err\n");
来源：http://eqa.yueranfly.top

JS:   console.error("err")
来源：http://exn.ehwqpu.com

TS:   console.error("err")
来源：http://mue.epnwcf.com

Java: System.err.println("err")
来源：http://vls.shzxlz.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://fth.zhengqikj.top

Ruby: warn "err"
来源：http://uiv.yuxming.cn

C#:   Console.Error.WriteLine("err")
来源：http://hou.gaohongyu789.top

[M07] 判断是否为主入口
来源：http://plp.pengpengdd.cyou

Py:   if __name__ == "__main__":
来源：http://cee.cqqwz.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://vue.yj20258.top

JS:   require.main === module
来源：http://fku.chenlongwang.top

TS:   require.main === module
来源：http://frt.jiagoushi.top

Java: public static void main(String[] args)
来源：http://smf.wangdashe.top

Go:   func main()
来源：http://mvp.zhaomingkeji.xyz

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://gbv.zhongyouzk.top

C#:   static void Main(string[] args)
来源：http://blz.9152youxi.cn

[M08] 获取系统与运行时信息
来源：http://hut.yanxiufei.cn

Py:   platform.system();  platform.python_version()
来源：http://qad.uphjek.com

PHP:  PHP_OS;  phpversion();
来源：http://pvr.hesvh.cn

JS:   process.platform;  process.version
来源：http://hlu.jinghuilouyu.cn

TS:   process.platform;  process.version
来源：http://mcp.ppjwa.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://bgn.tarul.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://ejg.guannengcc.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://crk.yuanzhike.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://wid.ywan-chungtsiang.top

================================================================================
来源：http://cdz.wangshuangyany.cn

N. 数据结构与算法
来源：http://uhq.yongpay.top

================================================================================
来源：http://jty.jinqigufen.top

[N01] 二分查找（有序数组）
来源：http://xvw.ppjwa.cn

Py:   bisect.bisect_left(arr, x)
来源：http://blk.birdmap.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ouz.jlsjyb.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://kgc.vehdjk.com

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ttz.shangyingyoupin.top

Java: Arrays.binarySearch(arr, x)
来源：http://vrm.nwbrower.top

Go:   sort.SearchInts(arr, x)
来源：http://qfy.xingfuxueyuan.xyz

Ruby: arr.bsearch { |e| e >= x }
来源：http://gno.ppjwa.cn

C#:   Array.BinarySearch(arr, x)
来源：http://vlj.ydzc1.top

[N02] 排序（工程实践用内置实现）
来源：http://jlr.dashuyun.cn

Py:   sorted(arr);  arr.sort()
来源：http://zgc.smart0.xyz

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ymb.uphjek.com

JS:   [...arr].sort((a, b) => a - b)
来源：http://ulf.zhixingplan.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://dry.hesvh.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ksk.feifeiyinyue.top

Go:   slices.Sort(arr)
来源：http://qrr.daria6918.cn

Ruby: arr.sort
来源：http://rly.sysykeji.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://lgv.iojbl.cn

[N03] 快速排序（分治示例）
来源：http://lsp.hnqzz.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://sun.pengpengdd.cyou

PHP:  // 递归实现，或用 usort
来源：http://tqv.cdnleiting.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ypl.fehbvm.com

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://xme.yuxming.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ufc.hesvh.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://abr.gaohongyu789.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://yca.jlsjyb.cn

C#:   // 手写递归，或 Array.Sort
来源：http://auk.hongshengwenyu.top

[N04] 斐波那契数列
来源：http://ohf.dashuyun.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://djv.xziqi.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://tfe.xuanzx.com

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://gru.hesvh.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://zxd.xinyue.icu

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://egf.gaohongyu789.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://snw.haohaochexian.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wnz.chenlongwang.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ppr.shangyingyoupin.top

[N05] 最大公约数
来源：http://rht.daxiang520.top

Py:   math.gcd(a, b)
来源：http://znb.shzxlz.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://vmq.ctjpmb.com

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://kpk.pycfn.com

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ivh.nwbrower.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://efc.vqdsnc.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://nkj.zhaomingkeji.xyz

Ruby: a.gcd(b)
来源：http://knp.guowangkeji.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://meq.gogol.net.cn

[N06] 判断回文字符串
来源：http://kec.sjlbkw.cn

Py:   s == s[::-1]
来源：http://oky.ehwqpu.com

PHP:  $s === strrev($s);
来源：http://wpz.nwbrower.top

JS:   s === [...s].reverse().join("")
来源：http://rhl.shanyushiyangkeji.top

TS:   s === [...s].reverse().join("")
来源：http://irl.xuanzx.com

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://god.jinqigufen.top

Go:   // 双指针从两端比较
来源：http://jof.zhaomingkeji.xyz

Ruby: s == s.reverse
来源：http://lon.zhaomingkeji.xyz

C#:   s == new string(s.Reverse().ToArray())
来源：http://pps.xuanzx.com

[N07] 两数之和（返回下标）
来源：http://iek.gotoacloud.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://dca.yuanzhike.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://amb.ywan-chungtsiang.top

JS:   // 手写 Map：map.set(v, i)
来源：http://rhe.316326.xyz

TS:   // 手写 Map<string, number>
来源：http://cvi.jinqigufen.top

Java: // 手写 HashMap
来源：http://csy.hcnkem.com

Go:   // 手写 map[int]int
来源：http://vmx.shuidangran.top

Ruby: // 手写 Hash
来源：http://xyj.hesvh.cn

C#:   // 手写 Dictionary<int, int>
来源：http://sae.gogol.net.cn

[N08] 生成全排列
来源：http://sji.tianlin.xyz

Py:   itertools.permutations(arr)
来源：http://mmn.gzhubu.top

PHP:  // 手写递归交换
来源：http://oei.shangyingyoupin.top

JS:   // 手写回溯递归
来源：http://hnu.hysaishi.cn

TS:   // 手写回溯递归
来源：http://prr.chenlongwang.top

Java: // 手写回溯递归
来源：http://jei.sxryk.cn

Go:   // 手写回溯递归
来源：http://dtk.jiagoushi.top

Ruby: arr.permutation.to_a
来源：http://opn.bbcook.cn

C#:   // 手写回溯递归
来源：http://dzy.fktsv.cn

[N09] 栈与队列
来源：http://xud.yangfankeji.com

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://aez.birdmap.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://pzz.yangfankeji.com

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://adk.jqgfzy.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hdu.zhiwuduotai.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wgf.sysykeji.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://lcc.cashguo.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://lal.chenlongwang.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://itu.birdmap.top

[N10] 链表节点定义
来源：http://mgh.dashuyun.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ydm.gogol.net.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://zkr.guannengcc.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://chc.aizwys.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://aat.gzhubu.top

Java: class Node { int v; Node next; }
来源：http://tlk.yueranfly.top

Go:   type Node struct { V int; Next *Node }
来源：http://vso.fzhhl.top

Ruby: Node = Struct.new(:v, :next)
来源：http://ygr.vqdsnc.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://pdn.bjfxy.top

[N11] 二叉树中序遍历
来源：http://yjj.hnxiangtu.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hwq.hywenlv.cn

PHP:  // 手写递归函数
来源：http://xhg.xziqi.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ied.zhoulong.xyz

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hko.yvedp.cn

Java: // 手写递归
来源：http://nmq.jinqigufen.top

Go:   // 手写递归
来源：http://pgg.hongshengwenyu.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://kqa.daxiang520.top

C#:   // 手写递归
来源：http://wvf.cashguo.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://yxa.9152youxi.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wpz.tianlin.xyz

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://act.xziqi.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://vpw.yj20258.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://pfx.jinqigfzy.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://udl.zhongyouzk.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://jzl.ctjpmb.com

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://svq.sxryk.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://amn.jinyuanbaomall.cn

================================================================================
来源：http://cyn.jyoumei.cn

O. 并发与异步
来源：http://nbd.nwbrower.top

================================================================================
来源：http://vrm.shzxlz.cn

[O01] 启动一个线程
来源：http://rue.jinghuilouyu.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://upo.52xcode.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://rzg.wangshuangyany.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://zue.zhixingplan.top

TS:   // 同 JS
来源：http://zky.c1oappe.top

Java: new Thread(() -> f()).start()
来源：http://ocx.hywenlv.cn

Go:   go f()
来源：http://cil.bbcook.cn

Ruby: Thread.new { f }
来源：http://qvk.xingfuxueyuan.xyz

C#:   Task.Run(() => F());
来源：http://xgu.dashuyun.cn

[O02] 使用线程池
来源：http://qki.fanxiaobao.xyz

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ztv.chenlongwang.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://rzn.guannengcc.top

JS:   // worker_threads 线程池
来源：http://pyk.gaohongyu789.top

TS:   // worker_threads 线程池
来源：http://roa.cqqwz.cn

Java: Executors.newFixedThreadPool(4)
来源：http://ztl.epnwcf.com

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wxd.haohaochexian.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://qbk.yonumen.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://nmo.chenlongwang.top

[O03] 加锁保护共享数据
来源：http://rwd.zhengqikj.top

Py:   with lock: shared += 1
来源：http://owm.xziqi.cn

PHP:  // 用 flock() 做文件锁
来源：http://xmm.jianghu66.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://yzm.mhx1999.top

TS:   // 同 JS
来源：http://bfm.shuidangran.top

Java: synchronized (this) { shared++; }
来源：http://wsd.zhongyouzk.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://uax.smart0.xyz

Ruby: mutex.synchronize { shared += 1 }
来源：http://pzh.jinqigfzy.top

C#:   lock (gate) { shared++; }
来源：http://qtt.chenzaomai.com

[O04] 定义异步函数并等待
来源：http://azp.jianghu66.top

Py:   async def f():⏎    await g()
来源：http://gtk.tanke756.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://pir.havefunace.top

JS:   async function f() { await g(); }
来源：http://ixx.ehwqpu.com

TS:   async function f(): Promise<void> { await g(); }
来源：http://qwx.jinqigfzy.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://oin.jqgfzy.top


<!-- 参考信息 -->