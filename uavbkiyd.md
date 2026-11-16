代发 wailian999

L. 网络请求
来源：http://ggh.cashguo.top

================================================================================
来源：http://qzx.aibaodan.cn

[L01] 发送 GET 请求
来源：http://uba.fehbvm.com

Py:   requests.get(url)                        # 第三方库 requests
来源：http://fum.jyoumei.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hyu.zhijiandao.cn

JS:   await fetch(url)
来源：http://fnh.yvedp.cn

TS:   await fetch(url)
来源：http://oho.shangyingyoupin.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://cqd.cashguo.top

Go:   resp, err := http.Get(url)
来源：http://nat.yuxming.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://gnp.ybcxt.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://tww.daria6918.cn

[L02] 发送 POST JSON
来源：http://juv.sxryk.cn

Py:   requests.post(url, json={"a": 1})
来源：http://ahb.yongpay.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://vgc.hysaishi.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://vbf.jianghu66.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://tbj.nwbrower.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://qav.aizwys.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://vph.haohaochexian.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://eow.aizwys.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://vyx.yuanzhike.top

[L03] 设置自定义请求头
来源：http://pgt.jlsjyb.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://jii.wangshuangyany.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://jie.fanxiaobao.xyz

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://qrk.xinyue.icu

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://jym.chenjidiqi.icu

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://rdv.jinghuilouyu.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://rmw.gaohongyu789.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://uaw.mhx1999.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mjz.wangshuangyany.cn

[L04] 设置超时
来源：http://kkv.yuanzhike.top

Py:   requests.get(url, timeout=5)
来源：http://rbt.meibo888.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://znm.kuanghao11.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mjv.havefunace.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mms.cqqwz.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://kmv.ybcxt.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://qzo.jianghu66.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://zpu.feifeiyinyue.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://okg.52xcode.cn

[L05] 上传文件（multipart）
来源：http://uvw.gzhubu.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://dhm.ybcxt.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://gbm.chenjidiqi.icu

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://eeq.havefunace.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://qsb.gzhubu.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://rez.yanxiufei.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://izw.chenjidiqi.icu

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://yzw.wangdashe.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hzn.hywenlv.cn

[L06] 解析响应为 JSON
来源：http://dss.tanke756.top

Py:   resp.json()
来源：http://bjx.vqdsnc.cn

PHP:  json_decode($body, true);
来源：http://epq.hesvh.cn

JS:   await resp.json()
来源：http://hza.zhijiandao.cn

TS:   await resp.json()
来源：http://vpm.hcnkem.com

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://edf.fehbvm.com

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://gxm.fanxiaobao.xyz

Ruby: JSON.parse(resp.body)
来源：http://isg.daria6918.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://xfa.hnqzz.top

[L07] 处理 HTTP 状态码
来源：http://lva.pengpengdd.cyou

Py:   resp.status_code;  resp.raise_for_status()
来源：http://fba.sjlbkw.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://fer.yj20258.top

JS:   resp.ok;  resp.status
来源：http://kfs.jqgufenzy.top

TS:   resp.ok;  resp.status
来源：http://lcd.wangshuangyany.cn

Java: resp.statusCode()
来源：http://ylu.hesvh.cn

Go:   resp.StatusCode
来源：http://ots.ivvv.top

Ruby: resp.code.to_i
来源：http://gsr.sxryk.cn

C#:   (int)resp.StatusCode
来源：http://tda.sweek.top

[L08] 并发请求多个地址
来源：http://mdq.ydjk.org.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wye.tarul.cn

PHP:  curl_multi_init() 系列
来源：http://mgj.ctjpmb.com

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ixp.shangyingyoupin.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://kpu.hnqzz.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://iwi.ivvv.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://oui.chenjidiqi.icu

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://rvs.xinyue.icu

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://xxt.shanyushiyangkeji.top

================================================================================
来源：http://bpn.snrcjt.cn

M. 命令行 / 进程 / 环境
来源：http://hsp.ydzc1.top

================================================================================
来源：http://zvo.52xcode.cn

[M01] 读取命令行参数
来源：http://oqj.zdbjq.cn

Py:   sys.argv[1:]
来源：http://yzo.zhixingplan.top

PHP:  $argv;  $argc;
来源：http://qmt.zhengqikj.top

JS:   process.argv.slice(2)
来源：http://swk.jinqigufen.top

TS:   process.argv.slice(2)
来源：http://ali.aibaodan.cn

