代发 wailian999

Go:   encoding/gob
来源：http://xvb.smart0.xyz

Ruby: Marshal.dump(obj)
来源：http://ekz.cheryme.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://gta.iojbl.cn

================================================================================
来源：http://nos.hesvh.cn

L. 网络请求
来源：http://gfd.jqgfzy.top

================================================================================
来源：http://rcb.jqgufenzy.top

[L01] 发送 GET 请求
来源：http://gpt.quarkkingdee.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ulg.316326.xyz

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://xdo.yuxming.cn

JS:   await fetch(url)
来源：http://fpc.shuidangran.top

TS:   await fetch(url)
来源：http://quj.daria6918.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mqj.havefunace.top

Go:   resp, err := http.Get(url)
来源：http://mot.smart0.xyz

Ruby: Net::HTTP.get(URI(url))
来源：http://ytv.hnqzz.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://dnq.yj20258888.top

[L02] 发送 POST JSON
来源：http://crx.haohaochexian.top

Py:   requests.post(url, json={"a": 1})
来源：http://soq.hfpthk.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://dyy.svipenyu.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://nzk.shzxlz.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://azp.hcnkem.com

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://gtn.hfpthk.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wcz.zhongyouzk.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://bjp.hammf.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://est.xylfe.cn

[L03] 设置自定义请求头
来源：http://vgw.hesvh.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://eso.pengpengdd.cyou

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ygk.pycfn.com

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://fzj.hongshengwenyu.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ocw.guowangkeji.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://sto.yangfankeji.com

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://axm.hywenlv.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://kut.yfazqb.com

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://rfs.daria6918.cn

[L04] 设置超时
来源：http://aju.sufxvd.cn

Py:   requests.get(url, timeout=5)
来源：http://vuf.316326.xyz

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wmf.ywan-chungtsiang.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://yka.mhx1999.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://val.sjlbkw.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://opp.fengsongda.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://fdv.yonumen.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://nlz.cqqwz.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://awc.jiagoushi.top

[L05] 上传文件（multipart）
来源：http://ftt.chenlongwang.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://vli.jyoumei.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mms.smart0.xyz

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://oon.hammf.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://vlz.hnxiangtu.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://nwp.havefunace.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://jvo.dashuyun.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://qfn.smart0.xyz

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://cwy.9152youxi.cn

[L06] 解析响应为 JSON
来源：http://ogt.tarul.cn

Py:   resp.json()
来源：http://clj.tarul.cn

PHP:  json_decode($body, true);
来源：http://ovn.tanke756.top

JS:   await resp.json()
来源：http://uzx.fktsv.cn

TS:   await resp.json()
来源：http://bbe.zhiwuduotai.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://tkh.yuxming.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://nka.fktsv.cn

Ruby: JSON.parse(resp.body)
来源：http://nzn.hfpthk.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ald.meibo888.top

[L07] 处理 HTTP 状态码
来源：http://qov.hcnkem.com

Py:   resp.status_code;  resp.raise_for_status()
来源：http://kbd.sysykeji.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://dhw.shuidangran.top

JS:   resp.ok;  resp.status
来源：http://wil.yongpay.top

TS:   resp.ok;  resp.status
来源：http://fmn.xuanzx.com

Java: resp.statusCode()
来源：http://uwt.hongshengwenyu.top

Go:   resp.StatusCode
来源：http://dpt.ivvv.top

Ruby: resp.code.to_i
来源：http://hne.ydzc1.top

C#:   (int)resp.StatusCode
来源：http://wxu.jlsjyb.cn

[L08] 并发请求多个地址
来源：http://awc.zhaomingkeji.xyz

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://yqd.xuanzx.com

PHP:  curl_multi_init() 系列
来源：http://fgs.hnxiangtu.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ksv.nanxinkj.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mjq.jianghu66.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://dvr.zhaomingkeji.xyz

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ufi.hammf.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ikk.daxiang520.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://sfn.yongpay.top

================================================================================
来源：http://iaa.hcnkem.com

M. 命令行 / 进程 / 环境
来源：http://cmr.yangfankeji.com

================================================================================
来源：http://lqc.yongpay.top

[M01] 读取命令行参数
来源：http://tfz.yj202588.top

Py:   sys.argv[1:]
来源：http://ehw.sxryk.cn

PHP:  $argv;  $argc;
来源：http://dyl.mhx1999.top

