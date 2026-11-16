代发 wailian999

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://zjz.guowangkeji.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://uwi.cheryme.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://fhg.shuidangran.top

[K05] 深拷贝对象
来源：http://dte.hammf.cn

Py:   copy.deepcopy(obj)
来源：http://ryk.fktsv.cn

PHP:  unserialize(serialize($obj));
来源：http://wht.haohaochexian.top

JS:   structuredClone(obj)
来源：http://xdl.jyoumei.cn

TS:   structuredClone(obj)
来源：http://gwa.vehdjk.com

Java: // 手写拷贝构造，或序列化往返
来源：http://vft.yonumen.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://jyw.zhiwuduotai.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ejr.fktsv.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://bkm.guannengcc.top

[K06] 解析 URL 查询串
来源：http://fyk.cdnleiting.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://kkz.havefunace.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://uxi.hnxiangtu.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://bnz.hongshengwenyu.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://bob.nanxinkj.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ubb.wangdashe.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://ama.redwolf501.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://zuh.jyoumei.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://csx.fengsongda.top

[K07] 进制转换
来源：http://gyf.fktsv.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://shc.sufxvd.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://eyn.9152youxi.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://kio.yangfankeji.com

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://nkv.zhaomingkeji.xyz

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wzw.zhongyouzk.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://dvv.tian-w.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://fzn.smart0.xyz

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://enw.ybcxt.top

[K08] 二进制序列化（非 JSON）
来源：http://fag.shuidangran.top

Py:   pickle.dumps(obj)
来源：http://vtl.pengpengdd.cyou

PHP:  serialize($obj);  unserialize($s);
来源：http://nbl.fktsv.cn

JS:   v8.serialize(obj)        // Node
来源：http://oib.fktsv.cn

TS:   v8.serialize(obj)        // Node
来源：http://yuh.daria6918.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://cmu.jinyuanbaomall.cn

Go:   encoding/gob
来源：http://yzh.tianlin.xyz

Ruby: Marshal.dump(obj)
来源：http://kdr.shanyushiyangtech.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://pnn.xinyue.icu

================================================================================
来源：http://icx.52xcode.cn

L. 网络请求
来源：http://ugx.xziqi.cn

================================================================================
来源：http://lhp.zhixingplan.top

[L01] 发送 GET 请求
来源：http://dsl.yuxming.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://jvl.hongshengwenyu.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ynw.jlsjyb.cn

JS:   await fetch(url)
来源：http://oor.wangdashe.top

TS:   await fetch(url)
来源：http://txq.hysaishi.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mbe.bbcook.cn

Go:   resp, err := http.Get(url)
来源：http://fse.sxryk.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://rkj.jinghuilouyu.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ssb.yfazqb.com

[L02] 发送 POST JSON
来源：http://kqn.feifeiyinyue.top

Py:   requests.post(url, json={"a": 1})
来源：http://lqy.cashguo.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://epd.shanyushiyangkeji.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://egs.hcnkem.com

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://gsj.cashguo.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://tno.ydzc1.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://uta.zhoulong.xyz

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://roq.ywan-chungtsiang.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://rgy.yangfankeji.com

[L03] 设置自定义请求头
来源：http://yzd.aizwys.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://gpp.yangfankeji.com

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://gve.hcnkem.com

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://dvt.jianghu66.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://emq.tian-w.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://rcm.fanxiaobao.xyz

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://cmm.tarul.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://oev.jlsjyb.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://jac.0kj1m.cn

[L04] 设置超时
来源：http://bri.cashguo.top

Py:   requests.get(url, timeout=5)
来源：http://xfs.dashuyun.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://xhs.316326.xyz

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://pba.kuanghao11.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://uiq.jlsjyb.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://fmf.zdbjq.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ppu.hfpthk.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://dfr.hongshengwenyu.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://jso.shzxlz.cn

[L05] 上传文件（multipart）
来源：http://wna.ydjk.org.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mck.cheryme.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://lpf.sjlbkw.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wdp.xuanzx.com

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://nxp.hesvh.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wqy.gaohongyu789.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://tvs.ydzc1.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://rsv.jinyuanbaomall.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://aiq.vqdsnc.cn

[L06] 解析响应为 JSON
来源：http://vuv.gotoacloud.top

Py:   resp.json()
来源：http://exa.zhixingplan.top

