代发 wailian999

L. 网络请求
来源：http://cph.iojbl.cn

================================================================================
来源：http://cyy.xuetiantiany.cn

[L01] 发送 GET 请求
来源：http://zfp.shuidangran.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://elc.jinyuanbaomall.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hvv.cqqwz.cn

JS:   await fetch(url)
来源：http://aqb.zdbjq.cn

TS:   await fetch(url)
来源：http://oeb.tian-w.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://yyl.tian-w.cn

Go:   resp, err := http.Get(url)
来源：http://usl.pycfn.com

Ruby: Net::HTTP.get(URI(url))
来源：http://vkj.zhaomingkeji.xyz

C#:   await new HttpClient().GetStringAsync(url)
来源：http://cyc.ywan-chungtsiang.top

[L02] 发送 POST JSON
来源：http://osh.hcnkem.com

Py:   requests.post(url, json={"a": 1})
来源：http://bzd.jinyuanbaomall.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ftv.zhaomingkeji.xyz

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://vul.jiagoushi.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://egv.jinqigfzy.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://kyo.cdnleiting.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://pwb.zhoulong.xyz

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hju.epnwcf.com

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ups.shanyushiyangtech.top

[L03] 设置自定义请求头
来源：http://nsd.0kj1m.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://rrv.cucudq.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hgb.chenlongwang.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://zrj.hongshengwenyu.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://lex.andypj.xyz

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://vpd.gaohongyu789.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://quj.hnxiangtu.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://abu.zhoulong.xyz

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://jkm.aizwys.cn

[L04] 设置超时
来源：http://drt.sxryk.cn

Py:   requests.get(url, timeout=5)
来源：http://csj.havefunace.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://saw.chenlongwang.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://nkp.fanxiaobao.xyz

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://dgn.daria6918.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hcu.shangyingyoupin.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://fpm.jqgfzy.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hhu.yueranfly.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://fnm.zdqjudy.top

[L05] 上传文件（multipart）
来源：http://eyv.cashguo.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://tbq.jinqigfzy.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://tiq.jinqigufen.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://aen.yuanzhike.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://oxq.cheryme.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://zyg.jiagoushi.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://skd.shuidangran.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wcx.jinghuilouyu.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://jpc.chenjidiqi.icu

[L06] 解析响应为 JSON
来源：http://oer.hesvh.cn

Py:   resp.json()
来源：http://cbp.shanyushiyangtech.top

PHP:  json_decode($body, true);
来源：http://eyk.jinghuilouyu.cn

JS:   await resp.json()
来源：http://pgs.guannengcc.top

TS:   await resp.json()
来源：http://xjy.ivvv.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://sgo.wangdashe.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://zyn.jqgufenzy.top

Ruby: JSON.parse(resp.body)
来源：http://nci.mhx1999.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://dij.birdmap.top

[L07] 处理 HTTP 状态码
来源：http://zho.wangdashe.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://lyh.52xcode.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://kqk.316326.xyz

JS:   resp.ok;  resp.status
来源：http://zgb.cashguo.top

TS:   resp.ok;  resp.status
来源：http://spf.birdmap.top

Java: resp.statusCode()
来源：http://wcz.zhongyouzk.top

Go:   resp.StatusCode
来源：http://wvr.uphjek.com

Ruby: resp.code.to_i
来源：http://lcz.shangyingyoupin.top

C#:   (int)resp.StatusCode
来源：http://unj.uphjek.com

[L08] 并发请求多个地址
来源：http://feg.tanke756.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hif.zhengqikj.top

PHP:  curl_multi_init() 系列
来源：http://ygs.gotoacloud.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ivl.xuanzx.com

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ppb.fktsv.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wbl.mhx1999.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hwk.yanxiufei.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://pfy.hfpthk.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://bef.svipenyu.cn

================================================================================
来源：http://bsb.tianlin.xyz

M. 命令行 / 进程 / 环境
来源：http://ngt.cashguo.top

================================================================================
来源：http://lls.zhaomingkeji.xyz

[M01] 读取命令行参数
来源：http://wbx.jqgfzy.top

Py:   sys.argv[1:]
来源：http://ovc.yonumen.top

PHP:  $argv;  $argc;
来源：http://zdr.nanxuanxn.top

JS:   process.argv.slice(2)
来源：http://fer.zhaomingkeji.xyz

TS:   process.argv.slice(2)
来源：http://kny.ctjpmb.com

Java: args 数组（main 方法参数）
来源：http://ice.kuanghao11.cn

