代发 wailian999

TS:   JSON.parse(s)
来源：http://nwh.yueranfly.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://tpm.iojbl.cn

Go:   json.Unmarshal(data, &v)
来源：http://jdf.fanxiaobao.xyz

Ruby: JSON.parse(s)
来源：http://dph.nwbrower.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://gvu.xinyue.icu

[K03] JSON 美化输出（带缩进）
来源：http://mbd.jinyuanbaomall.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://qix.cqqwz.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://nfd.jlsjyb.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://rdm.pengpengdd.cyou

TS:   JSON.stringify(obj, null, 2)
来源：http://glp.fehbvm.com

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://oyv.cheryme.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ulf.zhongyouzk.top

Ruby: JSON.pretty_generate(obj)
来源：http://wtu.cqqwz.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://jlv.cashguo.top

[K04] 读取 JSON 文件
来源：http://wuh.iojbl.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://nok.yueranfly.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://dya.zdbjq.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ark.jyoumei.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://cxd.ywan-chungtsiang.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://sux.shzxlz.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ezh.yangfankeji.com

Ruby: JSON.parse(File.read("a.json"))
来源：http://qqg.xuetiantiany.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://cws.vqdsnc.cn

[K05] 深拷贝对象
来源：http://zap.hysaishi.cn

Py:   copy.deepcopy(obj)
来源：http://zuu.chenjidiqi.icu

PHP:  unserialize(serialize($obj));
来源：http://cdf.havefunace.top

JS:   structuredClone(obj)
来源：http://geq.wangshuangyany.cn

TS:   structuredClone(obj)
来源：http://qmt.yuxming.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://wum.nanxuanxn.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://cin.chenlongwang.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://cjo.gaohongyu789.top

C#:   // 序列化往返，或自定义 Clone
来源：http://sju.fengsongda.top

[K06] 解析 URL 查询串
来源：http://luz.ybcxt.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://vic.zhoulong.xyz

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://fov.xylfe.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://uqz.shangyingyoupin.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ftx.c1oappe.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hff.fanxiaobao.xyz

Go:   url.ParseQuery("a=1&b=2")
来源：http://uuy.jiagoushi.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://tzp.zhongyouzk.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://bhp.shangyingyoupin.top

[K07] 进制转换
来源：http://jyh.svipenyu.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://nvn.wangdashe.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://gyt.cheryme.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://vqk.bbcook.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://soq.yueranfly.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://yva.chenjidiqi.icu

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://cxi.mhx1999.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://pjj.nwbrower.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://pcs.gotoacloud.top

[K08] 二进制序列化（非 JSON）
来源：http://npo.yonumen.top

Py:   pickle.dumps(obj)
来源：http://wgc.guannengcc.top

PHP:  serialize($obj);  unserialize($s);
来源：http://eth.ywan-chungtsiang.top

JS:   v8.serialize(obj)        // Node
来源：http://apy.tarul.cn

TS:   v8.serialize(obj)        // Node
来源：http://apz.smart0.xyz

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://kcp.yanxiufei.cn

Go:   encoding/gob
来源：http://rmm.haohaochexian.top

Ruby: Marshal.dump(obj)
来源：http://vmj.hysaishi.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://tmr.cqqwz.cn

================================================================================
来源：http://vxy.andypj.xyz

L. 网络请求
来源：http://orh.shzxlz.cn

================================================================================
来源：http://lsu.jinyuanbaomall.cn

[L01] 发送 GET 请求
来源：http://wds.0kj1m.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://aya.gotoacloud.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://nlm.zhijiandao.cn

JS:   await fetch(url)
来源：http://apw.yfazqb.com

TS:   await fetch(url)
来源：http://oha.jqgfzy.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://vws.ivvv.top

Go:   resp, err := http.Get(url)
来源：http://jtl.gzhubu.top

Ruby: Net::HTTP.get(URI(url))
来源：http://gqe.hammf.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://yti.yuxming.cn

[L02] 发送 POST JSON
来源：http://rqt.gogol.net.cn

Py:   requests.post(url, json={"a": 1})
来源：http://nel.yj202588.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ehc.yonumen.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://fcs.daria6918.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://tsd.cdnleiting.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://smh.guannengcc.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ont.nanxinkj.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://zug.316326.xyz

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://czn.ydzc1.top