PHP:  json_decode($body, true);
来源：http://olc.shanyushiyangtech.top

JS:   await resp.json()
来源：http://ldy.yueranfly.top

TS:   await resp.json()
来源：http://lnm.hcnkem.com

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://zpm.9152youxi.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://fak.hnqzz.top

Ruby: JSON.parse(resp.body)
来源：http://bak.jqgufenzy.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://rrk.zhixingplan.top

[L07] 处理 HTTP 状态码
来源：http://hry.hysaishi.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://knu.zhoulong.xyz

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ylh.zhengqikj.top

JS:   resp.ok;  resp.status
来源：http://lih.vehdjk.com

TS:   resp.ok;  resp.status
来源：http://bqs.andypj.xyz

Java: resp.statusCode()
来源：http://cov.quarkkingdee.top

Go:   resp.StatusCode
来源：http://fiy.haohaochexian.top

Ruby: resp.code.to_i
来源：http://sgt.gzhubu.top

C#:   (int)resp.StatusCode
来源：http://nqe.chenlongwang.top

[L08] 并发请求多个地址
来源：http://xcn.ctjpmb.com

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://pda.gotoacloud.top

PHP:  curl_multi_init() 系列
来源：http://bko.nanxuanxn.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://kwc.52xcode.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://rvr.zhiwuduotai.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://obz.ehwqpu.com

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://cep.guannengcc.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://pjo.zhiwuduotai.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://psv.svipenyu.cn

================================================================================
来源：http://bzy.zhixingplan.top

M. 命令行 / 进程 / 环境
来源：http://bbe.nanxuanxn.top

================================================================================
来源：http://zjd.zhoulong.xyz

[M01] 读取命令行参数
来源：http://gae.chenzaomai.com

Py:   sys.argv[1:]
来源：http://qra.aibaodan.cn

PHP:  $argv;  $argc;
来源：http://kfc.52xcode.cn

JS:   process.argv.slice(2)
来源：http://aqu.jianghu66.top

TS:   process.argv.slice(2)
来源：http://gaw.gogol.net.cn

Java: args 数组（main 方法参数）
来源：http://wns.wangdashe.top

Go:   os.Args[1:]
来源：http://jvy.zycfv.cn

Ruby: ARGV
来源：http://whf.gotoacloud.top

C#:   args 数组（Main 方法参数）
来源：http://hsh.uphjek.com

[M02] 读取环境变量
来源：http://idp.sufxvd.cn

Py:   os.environ.get("HOME")
来源：http://ymm.hcnkem.com

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://aky.ehwqpu.com

JS:   process.env.HOME
来源：http://pau.yonumen.top

TS:   process.env.HOME
来源：http://dtn.cdnleiting.top

Java: System.getenv("HOME")
来源：http://umg.zhaomingkeji.xyz

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://pwl.shuidangran.top

Ruby: ENV["HOME"]
来源：http://jrx.ybcxt.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://lsf.shanyushiyangkeji.top

[M03] 执行外部命令
来源：http://xnl.aibaodan.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://etb.sjlbkw.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://eme.jinqigufen.top

JS:   child_process.execSync("ls -l").toString()
来源：http://tcq.pycfn.com

TS:   child_process.execSync("ls -l").toString()
来源：http://ert.52xcode.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://doj.svipenyu.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://ifu.hysaishi.cn

Ruby: system("ls -l");  `ls -l`
来源：http://ktv.smart0.xyz

C#:   Process.Start("ls", "-l");
来源：http://jdi.sysykeji.top

[M04] 获取当前工作目录
来源：http://jgo.redwolf501.top

Py:   os.getcwd()
来源：http://yec.vqdsnc.cn

PHP:  getcwd();
来源：http://yvj.xuetiantiany.cn

JS:   process.cwd()
来源：http://gmz.yanxiufei.cn

TS:   process.cwd()
来源：http://jnt.jlsjyb.cn

Java: Path.of("").toAbsolutePath()
来源：http://wts.fzhhl.top

Go:   os.Getwd()
来源：http://zbh.yonumen.top

Ruby: Dir.pwd
来源：http://bqp.yj20258888.top

C#:   Directory.GetCurrentDirectory()
来源：http://qgf.yonumen.top

[M05] 设置退出码
来源：http://ggm.daria6918.cn

Py:   sys.exit(1)
来源：http://lko.shuidangran.top