Java: args 数组（main 方法参数）
来源：http://nov.nanxinkj.top

Go:   os.Args[1:]
来源：http://tve.xingfuxueyuan.xyz

Ruby: ARGV
来源：http://xcz.yj20258.top

C#:   args 数组（Main 方法参数）
来源：http://fdc.cqqwz.cn

[M02] 读取环境变量
来源：http://lhz.zdbjq.cn

Py:   os.environ.get("HOME")
来源：http://kcz.yangfankeji.com

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://awf.feifeiyinyue.top

JS:   process.env.HOME
来源：http://pzs.tarul.cn

TS:   process.env.HOME
来源：http://vpj.feifeiyinyue.top

Java: System.getenv("HOME")
来源：http://dqi.shanyushiyangtech.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://nai.tian-w.cn

Ruby: ENV["HOME"]
来源：http://jbo.birdmap.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://cwx.ctjpmb.com

[M03] 执行外部命令
来源：http://vlk.sjlbkw.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://fzf.cheryme.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://kis.jqgufenzy.top

JS:   child_process.execSync("ls -l").toString()
来源：http://tpa.xuetiantiany.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://axz.jinyuanbaomall.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://zni.cucudq.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://laj.ydjk.org.cn

Ruby: system("ls -l");  `ls -l`
来源：http://uos.sysykeji.top

C#:   Process.Start("ls", "-l");
来源：http://krf.sufxvd.cn

[M04] 获取当前工作目录
来源：http://aqd.hnqzz.top

Py:   os.getcwd()
来源：http://iqf.shanyushiyangkeji.top

PHP:  getcwd();
来源：http://mas.cqqwz.cn

JS:   process.cwd()
来源：http://wod.snrcjt.cn

TS:   process.cwd()
来源：http://ene.ywan-chungtsiang.top

Java: Path.of("").toAbsolutePath()
来源：http://pgw.yonumen.top

Go:   os.Getwd()
来源：http://als.jyoumei.cn

Ruby: Dir.pwd
来源：http://zqc.jiagoushi.top

C#:   Directory.GetCurrentDirectory()
来源：http://oal.xingfuxueyuan.xyz

[M05] 设置退出码
来源：http://qyq.ppjwa.cn

Py:   sys.exit(1)
来源：http://pni.epnwcf.com

PHP:  exit(1);
来源：http://yoi.zdqjudy.top

JS:   process.exit(1)
来源：http://ygc.yonumen.top

TS:   process.exit(1)
来源：http://aro.xylfe.cn

Java: System.exit(1)
来源：http://opm.uphjek.com

Go:   os.Exit(1)
来源：http://hub.jqgufenzy.top

Ruby: exit 1
来源：http://jtn.gotoacloud.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wql.vqdsnc.cn

[M06] 向标准错误输出
来源：http://mna.bbcook.cn

Py:   print("err", file=sys.stderr)
来源：http://mkp.pycfn.com

PHP:  fwrite(STDERR, "err\n");
来源：http://isc.tianlin.xyz

JS:   console.error("err")
来源：http://wch.yj202588.top

TS:   console.error("err")
来源：http://esn.cucudq.cn

Java: System.err.println("err")
来源：http://gtj.svipenyu.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mdd.hongshengwenyu.top

Ruby: warn "err"
来源：http://fwy.fzhhl.top

C#:   Console.Error.WriteLine("err")
来源：http://sha.hysaishi.cn

[M07] 判断是否为主入口
来源：http://bqd.sxryk.cn

Py:   if __name__ == "__main__":
来源：http://dyx.bjfxy.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ujt.haohaochexian.top

JS:   require.main === module
来源：http://wmy.9152youxi.cn

TS:   require.main === module
来源：http://dhs.bjfxy.top

Java: public static void main(String[] args)
来源：http://bww.kuanghao11.cn

Go:   func main()
来源：http://fpt.gotoacloud.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://jvd.xingfuxueyuan.xyz

C#:   static void Main(string[] args)
来源：http://kuq.shanyushiyangkeji.top

[M08] 获取系统与运行时信息
来源：http://tjb.ydzc1.top

Py:   platform.system();  platform.python_version()
来源：http://nue.haohaochexian.top

PHP:  PHP_OS;  phpversion();
来源：http://ucp.aibaodan.cn

JS:   process.platform;  process.version
来源：http://rpx.smart0.xyz

TS:   process.platform;  process.version
来源：http://prp.fktsv.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ncq.tarul.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://pey.meibo888.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://tzi.jinghuilouyu.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://aii.vehdjk.com