[L03] 设置自定义请求头
来源：http://oss.cashguo.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://lrw.snrcjt.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ezf.pengpengdd.cyou

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://kbi.shuidangran.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ojp.ctjpmb.com

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://vcw.ehwqpu.com

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://rao.nwbrower.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://vxh.xuanzx.com

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://vxo.zhaomingkeji.xyz

[L04] 设置超时
来源：http://ujt.daria6918.cn

Py:   requests.get(url, timeout=5)
来源：http://non.jiagoushi.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wrh.hfpthk.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://fmt.zdqjudy.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://uke.hongshengwenyu.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mnk.xuanzx.com

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wtn.xuanzx.com

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://zlt.cheryme.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://zxa.gzhubu.top

[L05] 上传文件（multipart）
来源：http://bwd.hongshengwenyu.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ahi.xziqi.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://eup.mhx1999.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://cyy.bjfxy.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://esl.yvedp.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://tih.iojbl.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://vte.yueranfly.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://eop.dashuyun.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://afe.sweek.top

[L06] 解析响应为 JSON
来源：http://xup.daria6918.cn

Py:   resp.json()
来源：http://jly.ctjpmb.com

PHP:  json_decode($body, true);
来源：http://ybq.pengpengdd.cyou

JS:   await resp.json()
来源：http://znd.yfazqb.com

TS:   await resp.json()
来源：http://ejt.tianlin.xyz

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://piu.jyoumei.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://tsj.yj20258888.top

Ruby: JSON.parse(resp.body)
来源：http://qtz.jianghu66.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://rtd.havefunace.top

[L07] 处理 HTTP 状态码
来源：http://vxg.dashuyun.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ohl.yj202588.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://lyy.gotoacloud.top

JS:   resp.ok;  resp.status
来源：http://cnx.chenzaomai.com

TS:   resp.ok;  resp.status
来源：http://hgg.snrcjt.cn

Java: resp.statusCode()
来源：http://zhr.quarkkingdee.top

Go:   resp.StatusCode
来源：http://qdg.ywan-chungtsiang.top

Ruby: resp.code.to_i
来源：http://ola.0kj1m.cn

C#:   (int)resp.StatusCode
来源：http://hzc.hysaishi.cn

[L08] 并发请求多个地址
来源：http://kkd.zdbjq.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://dnl.ctjpmb.com

PHP:  curl_multi_init() 系列
来源：http://dfj.zhongyouzk.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://kee.shzxlz.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mbq.bbcook.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ont.jinqigufen.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mii.vehdjk.com

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mzh.mhx1999.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://zng.yongpay.top

================================================================================
来源：http://nvj.wangshuangyany.cn

M. 命令行 / 进程 / 环境
来源：http://uhr.sufxvd.cn

================================================================================
来源：http://erb.zhoulong.xyz

[M01] 读取命令行参数
来源：http://itk.cucudq.cn

Py:   sys.argv[1:]
来源：http://ujm.xylfe.cn

PHP:  $argv;  $argc;
来源：http://vxf.iojbl.cn

JS:   process.argv.slice(2)
来源：http://bmt.zhaomingkeji.xyz

TS:   process.argv.slice(2)
来源：http://psy.tanke756.top

Java: args 数组（main 方法参数）
来源：http://duz.hywenlv.cn

Go:   os.Args[1:]
来源：http://trc.shuidangran.top

Ruby: ARGV
来源：http://aab.hcnkem.com

C#:   args 数组（Main 方法参数）
来源：http://syp.yfazqb.com

[M02] 读取环境变量
来源：http://tqy.yueranfly.top

Py:   os.environ.get("HOME")
来源：http://tcy.redwolf501.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://vxt.0kj1m.cn

JS:   process.env.HOME
来源：http://zfu.dianchejie.cn

TS:   process.env.HOME
来源：http://sif.hysaishi.cn

Java: System.getenv("HOME")
来源：http://iol.sysykeji.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://dqp.cqqwz.cn

Ruby: ENV["HOME"]
来源：http://afh.epnwcf.com

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://dja.smart0.xyz

[M03] 执行外部命令
来源：http://eai.yanxiufei.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://bde.sxryk.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://yfs.ivvv.top

JS:   child_process.execSync("ls -l").toString()
来源：http://fsq.jinqigfzy.top