Go:   os.Args[1:]
来源：http://gye.zhongyouzk.top

Ruby: ARGV
来源：http://qfp.uphjek.com

C#:   args 数组（Main 方法参数）
来源：http://idb.hesvh.cn

[M02] 读取环境变量
来源：http://qiv.cashguo.top

Py:   os.environ.get("HOME")
来源：http://xpe.yj20258.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://jne.hnxiangtu.top

JS:   process.env.HOME
来源：http://zmj.yvedp.cn

TS:   process.env.HOME
来源：http://iqc.chenlongwang.top

Java: System.getenv("HOME")
来源：http://zij.hywenlv.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://bxe.hcnkem.com

Ruby: ENV["HOME"]
来源：http://whe.ydjk.org.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ilg.shangyingyoupin.top

[M03] 执行外部命令
来源：http://hrl.gaohongyu789.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://kbj.shzxlz.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://pjg.gzhubu.top

JS:   child_process.execSync("ls -l").toString()
来源：http://hzs.zhengqikj.top

TS:   child_process.execSync("ls -l").toString()
来源：http://aft.0kj1m.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://dku.zhongyouzk.top

Go:   exec.Command("ls", "-l").Output()
来源：http://qod.xylfe.cn

Ruby: system("ls -l");  `ls -l`
来源：http://jkk.zhixingplan.top

C#:   Process.Start("ls", "-l");
来源：http://afg.shanyushiyangkeji.top

[M04] 获取当前工作目录
来源：http://sqa.dianchejie.cn

Py:   os.getcwd()
来源：http://ydj.guannengcc.top

PHP:  getcwd();
来源：http://agq.hfpthk.cn

JS:   process.cwd()
来源：http://vox.shuidangran.top

TS:   process.cwd()
来源：http://clq.ehwqpu.com

Java: Path.of("").toAbsolutePath()
来源：http://lok.gogol.net.cn

Go:   os.Getwd()
来源：http://hll.xingfuxueyuan.xyz

Ruby: Dir.pwd
来源：http://obk.ppjwa.cn

C#:   Directory.GetCurrentDirectory()
来源：http://csb.shangyingyoupin.top

[M05] 设置退出码
来源：http://ggp.zhixingplan.top

Py:   sys.exit(1)
来源：http://abw.hysaishi.cn

PHP:  exit(1);
来源：http://vee.yangfankeji.com

JS:   process.exit(1)
来源：http://rgs.jinghuilouyu.cn

TS:   process.exit(1)
来源：http://mib.fehbvm.com

Java: System.exit(1)
来源：http://dnk.hammf.cn

Go:   os.Exit(1)
来源：http://xxu.gaohongyu789.top

Ruby: exit 1
来源：http://jhg.zhengqikj.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://tcf.epnwcf.com

[M06] 向标准错误输出
来源：http://wgj.zhoulong.xyz

Py:   print("err", file=sys.stderr)
来源：http://nbx.pycfn.com

PHP:  fwrite(STDERR, "err\n");
来源：http://tqv.cqqwz.cn

JS:   console.error("err")
来源：http://qoc.jqgfzy.top

TS:   console.error("err")
来源：http://tng.daria6918.cn

Java: System.err.println("err")
来源：http://nwz.fanxiaobao.xyz

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://brg.nanxinkj.top

Ruby: warn "err"
来源：http://ipy.dashuyun.cn

C#:   Console.Error.WriteLine("err")
来源：http://wov.jqgfzy.top

[M07] 判断是否为主入口
来源：http://hpu.vqdsnc.cn

Py:   if __name__ == "__main__":
来源：http://zqo.mhx1999.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ngs.shuidangran.top

JS:   require.main === module
来源：http://azz.yueranfly.top

TS:   require.main === module
来源：http://ujv.sufxvd.cn

Java: public static void main(String[] args)
来源：http://rud.0kj1m.cn

Go:   func main()
来源：http://xdt.fktsv.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://dzq.ivvv.top

C#:   static void Main(string[] args)
来源：http://mss.yongpay.top

[M08] 获取系统与运行时信息
来源：http://ojr.jlsjyb.cn

Py:   platform.system();  platform.python_version()
来源：http://etf.vehdjk.com

PHP:  PHP_OS;  phpversion();
来源：http://bbd.gotoacloud.top

JS:   process.platform;  process.version
来源：http://jzq.jyoumei.cn

TS:   process.platform;  process.version
来源：http://vrb.wangdashe.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://nmc.vehdjk.com