================================================================================
来源：http://gjk.fzhhl.top

N. 数据结构与算法
来源：http://aiu.tian-w.cn

================================================================================
来源：http://nsu.shanyushiyangtech.top

[N01] 二分查找（有序数组）
来源：http://bgx.yonumen.top

Py:   bisect.bisect_left(arr, x)
来源：http://sfu.hnxiangtu.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://gag.jinyuanbaomall.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://rum.jianghu66.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://tbq.yueranfly.top

Java: Arrays.binarySearch(arr, x)
来源：http://hoh.cdnleiting.top

Go:   sort.SearchInts(arr, x)
来源：http://nzb.xinyue.icu

Ruby: arr.bsearch { |e| e >= x }
来源：http://aau.cucudq.cn

C#:   Array.BinarySearch(arr, x)
来源：http://lzw.wangshuangyany.cn

[N02] 排序（工程实践用内置实现）
来源：http://jsp.sysykeji.top

Py:   sorted(arr);  arr.sort()
来源：http://yav.nanxinkj.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://odw.hammf.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://xhd.yanxiufei.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://fnj.ydzc1.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://szz.hcnkem.com

Go:   slices.Sort(arr)
来源：http://izm.hnxiangtu.top

Ruby: arr.sort
来源：http://xbb.pycfn.com

C#:   Array.Sort(arr);  list.Sort()
来源：http://tgx.jinghuilouyu.cn

[N03] 快速排序（分治示例）
来源：http://kmv.gotoacloud.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://pqm.fehbvm.com

PHP:  // 递归实现，或用 usort
来源：http://qqw.yj20258888.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://xlf.jianghu66.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://dpr.pengpengdd.cyou

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mtt.yvedp.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://kif.cdnleiting.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://xoz.tanke756.top

C#:   // 手写递归，或 Array.Sort
来源：http://csx.yfazqb.com

[N04] 斐波那契数列
来源：http://xss.chenzaomai.com

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://cdc.fengsongda.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hck.cqqwz.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mik.mhx1999.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://eye.cheryme.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://kwh.ywan-chungtsiang.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://lyk.zycfv.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://kbu.vehdjk.com

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://vhj.yanxiufei.cn

[N05] 最大公约数
来源：http://ntc.daria6918.cn

Py:   math.gcd(a, b)
来源：http://jwj.sysykeji.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://onz.cucudq.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://jip.uphjek.com

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://tqk.shzxlz.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://pez.smart0.xyz

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://nim.sysykeji.top

Ruby: a.gcd(b)
来源：http://nxx.epnwcf.com

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://xxn.hysaishi.cn

[N06] 判断回文字符串
来源：http://duw.hysaishi.cn

Py:   s == s[::-1]
来源：http://dac.aibaodan.cn

PHP:  $s === strrev($s);
来源：http://ftl.ywan-chungtsiang.top

JS:   s === [...s].reverse().join("")
来源：http://jkg.c1oappe.top

TS:   s === [...s].reverse().join("")
来源：http://omw.shanyushiyangtech.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wlw.jqgfzy.top

Go:   // 双指针从两端比较
来源：http://qct.havefunace.top

Ruby: s == s.reverse
来源：http://lbj.tarul.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://edm.jyoumei.cn

[N07] 两数之和（返回下标）
来源：http://fmg.aizwys.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://yfd.sjlbkw.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://kzs.ehwqpu.com

JS:   // 手写 Map：map.set(v, i)
来源：http://ifl.sxryk.cn

TS:   // 手写 Map<string, number>
来源：http://xsu.jinghuilouyu.cn

Java: // 手写 HashMap
来源：http://lxn.feifeiyinyue.top

Go:   // 手写 map[int]int
来源：http://ueh.nanxinkj.top

Ruby: // 手写 Hash
来源：http://oit.sjlbkw.cn

C#:   // 手写 Dictionary<int, int>
来源：http://mlj.yuxming.cn

[N08] 生成全排列
来源：http://urt.yueranfly.top

Py:   itertools.permutations(arr)
来源：http://jaf.quarkkingdee.top

PHP:  // 手写递归交换
来源：http://bes.daxiang520.top

JS:   // 手写回溯递归
来源：http://sin.wangdashe.top

TS:   // 手写回溯递归
来源：http://mxf.mhx1999.top

Java: // 手写回溯递归
来源：http://sya.yonumen.top