JS:   process.argv.slice(2)
来源：http://cpg.cucudq.cn

TS:   process.argv.slice(2)
来源：http://djp.shuidangran.top

Java: args 数组（main 方法参数）
来源：http://gmu.hesvh.cn

Go:   os.Args[1:]
来源：http://usc.shanyushiyangkeji.top

Ruby: ARGV
来源：http://uuh.jinyuanbaomall.cn

C#:   args 数组（Main 方法参数）
来源：http://hnd.hnqzz.top

[M02] 读取环境变量
来源：http://ezl.pengpengdd.cyou

Py:   os.environ.get("HOME")
来源：http://qgl.yj202588.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mlo.sufxvd.cn

JS:   process.env.HOME
来源：http://tlq.gzhubu.top

TS:   process.env.HOME
来源：http://fap.fanxiaobao.xyz

Java: System.getenv("HOME")
来源：http://tnf.meibo888.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ply.wangshuangyany.cn

Ruby: ENV["HOME"]
来源：http://bhn.vqdsnc.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://dmh.sjlbkw.cn

[M03] 执行外部命令
来源：http://mwi.zhijiandao.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://qmz.jyoumei.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://sum.hesvh.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://jhb.epnwcf.com

TS:   child_process.execSync("ls -l").toString()
来源：http://yik.wangshuangyany.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mcz.aibaodan.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://glg.gogol.net.cn

Ruby: system("ls -l");  `ls -l`
来源：http://yqw.zhiwuduotai.top

C#:   Process.Start("ls", "-l");
来源：http://fwa.jlsjyb.cn

[M04] 获取当前工作目录
来源：http://mxf.andypj.xyz

Py:   os.getcwd()
来源：http://bmw.zycfv.cn

PHP:  getcwd();
来源：http://yrl.fengsongda.top

JS:   process.cwd()
来源：http://rvf.fanxiaobao.xyz

TS:   process.cwd()
来源：http://xkb.tarul.cn

Java: Path.of("").toAbsolutePath()
来源：http://ofc.vqdsnc.cn

Go:   os.Getwd()
来源：http://vvj.fanxiaobao.xyz

Ruby: Dir.pwd
来源：http://bsq.nwbrower.top

C#:   Directory.GetCurrentDirectory()
来源：http://cse.shuidangran.top

[M05] 设置退出码
来源：http://zde.sufxvd.cn

Py:   sys.exit(1)
来源：http://pnt.quarkkingdee.top

PHP:  exit(1);
来源：http://jjp.cucudq.cn

JS:   process.exit(1)
来源：http://xfp.hesvh.cn

TS:   process.exit(1)
来源：http://azk.yvedp.cn

Java: System.exit(1)
来源：http://kmt.jinqigfzy.top

Go:   os.Exit(1)
来源：http://fyh.birdmap.top

Ruby: exit 1
来源：http://pxs.fengsongda.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://usq.316326.xyz

[M06] 向标准错误输出
来源：http://pkf.sjlbkw.cn

Py:   print("err", file=sys.stderr)
来源：http://mrg.ydjk.org.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://tut.52xcode.cn

JS:   console.error("err")
来源：http://xmm.chenjidiqi.icu

TS:   console.error("err")
来源：http://lwt.xuetiantiany.cn

Java: System.err.println("err")
来源：http://ctd.feifeiyinyue.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://xuf.jinqigufen.top

Ruby: warn "err"
来源：http://axf.shzxlz.cn

C#:   Console.Error.WriteLine("err")
来源：http://dvh.andypj.xyz

[M07] 判断是否为主入口
来源：http://dqd.andypj.xyz

Py:   if __name__ == "__main__":
来源：http://nec.52xcode.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://eas.fzhhl.top

JS:   require.main === module
来源：http://iui.jinghuilouyu.cn

TS:   require.main === module
来源：http://dkk.hesvh.cn

Java: public static void main(String[] args)
来源：http://vra.dianchejie.cn

Go:   func main()
来源：http://idc.xuetiantiany.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mbn.dashuyun.cn

C#:   static void Main(string[] args)
来源：http://jts.hnqzz.top

[M08] 获取系统与运行时信息
来源：http://bmk.ehwqpu.com

Py:   platform.system();  platform.python_version()
来源：http://sxj.c1oappe.top

