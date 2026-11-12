代发 wailian999

Go:   encoding/gob
来源：http://pbv.shuidangran.top

Ruby: Marshal.dump(obj)
来源：http://fze.bbcook.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://weu.shzxlz.cn

================================================================================
来源：http://wob.yvedp.cn

L. 网络请求
来源：http://pry.havefunace.top

================================================================================
来源：http://wfq.sysykeji.top

[L01] 发送 GET 请求
来源：http://egd.gaohongyu789.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ghy.zhijiandao.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://gyn.ywan-chungtsiang.top

JS:   await fetch(url)
来源：http://kbz.wangdashe.top

TS:   await fetch(url)
来源：http://jta.mhx1999.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://vfa.fengsongda.top

Go:   resp, err := http.Get(url)
来源：http://xll.pengpengdd.cyou

Ruby: Net::HTTP.get(URI(url))
来源：http://cve.daxiang520.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://olg.cashguo.top

[L02] 发送 POST JSON
来源：http://yas.sjlbkw.cn

Py:   requests.post(url, json={"a": 1})
来源：http://jrg.ppjwa.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://elx.havefunace.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ezw.ctjpmb.com

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://qvm.jinqigfzy.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://jgr.ywan-chungtsiang.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://vkn.ivvv.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://qjn.tanke756.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://vhw.daxiang520.top

[L03] 设置自定义请求头
来源：http://uyc.yuxming.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://byy.zdbjq.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ecw.sysykeji.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wwv.jlsjyb.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://qxx.quarkkingdee.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://yws.sysykeji.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://lqh.yj20258888.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://elb.jqgufenzy.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://xyg.yfazqb.com

[L04] 设置超时
来源：http://yex.dianchejie.cn

Py:   requests.get(url, timeout=5)
来源：http://fdb.xuanzx.com

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://vey.zhengqikj.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://eby.fengsongda.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://rgy.bbcook.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://yad.tanke756.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://kav.sufxvd.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://rui.nanxinkj.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://noy.jiagoushi.top

[L05] 上传文件（multipart）
来源：http://jig.guowangkeji.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://yxp.fanxiaobao.xyz

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://lsj.nanxinkj.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://fkl.cqqwz.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://vto.chenlongwang.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wml.bjfxy.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mgz.quarkkingdee.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hhw.jinyuanbaomall.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://lqz.vqdsnc.cn

[L06] 解析响应为 JSON
来源：http://apz.hysaishi.cn

Py:   resp.json()
来源：http://doq.tianlin.xyz

PHP:  json_decode($body, true);
来源：http://viq.vehdjk.com

JS:   await resp.json()
来源：http://rct.zdbjq.cn

TS:   await resp.json()
来源：http://ulr.zdqjudy.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://gyv.smart0.xyz

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://aiu.hongshengwenyu.top

Ruby: JSON.parse(resp.body)
来源：http://gok.sxryk.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://lkz.chenlongwang.top

[L07] 处理 HTTP 状态码
来源：http://dmx.yongpay.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://sdn.sjlbkw.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://utm.shuidangran.top

JS:   resp.ok;  resp.status
来源：http://rcp.jinyuanbaomall.cn

TS:   resp.ok;  resp.status
来源：http://jfb.zycfv.cn

Java: resp.statusCode()
来源：http://oda.cucudq.cn

Go:   resp.StatusCode
来源：http://vcu.nanxuanxn.top

Ruby: resp.code.to_i
来源：http://sdo.fehbvm.com

C#:   (int)resp.StatusCode
来源：http://jsh.daria6918.cn

[L08] 并发请求多个地址
来源：http://oiw.daxiang520.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://lbw.yongpay.top

PHP:  curl_multi_init() 系列
来源：http://qlr.smart0.xyz

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://cmq.c1oappe.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://fiv.zhixingplan.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://evq.vehdjk.com

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://poi.sxryk.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://tvc.xylfe.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://thz.gaohongyu789.top

================================================================================
来源：http://nex.ybcxt.top

M. 命令行 / 进程 / 环境
来源：http://pmv.yj20258.top

================================================================================
来源：http://orl.yuxming.cn

[M01] 读取命令行参数
来源：http://xif.gogol.net.cn

Py:   sys.argv[1:]
来源：http://ekf.chenjidiqi.icu

PHP:  $argv;  $argc;
来源：http://wpc.feifeiyinyue.top

