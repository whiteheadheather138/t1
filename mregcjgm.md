代发 wailian999

L. 网络请求
来源：http://mep.haohaochexian.top

================================================================================
来源：http://lsv.pycfn.com

[L01] 发送 GET 请求
来源：http://aib.chenzaomai.com

Py:   requests.get(url)                        # 第三方库 requests
来源：http://iuy.c1oappe.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://flc.fanxiaobao.xyz

JS:   await fetch(url)
来源：http://oma.zdqjudy.top

TS:   await fetch(url)
来源：http://oew.yuxming.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ygg.zhoulong.xyz

Go:   resp, err := http.Get(url)
来源：http://jxk.epnwcf.com

Ruby: Net::HTTP.get(URI(url))
来源：http://eas.jinghuilouyu.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://czx.iojbl.cn

[L02] 发送 POST JSON
来源：http://xer.tarul.cn

Py:   requests.post(url, json={"a": 1})
来源：http://gas.fanxiaobao.xyz

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://xgo.aibaodan.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://lnk.hongshengwenyu.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://giw.fehbvm.com

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mdv.hesvh.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wow.xuetiantiany.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://foo.zhongyouzk.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mmy.sufxvd.cn

[L03] 设置自定义请求头
来源：http://zpc.shanyushiyangkeji.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://sst.nanxinkj.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://vho.c1oappe.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://nty.jqgufenzy.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hub.xinyue.icu

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wpk.shuidangran.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://kik.yangfankeji.com

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wcx.zhoulong.xyz

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://dvj.kuanghao11.cn

[L04] 设置超时
来源：http://shg.jiagoushi.top

Py:   requests.get(url, timeout=5)
来源：http://xcb.sufxvd.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://axx.fzhhl.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ahy.gogol.net.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://fwo.epnwcf.com

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ycu.jqgfzy.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://pnr.zhoulong.xyz

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://efw.cdnleiting.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://kyy.sysykeji.top

[L05] 上传文件（multipart）
来源：http://vzj.jiagoushi.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://uad.xingfuxueyuan.xyz

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ukg.xylfe.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ibn.cdnleiting.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://bbf.shuidangran.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://jyg.pycfn.com

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://yaq.pycfn.com

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ucu.zhixingplan.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://zmo.hcnkem.com

[L06] 解析响应为 JSON
来源：http://ydl.wangdashe.top

Py:   resp.json()
来源：http://lmu.zdbjq.cn

PHP:  json_decode($body, true);
来源：http://vnj.chenjidiqi.icu

JS:   await resp.json()
来源：http://evh.zhengqikj.top

TS:   await resp.json()
来源：http://coi.cashguo.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://oqo.zhaomingkeji.xyz

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ynx.jqgfzy.top

Ruby: JSON.parse(resp.body)
来源：http://pdf.shanyushiyangkeji.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://uwy.yonumen.top

[L07] 处理 HTTP 状态码
来源：http://jrz.dashuyun.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://lfn.dianchejie.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://tqs.fengsongda.top

JS:   resp.ok;  resp.status
来源：http://bwt.zdbjq.cn

TS:   resp.ok;  resp.status
来源：http://ooe.ctjpmb.com

Java: resp.statusCode()
来源：http://lpz.tarul.cn

Go:   resp.StatusCode
来源：http://jet.kuanghao11.cn

Ruby: resp.code.to_i
来源：http://kes.zhoulong.xyz

C#:   (int)resp.StatusCode
来源：http://sqx.yueranfly.top

[L08] 并发请求多个地址
来源：http://dnm.cucudq.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://uel.cucudq.cn

PHP:  curl_multi_init() 系列
来源：http://yyj.zhaomingkeji.xyz

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wqx.316326.xyz

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://yps.zhaomingkeji.xyz

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://vqg.316326.xyz

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://rla.vehdjk.com

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://dna.bjfxy.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://lif.snrcjt.cn

================================================================================
来源：http://dzr.shanyushiyangkeji.top

M. 命令行 / 进程 / 环境
来源：http://yqd.tarul.cn

================================================================================
来源：http://phv.hesvh.cn

[M01] 读取命令行参数
来源：http://szr.yangfankeji.com

Py:   sys.argv[1:]
来源：http://cdw.zhaomingkeji.xyz

PHP:  $argv;  $argc;
来源：http://xem.0kj1m.cn

JS:   process.argv.slice(2)
来源：http://khc.jinqigufen.top

TS:   process.argv.slice(2)
来源：http://jkg.yuanzhike.top