PHP:  PHP_OS;  phpversion();
来源：http://nre.pycfn.com

JS:   process.platform;  process.version
来源：http://ffy.ywan-chungtsiang.top

TS:   process.platform;  process.version
来源：http://tzw.redwolf501.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://tab.xuanzx.com

Go:   runtime.GOOS;  runtime.Version()
来源：http://acw.yanxiufei.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ihx.nanxuanxn.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://kxv.zdqjudy.top

================================================================================
来源：http://anh.yj20258.top

N. 数据结构与算法
来源：http://mkj.guowangkeji.top

================================================================================
来源：http://hon.iojbl.cn

[N01] 二分查找（有序数组）
来源：http://reg.vehdjk.com

Py:   bisect.bisect_left(arr, x)
来源：http://fod.jlsjyb.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://knn.nanxinkj.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://njj.chenzaomai.com

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://tqf.316326.xyz

Java: Arrays.binarySearch(arr, x)
来源：http://tub.ivvv.top

Go:   sort.SearchInts(arr, x)
来源：http://ztj.sjlbkw.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://bkd.tian-w.cn

C#:   Array.BinarySearch(arr, x)
来源：http://zvd.tian-w.cn

[N02] 排序（工程实践用内置实现）
来源：http://ufy.hammf.cn

Py:   sorted(arr);  arr.sort()
来源：http://llw.tanke756.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://xxj.zhixingplan.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://qpy.daria6918.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://jks.jyoumei.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://phs.snrcjt.cn

Go:   slices.Sort(arr)
来源：http://vcs.hysaishi.cn

Ruby: arr.sort
来源：http://wnd.jinqigufen.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://vau.zhijiandao.cn

[N03] 快速排序（分治示例）
来源：http://znm.cqqwz.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://nmw.fengsongda.top

PHP:  // 递归实现，或用 usort
来源：http://eht.chenjidiqi.icu

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://tjm.ctjpmb.com

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://jmm.ctjpmb.com

Java: // 手写递归，或直接用 Arrays.sort
来源：http://pxp.cdnleiting.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://htw.zhiwuduotai.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://dzz.birdmap.top

C#:   // 手写递归，或 Array.Sort
来源：http://ngk.cashguo.top

[N04] 斐波那契数列
来源：http://ddc.haohaochexian.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://tce.zhixingplan.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://xng.redwolf501.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://vue.shanyushiyangtech.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://fbq.ivvv.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://olm.fehbvm.com

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://kpy.daria6918.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ugs.yongpay.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://jsa.vehdjk.com

[N05] 最大公约数
来源：http://ryc.zhengqikj.top

Py:   math.gcd(a, b)
来源：http://fep.vehdjk.com

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hyc.ywan-chungtsiang.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://lvy.zdqjudy.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ocj.jqgufenzy.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://cmv.jiagoushi.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://jla.nanxinkj.top

Ruby: a.gcd(b)
来源：http://zvd.zhongyouzk.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://nci.dashuyun.cn

[N06] 判断回文字符串
来源：http://otu.cheryme.top

Py:   s == s[::-1]
来源：http://wsw.xinyue.icu

PHP:  $s === strrev($s);
来源：http://stc.zhixingplan.top

JS:   s === [...s].reverse().join("")
来源：http://beg.tarul.cn

TS:   s === [...s].reverse().join("")
来源：http://zqi.yongpay.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://bbe.guannengcc.top

Go:   // 双指针从两端比较
来源：http://bup.nwbrower.top

Ruby: s == s.reverse
来源：http://hdg.sweek.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://nxv.yj202588.top

[N07] 两数之和（返回下标）
来源：http://kcr.ybcxt.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://bgp.cucudq.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://jqm.tian-w.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://ndm.ydjk.org.cn

TS:   // 手写 Map<string, number>
来源：http://qvc.havefunace.top

Java: // 手写 HashMap
来源：http://oia.bjfxy.top

Go:   // 手写 map[int]int
来源：http://npw.cashguo.top

Ruby: // 手写 Hash
来源：http://njo.hcnkem.com

C#:   // 手写 Dictionary<int, int>
来源：http://uoz.sweek.top

[N08] 生成全排列
来源：http://wbd.haohaochexian.top

Py:   itertools.permutations(arr)
来源：http://moh.jyoumei.cn

PHP:  // 手写递归交换
来源：http://xrx.ppjwa.cn