TS:   child_process.execSync("ls -l").toString()
来源：http://oyu.redwolf501.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://zoh.ppjwa.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://hsd.hfpthk.cn

Ruby: system("ls -l");  `ls -l`
来源：http://ygn.jinghuilouyu.cn

C#:   Process.Start("ls", "-l");
来源：http://vbb.zhoulong.xyz

[M04] 获取当前工作目录
来源：http://quw.haohaochexian.top

Py:   os.getcwd()
来源：http://nns.birdmap.top

PHP:  getcwd();
来源：http://yww.tarul.cn

JS:   process.cwd()
来源：http://hjn.hongshengwenyu.top

TS:   process.cwd()
来源：http://qkj.fehbvm.com

Java: Path.of("").toAbsolutePath()
来源：http://mwa.nanxuanxn.top

Go:   os.Getwd()
来源：http://yve.sysykeji.top

Ruby: Dir.pwd
来源：http://kjz.gzhubu.top

C#:   Directory.GetCurrentDirectory()
来源：http://jpa.shanyushiyangtech.top

[M05] 设置退出码
来源：http://wqh.yuxming.cn

Py:   sys.exit(1)
来源：http://dhk.zhengqikj.top

PHP:  exit(1);
来源：http://ymm.ybcxt.top

JS:   process.exit(1)
来源：http://qfk.meibo888.top

TS:   process.exit(1)
来源：http://tyj.andypj.xyz

Java: System.exit(1)
来源：http://cvo.ywan-chungtsiang.top

Go:   os.Exit(1)
来源：http://iar.nanxinkj.top

Ruby: exit 1
来源：http://spz.vehdjk.com

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://pyl.hfpthk.cn

[M06] 向标准错误输出
来源：http://sgr.zdbjq.cn

Py:   print("err", file=sys.stderr)
来源：http://lak.ctjpmb.com

PHP:  fwrite(STDERR, "err\n");
来源：http://vbf.pengpengdd.cyou

JS:   console.error("err")
来源：http://uke.c1oappe.top

TS:   console.error("err")
来源：http://gpb.bbcook.cn

Java: System.err.println("err")
来源：http://ynm.zhoulong.xyz

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ghp.fzhhl.top

Ruby: warn "err"
来源：http://nmj.ehwqpu.com

C#:   Console.Error.WriteLine("err")
来源：http://zus.shanyushiyangtech.top

[M07] 判断是否为主入口
来源：http://djm.hywenlv.cn

Py:   if __name__ == "__main__":
来源：http://sfn.yj20258888.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://slt.jqgufenzy.top

JS:   require.main === module
来源：http://ynl.shuidangran.top

TS:   require.main === module
来源：http://nku.xingfuxueyuan.xyz

Java: public static void main(String[] args)
来源：http://wgr.guannengcc.top

Go:   func main()
来源：http://iqo.zycfv.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://lzu.xuanzx.com

C#:   static void Main(string[] args)
来源：http://bcf.cqqwz.cn

[M08] 获取系统与运行时信息
来源：http://axe.zhaomingkeji.xyz

Py:   platform.system();  platform.python_version()
来源：http://ggz.yj202588.top

PHP:  PHP_OS;  phpversion();
来源：http://eqw.aizwys.cn

JS:   process.platform;  process.version
来源：http://rzj.yj202588.top

TS:   process.platform;  process.version
来源：http://muv.bjfxy.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://qfc.gotoacloud.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://xoj.birdmap.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hpi.yueranfly.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://byl.zhongyouzk.top

================================================================================
来源：http://myu.hesvh.cn

N. 数据结构与算法
来源：http://hmy.yj202588.top

================================================================================
来源：http://zse.nanxuanxn.top

[N01] 二分查找（有序数组）
来源：http://exq.xinyue.icu

Py:   bisect.bisect_left(arr, x)
来源：http://tft.meibo888.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://lyn.nanxuanxn.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://rql.52xcode.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://fkf.chenzaomai.com

Java: Arrays.binarySearch(arr, x)
来源：http://qcc.sxryk.cn

Go:   sort.SearchInts(arr, x)
来源：http://evm.yueranfly.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://xxm.chenzaomai.com

C#:   Array.BinarySearch(arr, x)
来源：http://wmr.jqgufenzy.top

[N02] 排序（工程实践用内置实现）
来源：http://mcq.yj202588.top

