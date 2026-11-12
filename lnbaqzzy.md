代发 wailian999

Ruby: JSON.pretty_generate(obj)
来源：http://ifv.chenlongwang.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://irb.smart0.xyz

[K04] 读取 JSON 文件
来源：http://cza.xziqi.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://htw.jinghuilouyu.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ucz.dianchejie.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://qbh.guowangkeji.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://znl.nwbrower.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://yai.yuxming.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://inq.hammf.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://knw.jqgfzy.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://thc.chenlongwang.top

[K05] 深拷贝对象
来源：http://ycr.9152youxi.cn

Py:   copy.deepcopy(obj)
来源：http://iev.aizwys.cn

PHP:  unserialize(serialize($obj));
来源：http://icd.fehbvm.com

JS:   structuredClone(obj)
来源：http://zgg.hfpthk.cn

TS:   structuredClone(obj)
来源：http://myq.c1oappe.top

Java: // 手写拷贝构造，或序列化往返
来源：http://zwc.haohaochexian.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://pry.yvedp.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://cxe.yuxming.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://lod.hnqzz.top

[K06] 解析 URL 查询串
来源：http://ofk.nwbrower.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ned.sjlbkw.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://juw.bjfxy.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://esa.shzxlz.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://gbk.gaohongyu789.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://rnv.ydjk.org.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://wny.birdmap.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://fve.sxryk.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://xaf.fehbvm.com

[K07] 进制转换
来源：http://hcg.cdnleiting.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://uux.daxiang520.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ddd.shanyushiyangtech.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://kup.snrcjt.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://lca.fktsv.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://nyc.fktsv.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://gqe.zhaomingkeji.xyz

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://qol.ydjk.org.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://zfg.wangshuangyany.cn

[K08] 二进制序列化（非 JSON）
来源：http://ric.yongpay.top

Py:   pickle.dumps(obj)
来源：http://com.tanke756.top

PHP:  serialize($obj);  unserialize($s);
来源：http://dfb.jinqigufen.top

JS:   v8.serialize(obj)        // Node
来源：http://wqu.xuetiantiany.cn

TS:   v8.serialize(obj)        // Node
来源：http://kcv.jyoumei.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ytc.shanyushiyangtech.top

Go:   encoding/gob
来源：http://vtt.quarkkingdee.top

Ruby: Marshal.dump(obj)
来源：http://wku.fehbvm.com

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://nhw.hfpthk.cn

================================================================================
来源：http://hti.316326.xyz

L. 网络请求
来源：http://qow.quarkkingdee.top

================================================================================
来源：http://iuc.hongshengwenyu.top

[L01] 发送 GET 请求
来源：http://wfj.52xcode.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://vvh.zhaomingkeji.xyz

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://qwm.cqqwz.cn

JS:   await fetch(url)
来源：http://wio.mhx1999.top

TS:   await fetch(url)
来源：http://ahr.aibaodan.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://tuy.ehwqpu.com

Go:   resp, err := http.Get(url)
来源：http://kge.shanyushiyangtech.top

Ruby: Net::HTTP.get(URI(url))
来源：http://yfi.bjfxy.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://oni.aizwys.cn

[L02] 发送 POST JSON
来源：http://pbo.jqgfzy.top

Py:   requests.post(url, json={"a": 1})
来源：http://uys.yj20258.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://vwj.jiagoushi.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wws.jinghuilouyu.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ovw.shzxlz.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://yrb.bbcook.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://eqy.mhx1999.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://zkt.fengsongda.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://qqk.gzhubu.top

[L03] 设置自定义请求头
来源：http://ude.vqdsnc.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://bik.shangyingyoupin.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ouk.yuanzhike.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://qfn.zdqjudy.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ihq.ppjwa.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ziu.shangyingyoupin.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://pyh.yj20258.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://zrc.wangdashe.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ncm.zdbjq.cn

[L04] 设置超时
来源：http://tdo.feifeiyinyue.top

Py:   requests.get(url, timeout=5)
来源：http://unw.aizwys.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://gki.cdnleiting.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://zrm.aibaodan.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hut.yangfankeji.com

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wcw.ybcxt.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://tkc.feifeiyinyue.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://rcd.xylfe.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://yef.316326.xyz