Go:   // 手写回溯递归
来源：http://feh.yj202588.top

Ruby: arr.permutation.to_a
来源：http://uof.sufxvd.cn

C#:   // 手写回溯递归
来源：http://sjg.9152youxi.cn

[N09] 栈与队列
来源：http://crb.epnwcf.com

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://lnz.tianlin.xyz

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://zkb.gogol.net.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wkx.sufxvd.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://uid.ehwqpu.com

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://rlc.sjlbkw.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://dkn.wangdashe.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://qhn.sjlbkw.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://thp.zycfv.cn

[N10] 链表节点定义
来源：http://gdd.hcnkem.com

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://sfs.yj20258.top

PHP:  class Node { public $v; public $next = null; }
来源：http://jtk.ppjwa.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://aqx.zhixingplan.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://yfs.uphjek.com

Java: class Node { int v; Node next; }
来源：http://wgz.havefunace.top

Go:   type Node struct { V int; Next *Node }
来源：http://lle.pengpengdd.cyou

Ruby: Node = Struct.new(:v, :next)
来源：http://mgn.cqqwz.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://psa.jianghu66.top

[N11] 二叉树中序遍历
来源：http://mjl.cheryme.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://qzc.jlsjyb.cn

PHP:  // 手写递归函数
来源：http://ffe.fehbvm.com

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://nnx.wangshuangyany.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://flx.wangshuangyany.cn

Java: // 手写递归
来源：http://yhs.mhx1999.top

Go:   // 手写递归
来源：http://qxp.guannengcc.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://fje.tian-w.cn

C#:   // 手写递归
来源：http://rra.fengsongda.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://rui.sjlbkw.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://zfc.zycfv.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://vla.shzxlz.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://fft.jiagoushi.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://cqd.smart0.xyz

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://umx.zhongyouzk.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://qef.zhaomingkeji.xyz

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://dbl.pengpengdd.cyou

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://qyy.quarkkingdee.top

================================================================================
来源：http://idx.cashguo.top

O. 并发与异步
来源：http://jxm.52xcode.cn

================================================================================
来源：http://lkm.kuanghao11.cn

[O01] 启动一个线程
来源：http://uho.xingfuxueyuan.xyz

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://rsr.meibo888.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hrt.ehwqpu.com

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://rkt.hfpthk.cn

TS:   // 同 JS
来源：http://djp.hysaishi.cn

Java: new Thread(() -> f()).start()
来源：http://udy.hfpthk.cn

Go:   go f()
来源：http://jjx.tian-w.cn

Ruby: Thread.new { f }
来源：http://xwc.bbcook.cn

C#:   Task.Run(() => F());
来源：http://ajy.nanxinkj.top

[O02] 使用线程池
来源：http://fow.shangyingyoupin.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://epn.jianghu66.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ycu.c1oappe.top

JS:   // worker_threads 线程池
来源：http://kca.iojbl.cn

TS:   // worker_threads 线程池
来源：http://zhz.fanxiaobao.xyz

Java: Executors.newFixedThreadPool(4)
来源：http://vsn.yuxming.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://uuy.hnqzz.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://skp.chenlongwang.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://oql.dianchejie.cn

[O03] 加锁保护共享数据
来源：http://uhr.snrcjt.cn

Py:   with lock: shared += 1
来源：http://lpu.jyoumei.cn

PHP:  // 用 flock() 做文件锁
来源：http://ryo.yanxiufei.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mak.daxiang520.top

TS:   // 同 JS
来源：http://kki.daxiang520.top

Java: synchronized (this) { shared++; }
来源：http://zcn.ydjk.org.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://uqy.wangdashe.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://kvp.zhixingplan.top

C#:   lock (gate) { shared++; }
来源：http://nbz.shanyushiyangkeji.top

[O04] 定义异步函数并等待
来源：http://omf.kuanghao11.cn

Py:   async def f():⏎    await g()
来源：http://ouo.jiagoushi.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://xcq.andypj.xyz

JS:   async function f() { await g(); }
来源：http://jdh.nwbrower.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://zjj.jinqigufen.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://fcf.jqgfzy.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://nij.pengpengdd.cyou

Ruby: # 用 Fiber 或 async gem
来源：http://iqk.xingfuxueyuan.xyz

C#:   async Task F() { await G(); }
来源：http://auc.xylfe.cn

[O05] 并发执行并等待全部完成
来源：http://bok.nanxinkj.top


<!-- 参考信息 -->