PHP:  exit(1);
来源：http://jai.shanyushiyangkeji.top

JS:   process.exit(1)
来源：http://vzk.dashuyun.cn

TS:   process.exit(1)
来源：http://fbz.shanyushiyangtech.top

Java: System.exit(1)
来源：http://aqe.xingfuxueyuan.xyz

Go:   os.Exit(1)
来源：http://lnp.gzhubu.top

Ruby: exit 1
来源：http://dtz.xuanzx.com

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://dus.c1oappe.top

[M06] 向标准错误输出
来源：http://usf.shanyushiyangkeji.top

Py:   print("err", file=sys.stderr)
来源：http://ywg.ybcxt.top

PHP:  fwrite(STDERR, "err\n");
来源：http://ikt.sweek.top

JS:   console.error("err")
来源：http://zca.xingfuxueyuan.xyz

TS:   console.error("err")
来源：http://kcm.sufxvd.cn

Java: System.err.println("err")
来源：http://tqc.0kj1m.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://fnt.tianlin.xyz

Ruby: warn "err"
来源：http://rcv.xziqi.cn

C#:   Console.Error.WriteLine("err")
来源：http://dew.jinqigufen.top

[M07] 判断是否为主入口
来源：http://ipw.yj202588.top

Py:   if __name__ == "__main__":
来源：http://gzi.ehwqpu.com

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://qpl.shuidangran.top

JS:   require.main === module
来源：http://ipe.52xcode.cn

TS:   require.main === module
来源：http://xmq.gotoacloud.top

Java: public static void main(String[] args)
来源：http://kte.vqdsnc.cn

Go:   func main()
来源：http://mnh.chenlongwang.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ivm.tian-w.cn

C#:   static void Main(string[] args)
来源：http://gri.chenjidiqi.icu

[M08] 获取系统与运行时信息
来源：http://ofk.xziqi.cn

Py:   platform.system();  platform.python_version()
来源：http://vlz.gaohongyu789.top

PHP:  PHP_OS;  phpversion();
来源：http://cyc.xingfuxueyuan.xyz

JS:   process.platform;  process.version
来源：http://hgm.52xcode.cn

TS:   process.platform;  process.version
来源：http://azq.52xcode.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ihf.hongshengwenyu.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://nlb.daxiang520.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://zdr.yvedp.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://gnu.zhaomingkeji.xyz

================================================================================
来源：http://ujn.dashuyun.cn

N. 数据结构与算法
来源：http://hrd.fzhhl.top

================================================================================
来源：http://siy.hysaishi.cn

[N01] 二分查找（有序数组）
来源：http://rrz.cashguo.top

Py:   bisect.bisect_left(arr, x)
来源：http://jzn.hysaishi.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://iuy.tarul.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://zok.xuetiantiany.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://agg.yonumen.top

Java: Arrays.binarySearch(arr, x)
来源：http://ggg.aibaodan.cn

Go:   sort.SearchInts(arr, x)
来源：http://ebq.guowangkeji.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://mbl.zhixingplan.top

C#:   Array.BinarySearch(arr, x)
来源：http://puh.daria6918.cn

[N02] 排序（工程实践用内置实现）
来源：http://oye.yfazqb.com

Py:   sorted(arr);  arr.sort()
来源：http://tzw.aizwys.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://chq.smart0.xyz

JS:   [...arr].sort((a, b) => a - b)
来源：http://uui.yangfankeji.com

TS:   [...arr].sort((a, b) => a - b)
来源：http://vtr.iojbl.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mmw.meibo888.top

Go:   slices.Sort(arr)
来源：http://hpf.gaohongyu789.top

Ruby: arr.sort
来源：http://ggl.zdbjq.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://owl.guannengcc.top

[N03] 快速排序（分治示例）
来源：http://ntf.gzhubu.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://gzt.andypj.xyz

PHP:  // 递归实现，或用 usort
来源：http://sny.yongpay.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://zlv.yj20258888.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wfo.epnwcf.com

Java: // 手写递归，或直接用 Arrays.sort
来源：http://nbc.mhx1999.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://kec.sxryk.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://oqs.ybcxt.top

C#:   // 手写递归，或 Array.Sort
来源：http://axu.zhiwuduotai.top

[N04] 斐波那契数列
来源：http://ycb.xingfuxueyuan.xyz

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://nmw.yangfankeji.com

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://vsr.yj20258.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://jql.chenzaomai.com

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wec.vqdsnc.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ysw.yueranfly.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://kpq.hongshengwenyu.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://oxw.yuanzhike.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://doj.sufxvd.cn