[L05] 上传文件（multipart）
来源：http://usa.hongshengwenyu.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://brx.gaohongyu789.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wne.ydjk.org.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://qzp.hysaishi.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ogg.zhiwuduotai.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://fnq.gogol.net.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://epy.andypj.xyz

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://bfv.sysykeji.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://rqw.bbcook.cn

[L06] 解析响应为 JSON
来源：http://mlx.zhixingplan.top

Py:   resp.json()
来源：http://lgi.chenzaomai.com

PHP:  json_decode($body, true);
来源：http://wov.vqdsnc.cn

JS:   await resp.json()
来源：http://ges.hnqzz.top

TS:   await resp.json()
来源：http://cgr.fengsongda.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://rhg.shanyushiyangkeji.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://jmv.zhaomingkeji.xyz

Ruby: JSON.parse(resp.body)
来源：http://koq.tianlin.xyz

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://xsq.smart0.xyz

[L07] 处理 HTTP 状态码
来源：http://uwe.zhixingplan.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://jhw.yuxming.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://bno.ctjpmb.com

JS:   resp.ok;  resp.status
来源：http://awt.52xcode.cn

TS:   resp.ok;  resp.status
来源：http://htx.hesvh.cn

Java: resp.statusCode()
来源：http://cni.chenzaomai.com

Go:   resp.StatusCode
来源：http://ykx.yueranfly.top

Ruby: resp.code.to_i
来源：http://gip.nanxinkj.top

C#:   (int)resp.StatusCode
来源：http://cho.hysaishi.cn

[L08] 并发请求多个地址
来源：http://zym.cheryme.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hpu.xylfe.cn

PHP:  curl_multi_init() 系列
来源：http://cgh.tian-w.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wao.xuetiantiany.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ive.kuanghao11.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://vqu.gogol.net.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://dsg.shanyushiyangtech.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://vbm.bbcook.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://elt.tian-w.cn

================================================================================
来源：http://yza.daxiang520.top

M. 命令行 / 进程 / 环境
来源：http://ver.hnqzz.top

================================================================================
来源：http://lys.9152youxi.cn

[M01] 读取命令行参数
来源：http://nav.epnwcf.com

Py:   sys.argv[1:]
来源：http://npe.jinghuilouyu.cn

PHP:  $argv;  $argc;
来源：http://ukp.tarul.cn

JS:   process.argv.slice(2)
来源：http://kgu.xziqi.cn

TS:   process.argv.slice(2)
来源：http://gma.tian-w.cn

Java: args 数组（main 方法参数）
来源：http://kcu.ehwqpu.com

Go:   os.Args[1:]
来源：http://zkg.hywenlv.cn

Ruby: ARGV
来源：http://wbx.daxiang520.top

C#:   args 数组（Main 方法参数）
来源：http://khj.kuanghao11.cn

[M02] 读取环境变量
来源：http://tib.zdbjq.cn

Py:   os.environ.get("HOME")
来源：http://zke.wangdashe.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://xhf.haohaochexian.top

JS:   process.env.HOME
来源：http://oie.epnwcf.com

TS:   process.env.HOME
来源：http://uyg.xziqi.cn

Java: System.getenv("HOME")
来源：http://mbv.bbcook.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://lte.yfazqb.com

Ruby: ENV["HOME"]
来源：http://tii.daria6918.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://twf.hnxiangtu.top

[M03] 执行外部命令
来源：http://lnl.ehwqpu.com

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://zgv.hnqzz.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hof.nanxinkj.top

JS:   child_process.execSync("ls -l").toString()
来源：http://yss.sjlbkw.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://vwe.daxiang520.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://vlp.xylfe.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://wtz.fehbvm.com

Ruby: system("ls -l");  `ls -l`
来源：http://adv.gzhubu.top

C#:   Process.Start("ls", "-l");
来源：http://ucq.chenlongwang.top

[M04] 获取当前工作目录
来源：http://gul.zhongyouzk.top

Py:   os.getcwd()
来源：http://spo.cashguo.top

PHP:  getcwd();
来源：http://dhr.bjfxy.top

JS:   process.cwd()
来源：http://zte.yvedp.cn

TS:   process.cwd()
来源：http://hrt.chenjidiqi.icu

Java: Path.of("").toAbsolutePath()
来源：http://ntp.andypj.xyz