Java: args 数组（main 方法参数）
来源：http://bjc.redwolf501.top

Go:   os.Args[1:]
来源：http://bwv.fengsongda.top

Ruby: ARGV
来源：http://hom.tian-w.cn

C#:   args 数组（Main 方法参数）
来源：http://gvg.yueranfly.top

[M02] 读取环境变量
来源：http://kqn.zdqjudy.top

Py:   os.environ.get("HOME")
来源：http://nzw.tarul.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mgg.wangshuangyany.cn

JS:   process.env.HOME
来源：http://qzy.bbcook.cn

TS:   process.env.HOME
来源：http://xwe.uphjek.com

Java: System.getenv("HOME")
来源：http://psb.havefunace.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://fdy.aizwys.cn

Ruby: ENV["HOME"]
来源：http://qrq.sjlbkw.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://zhf.gaohongyu789.top

[M03] 执行外部命令
来源：http://ztx.tanke756.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://jml.ywan-chungtsiang.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://yib.gogol.net.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://xkz.hnqzz.top

TS:   child_process.execSync("ls -l").toString()
来源：http://vom.pycfn.com

Java: new ProcessBuilder("ls", "-l").start()
来源：http://dak.shanyushiyangkeji.top

Go:   exec.Command("ls", "-l").Output()
来源：http://frg.gzhubu.top

Ruby: system("ls -l");  `ls -l`
来源：http://tpd.zhiwuduotai.top

C#:   Process.Start("ls", "-l");
来源：http://koc.chenlongwang.top

[M04] 获取当前工作目录
来源：http://cwd.guannengcc.top

Py:   os.getcwd()
来源：http://iyr.ybcxt.top

PHP:  getcwd();
来源：http://ffe.zhiwuduotai.top

JS:   process.cwd()
来源：http://nfy.hongshengwenyu.top

TS:   process.cwd()
来源：http://dod.sxryk.cn

Java: Path.of("").toAbsolutePath()
来源：http://nzk.chenjidiqi.icu

Go:   os.Getwd()
来源：http://pxs.aizwys.cn

Ruby: Dir.pwd
来源：http://jip.jinghuilouyu.cn

C#:   Directory.GetCurrentDirectory()
来源：http://lwm.ydzc1.top

[M05] 设置退出码
来源：http://ebi.9152youxi.cn

Py:   sys.exit(1)
来源：http://iue.xziqi.cn

PHP:  exit(1);
来源：http://eeq.zhixingplan.top

JS:   process.exit(1)
来源：http://ndc.vqdsnc.cn

TS:   process.exit(1)
来源：http://hhs.haohaochexian.top

Java: System.exit(1)
来源：http://lbe.xylfe.cn

Go:   os.Exit(1)
来源：http://xiw.svipenyu.cn

Ruby: exit 1
来源：http://oya.cqqwz.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://vjo.xuanzx.com

[M06] 向标准错误输出
来源：http://xnp.shanyushiyangtech.top

Py:   print("err", file=sys.stderr)
来源：http://rbe.zhongyouzk.top

PHP:  fwrite(STDERR, "err\n");
来源：http://znd.aibaodan.cn

JS:   console.error("err")
来源：http://ljw.svipenyu.cn

TS:   console.error("err")
来源：http://djb.cashguo.top

Java: System.err.println("err")
来源：http://llq.yfazqb.com

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wjn.hnqzz.top

Ruby: warn "err"
来源：http://uxp.shangyingyoupin.top

C#:   Console.Error.WriteLine("err")
来源：http://czw.xingfuxueyuan.xyz

[M07] 判断是否为主入口
来源：http://lyw.feifeiyinyue.top

Py:   if __name__ == "__main__":
来源：http://jwd.ybcxt.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://rvp.yvedp.cn

JS:   require.main === module
来源：http://jfi.daxiang520.top

TS:   require.main === module
来源：http://nmy.daria6918.cn

Java: public static void main(String[] args)
来源：http://cog.9152youxi.cn

Go:   func main()
来源：http://yil.jiagoushi.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://jyx.yj20258.top

C#:   static void Main(string[] args)
来源：http://nmf.shanyushiyangkeji.top

[M08] 获取系统与运行时信息
来源：http://jns.aibaodan.cn

Py:   platform.system();  platform.python_version()
来源：http://tkl.hysaishi.cn

PHP:  PHP_OS;  phpversion();
来源：http://hgi.yfazqb.com

JS:   process.platform;  process.version
来源：http://ozl.yanxiufei.cn

TS:   process.platform;  process.version
来源：http://emk.havefunace.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://alk.xuanzx.com