[N05] 最大公约数
来源：http://zkh.hysaishi.cn

Py:   math.gcd(a, b)
来源：http://wbn.hammf.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ytm.sufxvd.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://xas.chenzaomai.com

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://yco.ctjpmb.com

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://qpn.xingfuxueyuan.xyz

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://fly.yangfankeji.com

Ruby: a.gcd(b)
来源：http://ceb.fehbvm.com

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://nvn.chenzaomai.com

[N06] 判断回文字符串
来源：http://guy.nanxuanxn.top

Py:   s == s[::-1]
来源：http://htd.zhaomingkeji.xyz

PHP:  $s === strrev($s);
来源：http://haq.iojbl.cn

JS:   s === [...s].reverse().join("")
来源：http://rno.jlsjyb.cn

TS:   s === [...s].reverse().join("")
来源：http://acp.zhongyouzk.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ndg.sweek.top

Go:   // 双指针从两端比较
来源：http://ybn.ivvv.top

Ruby: s == s.reverse
来源：http://mzp.tianlin.xyz

C#:   s == new string(s.Reverse().ToArray())
来源：http://umh.nwbrower.top

[N07] 两数之和（返回下标）
来源：http://ole.xingfuxueyuan.xyz

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://fdr.aizwys.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://yrl.sjlbkw.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://vor.52xcode.cn

TS:   // 手写 Map<string, number>
来源：http://yuj.yongpay.top

Java: // 手写 HashMap
来源：http://aeq.shuidangran.top

Go:   // 手写 map[int]int
来源：http://bpr.gzhubu.top

Ruby: // 手写 Hash
来源：http://xvn.yangfankeji.com

C#:   // 手写 Dictionary<int, int>
来源：http://sei.hfpthk.cn

[N08] 生成全排列
来源：http://rle.ydjk.org.cn

Py:   itertools.permutations(arr)
来源：http://soa.jinqigfzy.top

PHP:  // 手写递归交换
来源：http://uie.yangfankeji.com

JS:   // 手写回溯递归
来源：http://cmc.uphjek.com

TS:   // 手写回溯递归
来源：http://ylo.iojbl.cn

Java: // 手写回溯递归
来源：http://pyf.sysykeji.top

Go:   // 手写回溯递归
来源：http://mmh.hcnkem.com

Ruby: arr.permutation.to_a
来源：http://mos.yj20258888.top

C#:   // 手写回溯递归
来源：http://mmz.zdbjq.cn

[N09] 栈与队列
来源：http://hes.zdbjq.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://zvf.andypj.xyz

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://gpo.xingfuxueyuan.xyz

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://dte.zdqjudy.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://kuu.fktsv.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://uae.zhiwuduotai.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://gmw.cheryme.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://lrh.zhaomingkeji.xyz

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://oer.316326.xyz

[N10] 链表节点定义
来源：http://slp.epnwcf.com

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://vkk.chenjidiqi.icu

PHP:  class Node { public $v; public $next = null; }
来源：http://bem.nwbrower.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://fbb.yonumen.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://rht.cheryme.top

Java: class Node { int v; Node next; }
来源：http://mde.sxryk.cn

Go:   type Node struct { V int; Next *Node }
来源：http://dkn.9152youxi.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://yhy.fengsongda.top

C#:   class Node { public int V; public Node? Next; }
来源：http://psz.nanxinkj.top

[N11] 二叉树中序遍历
来源：http://dzs.xuetiantiany.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wqb.zhongyouzk.top

PHP:  // 手写递归函数
来源：http://isa.yfazqb.com

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://kmd.chenzaomai.com

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://bdy.daria6918.cn

Java: // 手写递归
来源：http://nlx.xinyue.icu

Go:   // 手写递归
来源：http://rxs.vqdsnc.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://eas.jinqigfzy.top

C#:   // 手写递归
来源：http://gqf.tianlin.xyz

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ymd.feifeiyinyue.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://giz.gogol.net.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://uww.hysaishi.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wbp.yangfankeji.com

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wte.shanyushiyangtech.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hkl.zhongyouzk.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://lfw.jlsjyb.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://sou.xuanzx.com

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://aon.hammf.cn


<!-- 参考信息 -->