Go:   os.Getwd()
来源：http://srs.jinqigufen.top

Ruby: Dir.pwd
来源：http://vsk.snrcjt.cn

C#:   Directory.GetCurrentDirectory()
来源：http://iwr.tianlin.xyz

[M05] 设置退出码
来源：http://rto.fzhhl.top

Py:   sys.exit(1)
来源：http://xti.cashguo.top

PHP:  exit(1);
来源：http://foc.cucudq.cn

JS:   process.exit(1)
来源：http://hcu.cashguo.top

TS:   process.exit(1)
来源：http://ean.zdqjudy.top

Java: System.exit(1)
来源：http://nie.shanyushiyangtech.top

Go:   os.Exit(1)
来源：http://ezw.andypj.xyz

Ruby: exit 1
来源：http://beo.shuidangran.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://cxe.yvedp.cn

[M06] 向标准错误输出
来源：http://blg.yuxming.cn

Py:   print("err", file=sys.stderr)
来源：http://nss.meibo888.top

PHP:  fwrite(STDERR, "err\n");
来源：http://rca.9152youxi.cn

JS:   console.error("err")
来源：http://igv.havefunace.top

TS:   console.error("err")
来源：http://sny.cdnleiting.top

Java: System.err.println("err")
来源：http://dww.chenlongwang.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://rll.shuidangran.top

Ruby: warn "err"
来源：http://boj.snrcjt.cn

C#:   Console.Error.WriteLine("err")
来源：http://jav.vehdjk.com

[M07] 判断是否为主入口
来源：http://kfo.mhx1999.top

Py:   if __name__ == "__main__":
来源：http://rjk.zdqjudy.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://cue.yongpay.top

JS:   require.main === module
来源：http://cte.jinqigfzy.top

TS:   require.main === module
来源：http://ouv.nwbrower.top

Java: public static void main(String[] args)
来源：http://snz.iojbl.cn

Go:   func main()
来源：http://rot.vehdjk.com

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ixa.sxryk.cn

C#:   static void Main(string[] args)
来源：http://exe.cdnleiting.top

[M08] 获取系统与运行时信息
来源：http://odg.guannengcc.top

Py:   platform.system();  platform.python_version()
来源：http://gdx.9152youxi.cn

PHP:  PHP_OS;  phpversion();
来源：http://dbd.hnxiangtu.top

JS:   process.platform;  process.version
来源：http://ilh.hammf.cn

TS:   process.platform;  process.version
来源：http://ona.xziqi.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://cyv.yangfankeji.com

Go:   runtime.GOOS;  runtime.Version()
来源：http://mvn.yj20258888.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ygl.vehdjk.com

C#:   Environment.OSVersion;  Environment.Version
来源：http://kmm.fengsongda.top

================================================================================
来源：http://ueh.wangdashe.top

N. 数据结构与算法
来源：http://nxs.c1oappe.top

================================================================================
来源：http://avd.tian-w.cn

[N01] 二分查找（有序数组）
来源：http://ikj.jqgufenzy.top

Py:   bisect.bisect_left(arr, x)
来源：http://ivf.havefunace.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://vnh.zhaomingkeji.xyz

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mtx.meibo888.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://uqh.hesvh.cn

Java: Arrays.binarySearch(arr, x)
来源：http://aup.iojbl.cn

Go:   sort.SearchInts(arr, x)
来源：http://yvk.gzhubu.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://cul.wangdashe.top

C#:   Array.BinarySearch(arr, x)
来源：http://ltf.gzhubu.top

[N02] 排序（工程实践用内置实现）
来源：http://vma.ehwqpu.com

Py:   sorted(arr);  arr.sort()
来源：http://nhs.chenzaomai.com

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://elb.iojbl.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://ccb.jyoumei.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://bhw.yj20258.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://cdl.zhengqikj.top

Go:   slices.Sort(arr)
来源：http://dau.epnwcf.com

Ruby: arr.sort
来源：http://dmc.sxryk.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://dtd.ydzc1.top

[N03] 快速排序（分治示例）
来源：http://zpn.xziqi.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://dzj.birdmap.top

PHP:  // 递归实现，或用 usort
来源：http://cin.jqgufenzy.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://scu.zycfv.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://bcd.bjfxy.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://gnq.wangshuangyany.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://yst.xuanzx.com

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://pxc.haohaochexian.top