JS:   process.argv.slice(2)
来源：http://njr.snrcjt.cn

TS:   process.argv.slice(2)
来源：http://sid.zhixingplan.top

Java: args 数组（main 方法参数）
来源：http://bqi.aibaodan.cn

Go:   os.Args[1:]
来源：http://qlh.fengsongda.top

Ruby: ARGV
来源：http://nfu.aizwys.cn

C#:   args 数组（Main 方法参数）
来源：http://aec.haohaochexian.top

[M02] 读取环境变量
来源：http://ond.cashguo.top

Py:   os.environ.get("HOME")
来源：http://bor.tanke756.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://tra.ydjk.org.cn

JS:   process.env.HOME
来源：http://ywb.redwolf501.top

TS:   process.env.HOME
来源：http://ayl.shangyingyoupin.top

Java: System.getenv("HOME")
来源：http://zit.vqdsnc.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ddl.vehdjk.com

Ruby: ENV["HOME"]
来源：http://jhl.fzhhl.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://xlo.iojbl.cn

[M03] 执行外部命令
来源：http://ont.snrcjt.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mju.jlsjyb.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wmv.gzhubu.top

JS:   child_process.execSync("ls -l").toString()
来源：http://zgh.hysaishi.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://pgb.yanxiufei.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://cph.kuanghao11.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://blj.snrcjt.cn

Ruby: system("ls -l");  `ls -l`
来源：http://caz.zhengqikj.top

C#:   Process.Start("ls", "-l");
来源：http://sdc.kuanghao11.cn

[M04] 获取当前工作目录
来源：http://oqz.zhoulong.xyz

Py:   os.getcwd()
来源：http://vri.zhoulong.xyz

PHP:  getcwd();
来源：http://tmm.ybcxt.top

JS:   process.cwd()
来源：http://wgz.jlsjyb.cn

TS:   process.cwd()
来源：http://dti.chenjidiqi.icu

Java: Path.of("").toAbsolutePath()
来源：http://xta.yj20258888.top

Go:   os.Getwd()
来源：http://fbh.xuetiantiany.cn

Ruby: Dir.pwd
来源：http://qnj.sweek.top

C#:   Directory.GetCurrentDirectory()
来源：http://amf.nanxuanxn.top

[M05] 设置退出码
来源：http://drl.yj20258.top

Py:   sys.exit(1)
来源：http://eyh.sufxvd.cn

PHP:  exit(1);
来源：http://vul.birdmap.top

JS:   process.exit(1)
来源：http://lvi.sjlbkw.cn

TS:   process.exit(1)
来源：http://cbz.52xcode.cn

Java: System.exit(1)
来源：http://nas.gotoacloud.top

Go:   os.Exit(1)
来源：http://hqc.hfpthk.cn

Ruby: exit 1
来源：http://doq.aibaodan.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://vhm.shangyingyoupin.top

[M06] 向标准错误输出
来源：http://rgr.hnxiangtu.top

Py:   print("err", file=sys.stderr)
来源：http://zjy.pycfn.com

PHP:  fwrite(STDERR, "err\n");
来源：http://fxe.0kj1m.cn

JS:   console.error("err")
来源：http://upo.hcnkem.com

TS:   console.error("err")
来源：http://qac.fehbvm.com

Java: System.err.println("err")
来源：http://htv.shuidangran.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://rdd.zdbjq.cn

Ruby: warn "err"
来源：http://drt.yonumen.top

C#:   Console.Error.WriteLine("err")
来源：http://bfm.sysykeji.top

[M07] 判断是否为主入口
来源：http://fja.uphjek.com

Py:   if __name__ == "__main__":
来源：http://msk.dianchejie.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://okv.zycfv.cn

JS:   require.main === module
来源：http://oah.ppjwa.cn

TS:   require.main === module
来源：http://hov.daria6918.cn

Java: public static void main(String[] args)
来源：http://rdh.guowangkeji.top

Go:   func main()
来源：http://yvt.zdqjudy.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://rhq.yj20258.top

C#:   static void Main(string[] args)
来源：http://lqn.52xcode.cn

[M08] 获取系统与运行时信息
来源：http://jwp.tianlin.xyz

Py:   platform.system();  platform.python_version()
来源：http://qea.hfpthk.cn

PHP:  PHP_OS;  phpversion();
来源：http://bdw.pengpengdd.cyou