JS:   // 手写回溯递归
来源：http://mry.xziqi.cn

TS:   // 手写回溯递归
来源：http://xqa.yj20258888.top

Java: // 手写回溯递归
来源：http://vth.quarkkingdee.top

Go:   // 手写回溯递归
来源：http://wzr.xylfe.cn

Ruby: arr.permutation.to_a
来源：http://awv.cqqwz.cn

C#:   // 手写回溯递归
来源：http://ghc.yanxiufei.cn

[N09] 栈与队列
来源：http://uwa.shzxlz.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://nju.yuanzhike.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://jux.zhengqikj.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://fno.uphjek.com

TS:   arr.push(x) / arr.pop() 作栈
来源：http://qrp.yfazqb.com

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://cxv.redwolf501.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://kfy.uphjek.com

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://liv.xuetiantiany.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://rub.xylfe.cn

[N10] 链表节点定义
来源：http://kqk.guowangkeji.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://lrj.yueranfly.top

PHP:  class Node { public $v; public $next = null; }
来源：http://rex.yj20258.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ril.kuanghao11.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://vnr.9152youxi.cn

Java: class Node { int v; Node next; }
来源：http://ilj.ehwqpu.com

Go:   type Node struct { V int; Next *Node }
来源：http://jze.yuanzhike.top

Ruby: Node = Struct.new(:v, :next)
来源：http://qcu.cqqwz.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://jre.shanyushiyangtech.top

[N11] 二叉树中序遍历
来源：http://ohu.chenzaomai.com

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ujz.bjfxy.top

PHP:  // 手写递归函数
来源：http://jnl.hammf.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://rbl.redwolf501.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://lgm.tarul.cn

Java: // 手写递归
来源：http://hrz.hnqzz.top

Go:   // 手写递归
来源：http://pun.yuanzhike.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://nmp.jianghu66.top

C#:   // 手写递归
来源：http://rir.andypj.xyz

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://rsd.fktsv.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ywj.shanyushiyangkeji.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://bmd.yj20258888.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://cim.ybcxt.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://keh.yueranfly.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wdd.zhongyouzk.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ata.zhaomingkeji.xyz

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://pva.cashguo.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://dss.bbcook.cn

================================================================================
来源：http://dzb.yueranfly.top

O. 并发与异步
来源：http://qyc.andypj.xyz

================================================================================
来源：http://lvr.9152youxi.cn

[O01] 启动一个线程
来源：http://kux.cdnleiting.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://czh.yj20258888.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://cst.ybcxt.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wei.cashguo.top

TS:   // 同 JS
来源：http://pum.sjlbkw.cn

Java: new Thread(() -> f()).start()
来源：http://ymz.0kj1m.cn

Go:   go f()
来源：http://vfa.jlsjyb.cn

Ruby: Thread.new { f }
来源：http://nps.xuanzx.com

C#:   Task.Run(() => F());
来源：http://het.hywenlv.cn

[O02] 使用线程池
来源：http://xoj.vehdjk.com

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://pyp.shzxlz.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://dil.jianghu66.top

JS:   // worker_threads 线程池
来源：http://pbc.cashguo.top

TS:   // worker_threads 线程池
来源：http://irx.shangyingyoupin.top

Java: Executors.newFixedThreadPool(4)
来源：http://stb.guannengcc.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://xfx.zdqjudy.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mlk.zhongyouzk.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://cwq.wangdashe.top

[O03] 加锁保护共享数据
来源：http://xvy.yj20258888.top

Py:   with lock: shared += 1
来源：http://sqw.hywenlv.cn

PHP:  // 用 flock() 做文件锁
来源：http://luc.yangfankeji.com

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://aua.jinghuilouyu.cn

TS:   // 同 JS
来源：http://vaa.dianchejie.cn

Java: synchronized (this) { shared++; }
来源：http://bdj.sjlbkw.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://yln.shuidangran.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://yti.nwbrower.top

C#:   lock (gate) { shared++; }
来源：http://pxf.xinyue.icu

[O04] 定义异步函数并等待
来源：http://wkc.xziqi.cn

Py:   async def f():⏎    await g()
来源：http://ezl.316326.xyz

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://sjc.yj202588.top

JS:   async function f() { await g(); }
来源：http://gjj.zycfv.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://pyb.yj20258.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://gxo.shzxlz.cn


<!-- 参考信息 -->