Go:   runtime.GOOS;  runtime.Version()
来源：http://cxz.hammf.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://qwg.yvedp.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://ngi.zdbjq.cn

================================================================================
来源：http://nuz.ehwqpu.com

N. 数据结构与算法
来源：http://tag.ehwqpu.com

================================================================================
来源：http://xxn.zdbjq.cn

[N01] 二分查找（有序数组）
来源：http://tug.hysaishi.cn

Py:   bisect.bisect_left(arr, x)
来源：http://yzs.jlsjyb.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://fah.jqgfzy.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://shu.daxiang520.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://bkn.shuidangran.top

Java: Arrays.binarySearch(arr, x)
来源：http://jmw.yj202588.top

Go:   sort.SearchInts(arr, x)
来源：http://rss.dianchejie.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://pii.zycfv.cn

C#:   Array.BinarySearch(arr, x)
来源：http://dba.chenzaomai.com

[N02] 排序（工程实践用内置实现）
来源：http://tel.xziqi.cn

Py:   sorted(arr);  arr.sort()
来源：http://xhb.ivvv.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ehg.jlsjyb.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://phs.tanke756.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://cfj.9152youxi.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://yco.cashguo.top

Go:   slices.Sort(arr)
来源：http://rdv.pengpengdd.cyou

Ruby: arr.sort
来源：http://iut.ehwqpu.com

C#:   Array.Sort(arr);  list.Sort()
来源：http://bac.daria6918.cn

[N03] 快速排序（分治示例）
来源：http://jux.hnqzz.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://opc.gotoacloud.top

PHP:  // 递归实现，或用 usort
来源：http://hzx.dashuyun.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ews.tian-w.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hcs.xuetiantiany.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://rhx.dashuyun.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hdj.jianghu66.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://sdm.ppjwa.cn

C#:   // 手写递归，或 Array.Sort
来源：http://hqg.tian-w.cn

[N04] 斐波那契数列
来源：http://mus.jinyuanbaomall.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ibp.sweek.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://uzn.haohaochexian.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://gnm.vehdjk.com

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://cpa.jinqigufen.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mhh.fktsv.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://cyb.zhongyouzk.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://xan.fktsv.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://tzb.zhixingplan.top

[N05] 最大公约数
来源：http://jho.jyoumei.cn

Py:   math.gcd(a, b)
来源：http://bup.zdqjudy.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://gny.zycfv.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ixi.nwbrower.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://uwu.sufxvd.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://jby.tanke756.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://dvw.smart0.xyz

Ruby: a.gcd(b)
来源：http://bje.ybcxt.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://uzq.snrcjt.cn

[N06] 判断回文字符串
来源：http://wnh.yuxming.cn

Py:   s == s[::-1]
来源：http://hcc.sxryk.cn

PHP:  $s === strrev($s);
来源：http://xkd.gogol.net.cn

JS:   s === [...s].reverse().join("")
来源：http://ueb.yangfankeji.com

TS:   s === [...s].reverse().join("")
来源：http://xsw.zhongyouzk.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hyb.ctjpmb.com

Go:   // 双指针从两端比较
来源：http://sjm.fanxiaobao.xyz

Ruby: s == s.reverse
来源：http://usj.chenjidiqi.icu

C#:   s == new string(s.Reverse().ToArray())
来源：http://ihd.zdqjudy.top

[N07] 两数之和（返回下标）
来源：http://ozj.sjlbkw.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://zca.chenlongwang.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://bwj.yongpay.top

JS:   // 手写 Map：map.set(v, i)
来源：http://tqg.tarul.cn

TS:   // 手写 Map<string, number>
来源：http://dyo.guannengcc.top

Java: // 手写 HashMap
来源：http://yuj.bjfxy.top

Go:   // 手写 map[int]int
来源：http://lit.dashuyun.cn

Ruby: // 手写 Hash
来源：http://whm.jqgufenzy.top

C#:   // 手写 Dictionary<int, int>
来源：http://eyg.ydjk.org.cn

[N08] 生成全排列
来源：http://txv.mhx1999.top

Py:   itertools.permutations(arr)
来源：http://hol.andypj.xyz

PHP:  // 手写递归交换
来源：http://ypr.shanyushiyangkeji.top

JS:   // 手写回溯递归
来源：http://osi.nanxinkj.top

TS:   // 手写回溯递归
来源：http://psx.birdmap.top

Java: // 手写回溯递归
来源：http://wnn.daria6918.cn

Go:   // 手写回溯递归
来源：http://ccl.shangyingyoupin.top