JS:   process.platform;  process.version
来源：http://gji.fzhhl.top

TS:   process.platform;  process.version
来源：http://kik.hysaishi.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wtx.zdqjudy.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://cvw.zhixingplan.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://nqk.ppjwa.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://ifa.bbcook.cn

================================================================================
来源：http://vyj.ehwqpu.com

N. 数据结构与算法
来源：http://mjm.hongshengwenyu.top

================================================================================
来源：http://cov.shanyushiyangkeji.top

[N01] 二分查找（有序数组）
来源：http://swg.wangdashe.top

Py:   bisect.bisect_left(arr, x)
来源：http://abb.fanxiaobao.xyz

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://flk.ctjpmb.com

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ntp.sufxvd.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ums.hnqzz.top

Java: Arrays.binarySearch(arr, x)
来源：http://was.yonumen.top

Go:   sort.SearchInts(arr, x)
来源：http://vez.hcnkem.com

Ruby: arr.bsearch { |e| e >= x }
来源：http://jhb.nwbrower.top

C#:   Array.BinarySearch(arr, x)
来源：http://fyf.ctjpmb.com

[N02] 排序（工程实践用内置实现）
来源：http://epz.gzhubu.top

Py:   sorted(arr);  arr.sort()
来源：http://ppy.zhoulong.xyz

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://kak.shangyingyoupin.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://ymd.kuanghao11.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://fjk.hesvh.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://vyo.havefunace.top

Go:   slices.Sort(arr)
来源：http://cmn.ydjk.org.cn

Ruby: arr.sort
来源：http://dhr.yangfankeji.com

C#:   Array.Sort(arr);  list.Sort()
来源：http://pvt.hywenlv.cn

[N03] 快速排序（分治示例）
来源：http://kui.vehdjk.com

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hob.yuanzhike.top

PHP:  // 递归实现，或用 usort
来源：http://ozg.dashuyun.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://dcg.jianghu66.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://tiy.sufxvd.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://xxh.yvedp.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://sss.jinqigfzy.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://tid.yangfankeji.com

C#:   // 手写递归，或 Array.Sort
来源：http://fgs.jianghu66.top

[N04] 斐波那契数列
来源：http://wzs.bjfxy.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://cqa.chenjidiqi.icu

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://xnz.jianghu66.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://uok.shanyushiyangkeji.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://nvw.yj20258.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://yaj.jinghuilouyu.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://qmr.zdbjq.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://taz.gaohongyu789.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hbu.zhoulong.xyz

[N05] 最大公约数
来源：http://ahl.yuanzhike.top

Py:   math.gcd(a, b)
来源：http://vxc.yvedp.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wdp.ydjk.org.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://qxi.sxryk.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://xgy.shanyushiyangkeji.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://xbf.xingfuxueyuan.xyz

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://cxj.yfazqb.com

Ruby: a.gcd(b)
来源：http://gph.0kj1m.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://gpo.yongpay.top

[N06] 判断回文字符串
来源：http://lrk.haohaochexian.top

Py:   s == s[::-1]
来源：http://dcv.wangdashe.top

PHP:  $s === strrev($s);
来源：http://ixs.zhongyouzk.top

JS:   s === [...s].reverse().join("")
来源：http://aka.chenjidiqi.icu

TS:   s === [...s].reverse().join("")
来源：http://xxc.yj202588.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://yst.havefunace.top

Go:   // 双指针从两端比较
来源：http://pek.c1oappe.top

Ruby: s == s.reverse
来源：http://iqv.xziqi.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://klc.jinqigfzy.top

[N07] 两数之和（返回下标）
来源：http://yvh.tianlin.xyz

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://lqa.hysaishi.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://lts.sufxvd.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://gog.svipenyu.cn

TS:   // 手写 Map<string, number>
来源：http://ymz.wangdashe.top

Java: // 手写 HashMap
来源：http://ira.mhx1999.top

Go:   // 手写 map[int]int
来源：http://nwl.meibo888.top

Ruby: // 手写 Hash
来源：http://hdd.zhaomingkeji.xyz

C#:   // 手写 Dictionary<int, int>
来源：http://sco.aizwys.cn

[N08] 生成全排列
来源：http://pjv.xinyue.icu

Py:   itertools.permutations(arr)
来源：http://vyi.meibo888.top

PHP:  // 手写递归交换
来源：http://qao.shzxlz.cn