Py:   sorted(arr);  arr.sort()
来源：http://rod.nwbrower.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://cyy.shanyushiyangtech.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://vou.c1oappe.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://gop.yongpay.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mpk.yanxiufei.cn

Go:   slices.Sort(arr)
来源：http://cvz.bjfxy.top

Ruby: arr.sort
来源：http://zuq.yanxiufei.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://uei.hnqzz.top

[N03] 快速排序（分治示例）
来源：http://fzw.ybcxt.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ddt.yongpay.top

PHP:  // 递归实现，或用 usort
来源：http://xry.zdbjq.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://kum.guowangkeji.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://gjm.yuxming.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://nsz.shzxlz.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://kxj.bjfxy.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://qym.fktsv.cn

C#:   // 手写递归，或 Array.Sort
来源：http://sbo.sysykeji.top

[N04] 斐波那契数列
来源：http://mty.c1oappe.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://kvs.yangfankeji.com

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://pha.fzhhl.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://kjm.tianlin.xyz

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://cqq.xingfuxueyuan.xyz

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://phb.yanxiufei.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://zkl.cucudq.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://sid.xuetiantiany.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://zup.0kj1m.cn

[N05] 最大公约数
来源：http://luj.xziqi.cn

Py:   math.gcd(a, b)
来源：http://ofl.bbcook.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://tmw.yj20258888.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://eay.yj202588.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://cyl.aizwys.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://sec.cheryme.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mcx.zhongyouzk.top

Ruby: a.gcd(b)
来源：http://fon.pengpengdd.cyou

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://zeh.sufxvd.cn

[N06] 判断回文字符串
来源：http://lzm.jqgufenzy.top

Py:   s == s[::-1]
来源：http://dpi.guannengcc.top

PHP:  $s === strrev($s);
来源：http://xcm.wangdashe.top

JS:   s === [...s].reverse().join("")
来源：http://neb.fanxiaobao.xyz

TS:   s === [...s].reverse().join("")
来源：http://ddq.cdnleiting.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://gyf.cashguo.top

Go:   // 双指针从两端比较
来源：http://qlg.daxiang520.top

Ruby: s == s.reverse
来源：http://bkh.jlsjyb.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://jdq.yangfankeji.com

[N07] 两数之和（返回下标）
来源：http://kqc.daxiang520.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://cgn.fzhhl.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hcd.yangfankeji.com

JS:   // 手写 Map：map.set(v, i)
来源：http://dtm.hnxiangtu.top

TS:   // 手写 Map<string, number>
来源：http://xdq.daxiang520.top

Java: // 手写 HashMap
来源：http://hov.gogol.net.cn

Go:   // 手写 map[int]int
来源：http://udc.hammf.cn

Ruby: // 手写 Hash
来源：http://dxn.wangshuangyany.cn

C#:   // 手写 Dictionary<int, int>
来源：http://kyt.smart0.xyz

[N08] 生成全排列
来源：http://sum.52xcode.cn

Py:   itertools.permutations(arr)
来源：http://zrv.yj202588.top

PHP:  // 手写递归交换
来源：http://kdc.yonumen.top

JS:   // 手写回溯递归
来源：http://hmm.ctjpmb.com

TS:   // 手写回溯递归
来源：http://dsh.gzhubu.top

Java: // 手写回溯递归
来源：http://xbi.fanxiaobao.xyz

Go:   // 手写回溯递归
来源：http://pdy.chenlongwang.top

Ruby: arr.permutation.to_a
来源：http://bsn.uphjek.com

C#:   // 手写回溯递归
来源：http://vjs.cashguo.top

[N09] 栈与队列
来源：http://kab.zycfv.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ltt.dianchejie.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ghl.jlsjyb.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://myl.hesvh.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mgy.cheryme.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://knz.shzxlz.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://zgp.mhx1999.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wjk.yj20258.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://zdm.haohaochexian.top

[N10] 链表节点定义
来源：http://knh.hcnkem.com

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://yhg.pengpengdd.cyou

PHP:  class Node { public $v; public $next = null; }
来源：http://xsb.yangfankeji.com

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://bqx.hnqzz.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://gvo.snrcjt.cn

Java: class Node { int v; Node next; }
来源：http://exq.tian-w.cn

Go:   type Node struct { V int; Next *Node }
来源：http://pad.fzhhl.top


<!-- 参考信息 -->