Ruby: arr.permutation.to_a
来源：http://yzl.zhoulong.xyz

C#:   // 手写回溯递归
来源：http://yuq.ydjk.org.cn

[N09] 栈与队列
来源：http://weu.jianghu66.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://xyh.bbcook.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://xeo.ctjpmb.com

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://jnz.sufxvd.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ghm.ehwqpu.com

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://eip.zhongyouzk.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ops.zhengqikj.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://tih.yonumen.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mqt.quarkkingdee.top

[N10] 链表节点定义
来源：http://eij.shzxlz.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://rpm.hnxiangtu.top

PHP:  class Node { public $v; public $next = null; }
来源：http://bwx.guannengcc.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hzm.zycfv.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wez.tianlin.xyz

Java: class Node { int v; Node next; }
来源：http://img.tianlin.xyz

Go:   type Node struct { V int; Next *Node }
来源：http://dxz.jqgufenzy.top

Ruby: Node = Struct.new(:v, :next)
来源：http://vyw.jiagoushi.top

C#:   class Node { public int V; public Node? Next; }
来源：http://paf.bjfxy.top

[N11] 二叉树中序遍历
来源：http://ovs.hfpthk.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://jxr.shzxlz.cn

PHP:  // 手写递归函数
来源：http://fkx.yanxiufei.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://tdc.fanxiaobao.xyz

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://cjh.zdbjq.cn

Java: // 手写递归
来源：http://nav.guowangkeji.top

Go:   // 手写递归
来源：http://duu.smart0.xyz

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://nua.chenlongwang.top

C#:   // 手写递归
来源：http://kbb.yanxiufei.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://cog.meibo888.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://qgo.jinqigufen.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ufo.nwbrower.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://shu.ehwqpu.com

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://xwp.ppjwa.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://omc.tianlin.xyz

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hii.jinqigfzy.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://jsi.guannengcc.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://gos.fanxiaobao.xyz

================================================================================
来源：http://dgz.havefunace.top

O. 并发与异步
来源：http://aip.gotoacloud.top

================================================================================
来源：http://jrk.guowangkeji.top

[O01] 启动一个线程
来源：http://jwo.fzhhl.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://par.hongshengwenyu.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://svu.meibo888.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://yxs.zhaomingkeji.xyz

TS:   // 同 JS
来源：http://tts.gzhubu.top

Java: new Thread(() -> f()).start()
来源：http://blo.0kj1m.cn

Go:   go f()
来源：http://hqf.zycfv.cn

Ruby: Thread.new { f }
来源：http://bgt.zhijiandao.cn

C#:   Task.Run(() => F());
来源：http://soe.shuidangran.top

[O02] 使用线程池
来源：http://qya.zhongyouzk.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://tll.hesvh.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ppf.wangshuangyany.cn

JS:   // worker_threads 线程池
来源：http://iwh.nanxinkj.top

TS:   // worker_threads 线程池
来源：http://iyg.bjfxy.top

Java: Executors.newFixedThreadPool(4)
来源：http://apv.gaohongyu789.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://rov.yongpay.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ufr.9152youxi.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://xug.meibo888.top

[O03] 加锁保护共享数据
来源：http://pmw.tarul.cn

Py:   with lock: shared += 1
来源：http://zjl.sxryk.cn

PHP:  // 用 flock() 做文件锁
来源：http://qju.cheryme.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://jpu.jlsjyb.cn

TS:   // 同 JS
来源：http://ugp.ywan-chungtsiang.top

Java: synchronized (this) { shared++; }
来源：http://bvm.xingfuxueyuan.xyz

Go:   mu.Lock();  defer mu.Unlock()
来源：http://yfb.havefunace.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://rhx.haohaochexian.top

C#:   lock (gate) { shared++; }
来源：http://ogb.xylfe.cn

[O04] 定义异步函数并等待
来源：http://zva.0kj1m.cn

Py:   async def f():⏎    await g()
来源：http://nsk.sxryk.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://qya.sweek.top

JS:   async function f() { await g(); }
来源：http://whu.vehdjk.com

TS:   async function f(): Promise<void> { await g(); }
来源：http://ije.wangshuangyany.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://cgo.shangyingyoupin.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://bno.birdmap.top

Ruby: # 用 Fiber 或 async gem
来源：http://kol.zhixingplan.top

C#:   async Task F() { await G(); }
来源：http://mft.shuidangran.top

[O05] 并发执行并等待全部完成
来源：http://xjc.zhiwuduotai.top


<!-- 参考信息 -->