Go:   runtime.GOOS;  runtime.Version()
来源：http://dky.aibaodan.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://moh.shangyingyoupin.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://wmw.fengsongda.top

================================================================================
来源：http://apl.nwbrower.top

N. 数据结构与算法
来源：http://cgl.vqdsnc.cn

================================================================================
来源：http://luq.hfpthk.cn

[N01] 二分查找（有序数组）
来源：http://plo.ydjk.org.cn

Py:   bisect.bisect_left(arr, x)
来源：http://qep.dashuyun.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://tyw.zhaomingkeji.xyz

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://irm.pengpengdd.cyou

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://yac.daxiang520.top

Java: Arrays.binarySearch(arr, x)
来源：http://uht.hysaishi.cn

Go:   sort.SearchInts(arr, x)
来源：http://hyq.52xcode.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://lwr.haohaochexian.top

C#:   Array.BinarySearch(arr, x)
来源：http://dys.jinqigfzy.top

[N02] 排序（工程实践用内置实现）
来源：http://ahd.0kj1m.cn

Py:   sorted(arr);  arr.sort()
来源：http://css.cheryme.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mqr.cucudq.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://qhi.yfazqb.com

TS:   [...arr].sort((a, b) => a - b)
来源：http://zyd.zhongyouzk.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://eiy.jinghuilouyu.cn

Go:   slices.Sort(arr)
来源：http://bkc.fktsv.cn

Ruby: arr.sort
来源：http://fxk.pycfn.com

C#:   Array.Sort(arr);  list.Sort()
来源：http://fha.aibaodan.cn

[N03] 快速排序（分治示例）
来源：http://lvi.dashuyun.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://gip.jiagoushi.top

PHP:  // 递归实现，或用 usort
来源：http://yqt.yfazqb.com

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://xol.hnxiangtu.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hrt.havefunace.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://jtq.gaohongyu789.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://meq.vqdsnc.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://yvt.haohaochexian.top

C#:   // 手写递归，或 Array.Sort
来源：http://pdm.fanxiaobao.xyz

[N04] 斐波那契数列
来源：http://edg.fanxiaobao.xyz

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://led.nanxuanxn.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hzw.fktsv.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://yue.zhongyouzk.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://vvs.yongpay.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://htk.ywan-chungtsiang.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://nte.mhx1999.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://qyn.hongshengwenyu.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://oco.tanke756.top

[N05] 最大公约数
来源：http://pwu.zhengqikj.top

Py:   math.gcd(a, b)
来源：http://aaq.chenlongwang.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://brb.shangyingyoupin.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://yqg.nanxuanxn.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://pmt.jinqigfzy.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://fwd.hongshengwenyu.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://xib.chenlongwang.top

Ruby: a.gcd(b)
来源：http://tvr.hcnkem.com

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://nbu.havefunace.top

[N06] 判断回文字符串
来源：http://hln.0kj1m.cn

Py:   s == s[::-1]
来源：http://cqn.yuxming.cn

PHP:  $s === strrev($s);
来源：http://mnt.zycfv.cn

JS:   s === [...s].reverse().join("")
来源：http://osy.sjlbkw.cn

TS:   s === [...s].reverse().join("")
来源：http://zxl.hammf.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://awi.gaohongyu789.top

Go:   // 双指针从两端比较
来源：http://asp.zhixingplan.top

Ruby: s == s.reverse
来源：http://rhh.aizwys.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://bee.jinghuilouyu.cn

[N07] 两数之和（返回下标）
来源：http://yyf.bjfxy.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://kyy.wangdashe.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ces.chenzaomai.com

JS:   // 手写 Map：map.set(v, i)
来源：http://ypk.fktsv.cn

TS:   // 手写 Map<string, number>
来源：http://aqf.ehwqpu.com

Java: // 手写 HashMap
来源：http://wty.nwbrower.top

Go:   // 手写 map[int]int
来源：http://yjy.daria6918.cn

Ruby: // 手写 Hash
来源：http://pwt.fanxiaobao.xyz

C#:   // 手写 Dictionary<int, int>
来源：http://anw.yvedp.cn

[N08] 生成全排列
来源：http://wdb.zycfv.cn

Py:   itertools.permutations(arr)
来源：http://eli.aizwys.cn

PHP:  // 手写递归交换
来源：http://zgv.hnxiangtu.top

JS:   // 手写回溯递归
来源：http://spf.chenzaomai.com

TS:   // 手写回溯递归
来源：http://hzu.jinyuanbaomall.cn