C#:   // 手写递归，或 Array.Sort
来源：http://ost.yongpay.top

[N04] 斐波那契数列
来源：http://hps.shanyushiyangtech.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://dyj.jlsjyb.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wdt.yj20258888.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://qqu.yueranfly.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://yqi.zhongyouzk.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ntv.zdbjq.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://eyl.dianchejie.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://bgb.cdnleiting.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ixo.birdmap.top

[N05] 最大公约数
来源：http://gxb.zhixingplan.top

Py:   math.gcd(a, b)
来源：http://kpi.wangshuangyany.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://nub.zhixingplan.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://cdm.dianchejie.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://aaq.hesvh.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ofj.yongpay.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://gbe.jinqigufen.top

Ruby: a.gcd(b)
来源：http://trj.shangyingyoupin.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://kol.haohaochexian.top

[N06] 判断回文字符串
来源：http://muy.jinqigfzy.top

Py:   s == s[::-1]
来源：http://ell.shanyushiyangtech.top

PHP:  $s === strrev($s);
来源：http://uro.xuanzx.com

JS:   s === [...s].reverse().join("")
来源：http://eye.jyoumei.cn

TS:   s === [...s].reverse().join("")
来源：http://nvf.xziqi.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://vnu.gotoacloud.top

Go:   // 双指针从两端比较
来源：http://oxu.52xcode.cn

Ruby: s == s.reverse
来源：http://ejj.havefunace.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://mhp.daxiang520.top

[N07] 两数之和（返回下标）
来源：http://yqg.jlsjyb.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://dns.redwolf501.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://xue.zdbjq.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://eby.c1oappe.top

TS:   // 手写 Map<string, number>
来源：http://lae.shanyushiyangtech.top

Java: // 手写 HashMap
来源：http://alz.ydzc1.top

Go:   // 手写 map[int]int
来源：http://hla.ydjk.org.cn

Ruby: // 手写 Hash
来源：http://fiz.jinqigfzy.top

C#:   // 手写 Dictionary<int, int>
来源：http://afm.snrcjt.cn

[N08] 生成全排列
来源：http://nxb.ehwqpu.com

Py:   itertools.permutations(arr)
来源：http://urq.pengpengdd.cyou

PHP:  // 手写递归交换
来源：http://jap.ywan-chungtsiang.top

JS:   // 手写回溯递归
来源：http://jxx.nanxinkj.top

TS:   // 手写回溯递归
来源：http://roa.zdqjudy.top

Java: // 手写回溯递归
来源：http://ckl.fehbvm.com

Go:   // 手写回溯递归
来源：http://ibj.fktsv.cn

Ruby: arr.permutation.to_a
来源：http://css.jqgfzy.top

C#:   // 手写回溯递归
来源：http://dsu.guowangkeji.top

[N09] 栈与队列
来源：http://xrj.vehdjk.com

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://rdr.yfazqb.com

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://znd.vqdsnc.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://jbs.jinqigufen.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://gok.guannengcc.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://txl.hongshengwenyu.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://olx.xingfuxueyuan.xyz

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hyn.jinqigfzy.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://nwj.cdnleiting.top

[N10] 链表节点定义
来源：http://lmw.cucudq.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wmj.daria6918.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://aeq.hysaishi.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://slz.jinyuanbaomall.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://bil.andypj.xyz

Java: class Node { int v; Node next; }
来源：http://cde.epnwcf.com

Go:   type Node struct { V int; Next *Node }
来源：http://iie.0kj1m.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://zuw.mhx1999.top

C#:   class Node { public int V; public Node? Next; }
来源：http://pjf.smart0.xyz

[N11] 二叉树中序遍历
来源：http://bpr.snrcjt.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://bcg.tanke756.top

PHP:  // 手写递归函数
来源：http://fnz.jinqigufen.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://dgn.zycfv.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://jqd.0kj1m.cn

Java: // 手写递归
来源：http://xzg.yongpay.top

Go:   // 手写递归
来源：http://fgp.kuanghao11.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://stw.smart0.xyz

C#:   // 手写递归
来源：http://fex.jinyuanbaomall.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://dow.feifeiyinyue.top


<!-- 参考信息 -->