JS:   // 手写回溯递归
来源：http://dbx.epnwcf.com

TS:   // 手写回溯递归
来源：http://czg.yj20258888.top

Java: // 手写回溯递归
来源：http://gpq.fanxiaobao.xyz

Go:   // 手写回溯递归
来源：http://pes.cdnleiting.top

Ruby: arr.permutation.to_a
来源：http://ocs.nanxinkj.top

C#:   // 手写回溯递归
来源：http://rhe.cqqwz.cn

[N09] 栈与队列
来源：http://ikw.hfpthk.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://xmw.316326.xyz

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://dfz.xingfuxueyuan.xyz

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mwu.pycfn.com

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hwb.zhengqikj.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://vmu.wangdashe.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://sxz.jlsjyb.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wfj.wangdashe.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://oyu.yueranfly.top

[N10] 链表节点定义
来源：http://lps.birdmap.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hgz.haohaochexian.top

PHP:  class Node { public $v; public $next = null; }
来源：http://gax.hysaishi.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://dzf.zhoulong.xyz

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ysc.ybcxt.top

Java: class Node { int v; Node next; }
来源：http://rcz.zdbjq.cn

Go:   type Node struct { V int; Next *Node }
来源：http://giz.xuanzx.com

Ruby: Node = Struct.new(:v, :next)
来源：http://gsv.sufxvd.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://zoi.ivvv.top

[N11] 二叉树中序遍历
来源：http://dha.yongpay.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://tcc.aizwys.cn

PHP:  // 手写递归函数
来源：http://pft.zhaomingkeji.xyz

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://len.yj20258888.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://zpu.cqqwz.cn

Java: // 手写递归
来源：http://csf.xziqi.cn

Go:   // 手写递归
来源：http://jol.meibo888.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://lug.redwolf501.top

C#:   // 手写递归
来源：http://hfr.xuetiantiany.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://lmm.gogol.net.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://gvb.cqqwz.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://qlm.aibaodan.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://vyp.fzhhl.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://opy.xylfe.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://okw.iojbl.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://pku.jyoumei.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://agr.sysykeji.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://kjx.hammf.cn

================================================================================
来源：http://gcf.jinghuilouyu.cn

O. 并发与异步
来源：http://lxq.chenlongwang.top

================================================================================
来源：http://uta.xinyue.icu

[O01] 启动一个线程
来源：http://evh.shzxlz.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://nol.shangyingyoupin.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://rhe.52xcode.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ufo.gzhubu.top

TS:   // 同 JS
来源：http://jeq.tarul.cn

Java: new Thread(() -> f()).start()
来源：http://iox.xuetiantiany.cn

Go:   go f()
来源：http://zay.chenjidiqi.icu

Ruby: Thread.new { f }
来源：http://ket.guannengcc.top

C#:   Task.Run(() => F());
来源：http://rqd.ppjwa.cn

[O02] 使用线程池
来源：http://fxq.shuidangran.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://kjp.hcnkem.com

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hcg.uphjek.com

JS:   // worker_threads 线程池
来源：http://jpq.ehwqpu.com

TS:   // worker_threads 线程池
来源：http://vlq.jqgfzy.top

Java: Executors.newFixedThreadPool(4)
来源：http://uki.yfazqb.com

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://lyj.c1oappe.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://kdf.shanyushiyangtech.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ijm.andypj.xyz

[O03] 加锁保护共享数据
来源：http://pps.gzhubu.top

Py:   with lock: shared += 1
来源：http://tkx.ydzc1.top

PHP:  // 用 flock() 做文件锁
来源：http://rvv.zhaomingkeji.xyz

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://llq.jinqigfzy.top

TS:   // 同 JS
来源：http://gpy.yueranfly.top

Java: synchronized (this) { shared++; }
来源：http://rmf.zhoulong.xyz

Go:   mu.Lock();  defer mu.Unlock()
来源：http://bzn.jinqigufen.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://ezm.ctjpmb.com

C#:   lock (gate) { shared++; }
来源：http://kvj.snrcjt.cn

[O04] 定义异步函数并等待
来源：http://hlc.daria6918.cn

Py:   async def f():⏎    await g()
来源：http://rhn.hysaishi.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://qud.yonumen.top

JS:   async function f() { await g(); }
来源：http://fmr.wangshuangyany.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://tmm.daria6918.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://sdz.wangshuangyany.cn


<!-- 参考信息 -->