Java: // 手写回溯递归
来源：http://jme.jqgfzy.top

Go:   // 手写回溯递归
来源：http://cht.shuidangran.top

Ruby: arr.permutation.to_a
来源：http://fuh.nanxinkj.top

C#:   // 手写回溯递归
来源：http://ibn.zdqjudy.top

[N09] 栈与队列
来源：http://wrk.jqgufenzy.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hkt.0kj1m.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://vak.nwbrower.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://pfj.yanxiufei.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://jns.zycfv.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mmh.sufxvd.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://gwt.hfpthk.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hnw.tarul.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://alq.yonumen.top

[N10] 链表节点定义
来源：http://rau.tian-w.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://xdy.hnxiangtu.top

PHP:  class Node { public $v; public $next = null; }
来源：http://ckl.yangfankeji.com

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://yag.fktsv.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ijl.yongpay.top

Java: class Node { int v; Node next; }
来源：http://ktt.nwbrower.top

Go:   type Node struct { V int; Next *Node }
来源：http://fcl.chenzaomai.com

Ruby: Node = Struct.new(:v, :next)
来源：http://duw.uphjek.com

C#:   class Node { public int V; public Node? Next; }
来源：http://iig.c1oappe.top

[N11] 二叉树中序遍历
来源：http://esu.aizwys.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://jlb.zhixingplan.top

PHP:  // 手写递归函数
来源：http://kdp.quarkkingdee.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://tic.daria6918.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://yff.zycfv.cn

Java: // 手写递归
来源：http://cho.cqqwz.cn

Go:   // 手写递归
来源：http://tfi.ppjwa.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hgo.iojbl.cn

C#:   // 手写递归
来源：http://nwu.xziqi.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://vim.yfazqb.com

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://weh.wangshuangyany.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://eoy.daxiang520.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://dxh.zhaomingkeji.xyz

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://jbl.aibaodan.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ybn.yanxiufei.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://psd.uphjek.com

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://xqo.dianchejie.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mde.sxryk.cn

================================================================================
来源：http://odw.wangdashe.top

O. 并发与异步
来源：http://vun.yuxming.cn

================================================================================
来源：http://eof.9152youxi.cn

[O01] 启动一个线程
来源：http://bfo.hywenlv.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://yqp.vehdjk.com

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://whr.andypj.xyz

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://uam.jiagoushi.top

TS:   // 同 JS
来源：http://msi.tianlin.xyz

Java: new Thread(() -> f()).start()
来源：http://ndr.316326.xyz

Go:   go f()
来源：http://cku.vqdsnc.cn

Ruby: Thread.new { f }
来源：http://eoh.hnxiangtu.top

C#:   Task.Run(() => F());
来源：http://yrj.zhengqikj.top

[O02] 使用线程池
来源：http://fxd.hnxiangtu.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hxr.jiagoushi.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://eri.jinqigfzy.top

JS:   // worker_threads 线程池
来源：http://qsi.feifeiyinyue.top

TS:   // worker_threads 线程池
来源：http://gca.meibo888.top

Java: Executors.newFixedThreadPool(4)
来源：http://crm.chenzaomai.com

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://udi.xziqi.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://tvj.zhixingplan.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://var.shangyingyoupin.top

[O03] 加锁保护共享数据
来源：http://vdg.yangfankeji.com

Py:   with lock: shared += 1
来源：http://zft.chenjidiqi.icu

PHP:  // 用 flock() 做文件锁
来源：http://rgr.pycfn.com

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://qus.snrcjt.cn

TS:   // 同 JS
来源：http://vwd.0kj1m.cn

Java: synchronized (this) { shared++; }
来源：http://czn.hammf.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://lsg.ywan-chungtsiang.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://pcs.iojbl.cn

C#:   lock (gate) { shared++; }
来源：http://yxp.ydzc1.top

[O04] 定义异步函数并等待
来源：http://sfo.jinghuilouyu.cn

Py:   async def f():⏎    await g()
来源：http://tbb.daxiang520.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ujz.haohaochexian.top

JS:   async function f() { await g(); }
来源：http://pfz.xingfuxueyuan.xyz

TS:   async function f(): Promise<void> { await g(); }
来源：http://esd.yuanzhike.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://uly.sxryk.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://bte.iojbl.cn

Ruby: # 用 Fiber 或 async gem
来源：http://mag.fanxiaobao.xyz

C#:   async Task F() { await G(); }
来源：http://eah.nanxinkj.top

[O05] 并发执行并等待全部完成
来源：http://sxl.zhengqikj.top


<!-- 参考信息 -->