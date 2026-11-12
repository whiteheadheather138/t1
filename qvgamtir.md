代发 wailian999

JS:   JSON.stringify(obj, null, 2)
来源：http://mch.yfazqb.com

TS:   JSON.stringify(obj, null, 2)
来源：http://ndh.wangdashe.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ohs.svipenyu.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://jkl.jinqigfzy.top

Ruby: JSON.pretty_generate(obj)
来源：http://bbd.wangdashe.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://fdh.birdmap.top

[K04] 读取 JSON 文件
来源：http://zhg.nwbrower.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://spi.jinqigufen.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://whm.hesvh.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://yoz.yj20258.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://jtv.jqgufenzy.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://qnt.pengpengdd.cyou

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://qsl.meibo888.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://vba.ydzc1.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://mmp.sweek.top

[K05] 深拷贝对象
来源：http://ona.0kj1m.cn

Py:   copy.deepcopy(obj)
来源：http://cts.yj20258.top

PHP:  unserialize(serialize($obj));
来源：http://qro.yuanzhike.top

JS:   structuredClone(obj)
来源：http://pxo.havefunace.top

TS:   structuredClone(obj)
来源：http://gow.smart0.xyz

Java: // 手写拷贝构造，或序列化往返
来源：http://bvo.hammf.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://dxs.xziqi.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://rlv.hongshengwenyu.top

C#:   // 序列化往返，或自定义 Clone
来源：http://ojq.shangyingyoupin.top

[K06] 解析 URL 查询串
来源：http://vzd.shuidangran.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://dfo.yj20258888.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://fug.xylfe.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://rqd.chenzaomai.com

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://gpb.mhx1999.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://gff.xuetiantiany.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://dec.smart0.xyz

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://djw.mhx1999.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://xai.xziqi.cn

[K07] 进制转换
来源：http://sni.zycfv.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://fvs.guowangkeji.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://zjh.yongpay.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://sot.yangfankeji.com

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://igj.sufxvd.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://thm.hnxiangtu.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ppa.wangdashe.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://nmv.fzhhl.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://iux.hammf.cn

[K08] 二进制序列化（非 JSON）
来源：http://qld.316326.xyz

Py:   pickle.dumps(obj)
来源：http://zyd.9152youxi.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://cmr.kuanghao11.cn

JS:   v8.serialize(obj)        // Node
来源：http://rbx.52xcode.cn

TS:   v8.serialize(obj)        // Node
来源：http://hfj.ehwqpu.com

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://bzv.iojbl.cn

Go:   encoding/gob
来源：http://xoi.ehwqpu.com

Ruby: Marshal.dump(obj)
来源：http://oqc.havefunace.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://pmk.shanyushiyangkeji.top

================================================================================
来源：http://lgq.yuanzhike.top

L. 网络请求
来源：http://czq.tarul.cn

================================================================================
来源：http://jjz.svipenyu.cn

[L01] 发送 GET 请求
来源：http://btm.fanxiaobao.xyz

Py:   requests.get(url)                        # 第三方库 requests
来源：http://qnd.9152youxi.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://aul.shzxlz.cn

JS:   await fetch(url)
来源：http://dqd.fktsv.cn

TS:   await fetch(url)
来源：http://eaj.tanke756.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://wyq.haohaochexian.top

Go:   resp, err := http.Get(url)
来源：http://oxq.zhiwuduotai.top

Ruby: Net::HTTP.get(URI(url))
来源：http://foy.yj20258.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://jef.shzxlz.cn

[L02] 发送 POST JSON
来源：http://gcp.xuetiantiany.cn

Py:   requests.post(url, json={"a": 1})
来源：http://qoc.jinghuilouyu.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://xuf.zhaomingkeji.xyz

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ufm.uphjek.com

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://pdw.zhoulong.xyz

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wue.sysykeji.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://kcx.hongshengwenyu.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://cbg.andypj.xyz

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://tri.redwolf501.top

[L03] 设置自定义请求头
来源：http://lie.c1oappe.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wwy.ehwqpu.com

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ihs.smart0.xyz

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://zpu.chenjidiqi.icu

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://rkp.kuanghao11.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://lxm.hfpthk.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://igv.daria6918.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://cyr.cdnleiting.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://nmm.vehdjk.com

[L04] 设置超时
来源：http://yuv.ywan-chungtsiang.top

Py:   requests.get(url, timeout=5)
来源：http://lis.havefunace.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://jit.dashuyun.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mrp.shanyushiyangtech.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://rob.daxiang520.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://vrn.yj20258.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://fsr.52xcode.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://upc.yangfankeji.com

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://awc.sjlbkw.cn

[L05] 上传文件（multipart）
来源：http://kba.hywenlv.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://kaz.xingfuxueyuan.xyz

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://iyo.yongpay.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://fgv.zdbjq.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ocq.fzhhl.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://esx.jlsjyb.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://nhl.xingfuxueyuan.xyz

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mpm.gaohongyu789.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://lrx.yangfankeji.com

[L06] 解析响应为 JSON
来源：http://xhv.gaohongyu789.top

Py:   resp.json()
来源：http://wev.jinqigfzy.top

PHP:  json_decode($body, true);
来源：http://jcm.xuanzx.com

JS:   await resp.json()
来源：http://til.ppjwa.cn

TS:   await resp.json()
来源：http://awr.yuanzhike.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://iil.vqdsnc.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://xmj.jqgfzy.top

Ruby: JSON.parse(resp.body)
来源：http://yky.yvedp.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://qzp.jyoumei.cn

[L07] 处理 HTTP 状态码
来源：http://zyt.xinyue.icu

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ckp.pycfn.com

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wxq.jinqigufen.top

JS:   resp.ok;  resp.status
来源：http://xzs.gogol.net.cn

TS:   resp.ok;  resp.status
来源：http://adc.yanxiufei.cn

Java: resp.statusCode()
来源：http://rih.daxiang520.top

Go:   resp.StatusCode
来源：http://ekx.cheryme.top

Ruby: resp.code.to_i
来源：http://zve.ybcxt.top

C#:   (int)resp.StatusCode
来源：http://oaq.cucudq.cn

[L08] 并发请求多个地址
来源：http://gyy.yongpay.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://adf.ydzc1.top

PHP:  curl_multi_init() 系列
来源：http://sae.jinyuanbaomall.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wsd.chenjidiqi.icu

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://lcx.tarul.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://rfa.fanxiaobao.xyz

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://cot.andypj.xyz

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ujx.hammf.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://tpo.shuidangran.top

================================================================================
来源：http://nni.jyoumei.cn

M. 命令行 / 进程 / 环境
来源：http://nvx.gaohongyu789.top

================================================================================
来源：http://bls.0kj1m.cn

[M01] 读取命令行参数
来源：http://xzr.gogol.net.cn

Py:   sys.argv[1:]
来源：http://yak.epnwcf.com

PHP:  $argv;  $argc;
来源：http://cjq.cashguo.top

JS:   process.argv.slice(2)
来源：http://vuu.hammf.cn

TS:   process.argv.slice(2)
来源：http://khp.jinqigfzy.top

Java: args 数组（main 方法参数）
来源：http://wmh.jqgufenzy.top

Go:   os.Args[1:]
来源：http://cdx.yuanzhike.top

Ruby: ARGV
来源：http://uzj.nanxuanxn.top

C#:   args 数组（Main 方法参数）
来源：http://ggt.andypj.xyz

[M02] 读取环境变量
来源：http://utw.feifeiyinyue.top

Py:   os.environ.get("HOME")
来源：http://qgg.nanxuanxn.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://uhe.xinyue.icu

JS:   process.env.HOME
来源：http://gyu.yueranfly.top

TS:   process.env.HOME
来源：http://rkk.hnqzz.top

Java: System.getenv("HOME")
来源：http://vwu.jiagoushi.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://eoc.yonumen.top

Ruby: ENV["HOME"]
来源：http://top.sjlbkw.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://oag.daria6918.cn

[M03] 执行外部命令
来源：http://cen.daria6918.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://qrl.havefunace.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wcg.chenlongwang.top

JS:   child_process.execSync("ls -l").toString()
来源：http://ast.vehdjk.com

TS:   child_process.execSync("ls -l").toString()
来源：http://phs.gaohongyu789.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://pyo.shanyushiyangkeji.top

Go:   exec.Command("ls", "-l").Output()
来源：http://rkl.tianlin.xyz

Ruby: system("ls -l");  `ls -l`
来源：http://pmk.xuanzx.com

C#:   Process.Start("ls", "-l");
来源：http://wmw.smart0.xyz

[M04] 获取当前工作目录
来源：http://ltj.chenjidiqi.icu

Py:   os.getcwd()
来源：http://wcq.jinqigfzy.top

PHP:  getcwd();
来源：http://vyo.hammf.cn

JS:   process.cwd()
来源：http://ltp.jinqigfzy.top

TS:   process.cwd()
来源：http://zzf.fehbvm.com

Java: Path.of("").toAbsolutePath()
来源：http://slz.hysaishi.cn

Go:   os.Getwd()
来源：http://pnc.cashguo.top

Ruby: Dir.pwd
来源：http://kzd.xuetiantiany.cn

C#:   Directory.GetCurrentDirectory()
来源：http://duh.dashuyun.cn

[M05] 设置退出码
来源：http://tgr.nwbrower.top

Py:   sys.exit(1)
来源：http://roi.xziqi.cn

PHP:  exit(1);
来源：http://woq.fktsv.cn

JS:   process.exit(1)
来源：http://url.jqgfzy.top

TS:   process.exit(1)
来源：http://hxq.sjlbkw.cn

Java: System.exit(1)
来源：http://icc.zhengqikj.top

Go:   os.Exit(1)
来源：http://kqg.yj202588.top

Ruby: exit 1
来源：http://sgk.bjfxy.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://whn.xinyue.icu

[M06] 向标准错误输出
来源：http://myn.shuidangran.top

Py:   print("err", file=sys.stderr)
来源：http://btz.zhijiandao.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://qhg.zhengqikj.top

JS:   console.error("err")
来源：http://xnu.yfazqb.com

TS:   console.error("err")
来源：http://iby.ppjwa.cn

Java: System.err.println("err")
来源：http://tne.xingfuxueyuan.xyz

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://xad.bjfxy.top

Ruby: warn "err"
来源：http://rqw.zhixingplan.top

C#:   Console.Error.WriteLine("err")
来源：http://oou.ydzc1.top

[M07] 判断是否为主入口
来源：http://bne.wangdashe.top

Py:   if __name__ == "__main__":
来源：http://owh.jinqigfzy.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hll.cdnleiting.top

JS:   require.main === module
来源：http://gyc.bbcook.cn

TS:   require.main === module
来源：http://gxh.jiagoushi.top

Java: public static void main(String[] args)
来源：http://kem.wangdashe.top

Go:   func main()
来源：http://abu.bbcook.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://zga.yuxming.cn

C#:   static void Main(string[] args)
来源：http://pgv.sysykeji.top

[M08] 获取系统与运行时信息
来源：http://lzu.hysaishi.cn

Py:   platform.system();  platform.python_version()
来源：http://gzp.hnqzz.top

PHP:  PHP_OS;  phpversion();
来源：http://dvo.cucudq.cn

JS:   process.platform;  process.version
来源：http://fwi.jinqigfzy.top

TS:   process.platform;  process.version
来源：http://stq.nwbrower.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://zhv.ybcxt.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://giu.tian-w.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://lkt.wangdashe.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://cue.yangfankeji.com

================================================================================
来源：http://dch.hywenlv.cn

N. 数据结构与算法
来源：http://ioj.yuanzhike.top

================================================================================
来源：http://uek.316326.xyz

[N01] 二分查找（有序数组）
来源：http://pwj.0kj1m.cn

Py:   bisect.bisect_left(arr, x)
来源：http://zzs.bjfxy.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://kkb.tian-w.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mqx.cashguo.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://qvz.shanyushiyangkeji.top

Java: Arrays.binarySearch(arr, x)
来源：http://cbw.cqqwz.cn

Go:   sort.SearchInts(arr, x)
来源：http://xms.shuidangran.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://sfg.jinghuilouyu.cn

C#:   Array.BinarySearch(arr, x)
来源：http://qis.ctjpmb.com

[N02] 排序（工程实践用内置实现）
来源：http://ban.jinyuanbaomall.cn

Py:   sorted(arr);  arr.sort()
来源：http://mui.xingfuxueyuan.xyz

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://bmt.ydzc1.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://ifv.bjfxy.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://ncg.xylfe.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hgv.havefunace.top

Go:   slices.Sort(arr)
来源：http://ksz.bjfxy.top

Ruby: arr.sort
来源：http://qqp.yongpay.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://kgb.hesvh.cn

[N03] 快速排序（分治示例）
来源：http://skw.jqgufenzy.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://aga.nanxuanxn.top

PHP:  // 递归实现，或用 usort
来源：http://oyc.zhengqikj.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://elt.vehdjk.com

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://yvk.daria6918.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://vtu.yonumen.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hpu.zhijiandao.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://omo.shanyushiyangtech.top

C#:   // 手写递归，或 Array.Sort
来源：http://qja.shanyushiyangtech.top

[N04] 斐波那契数列
来源：http://psu.daria6918.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://pmc.smart0.xyz

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ecl.cucudq.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://zjg.cheryme.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hgv.sufxvd.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://trx.ydjk.org.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://cdu.redwolf501.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://fkw.jqgfzy.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://idm.yfazqb.com

[N05] 最大公约数
来源：http://kdg.mhx1999.top

Py:   math.gcd(a, b)
来源：http://mkn.jinghuilouyu.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://uha.nanxuanxn.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mgj.yj20258888.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://jlh.daria6918.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://bnk.yuanzhike.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ekk.ppjwa.cn

Ruby: a.gcd(b)
来源：http://orm.epnwcf.com

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mvi.redwolf501.top

[N06] 判断回文字符串
来源：http://jnq.sxryk.cn

Py:   s == s[::-1]
来源：http://bvr.tanke756.top

PHP:  $s === strrev($s);
来源：http://ygb.zhixingplan.top

JS:   s === [...s].reverse().join("")
来源：http://bhc.hfpthk.cn

TS:   s === [...s].reverse().join("")
来源：http://zpf.cheryme.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://qap.feifeiyinyue.top

Go:   // 双指针从两端比较
来源：http://wse.tianlin.xyz

Ruby: s == s.reverse
来源：http://qhg.zdbjq.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://ncn.jqgfzy.top

[N07] 两数之和（返回下标）
来源：http://kxp.nanxinkj.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://est.0kj1m.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mgc.ydjk.org.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://qvg.tanke756.top

TS:   // 手写 Map<string, number>
来源：http://ksy.jlsjyb.cn

Java: // 手写 HashMap
来源：http://cbr.dianchejie.cn

Go:   // 手写 map[int]int
来源：http://aym.jinyuanbaomall.cn

Ruby: // 手写 Hash
来源：http://api.ivvv.top

C#:   // 手写 Dictionary<int, int>
来源：http://yup.quarkkingdee.top

[N08] 生成全排列
来源：http://abc.yangfankeji.com

Py:   itertools.permutations(arr)
来源：http://nmt.shuidangran.top

PHP:  // 手写递归交换
来源：http://dkk.zhengqikj.top

JS:   // 手写回溯递归
来源：http://tpt.xylfe.cn

TS:   // 手写回溯递归
来源：http://cmb.zdbjq.cn

Java: // 手写回溯递归
来源：http://qrr.xingfuxueyuan.xyz

Go:   // 手写回溯递归
来源：http://mpi.zdbjq.cn

Ruby: arr.permutation.to_a
来源：http://uqb.meibo888.top

C#:   // 手写回溯递归
来源：http://uvk.chenjidiqi.icu

[N09] 栈与队列
来源：http://kmh.yfazqb.com

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://zlk.yangfankeji.com

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://fby.sufxvd.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://rvd.ydzc1.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://skz.zhaomingkeji.xyz

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://xza.dianchejie.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wba.nanxuanxn.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://kxr.sufxvd.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://dbe.hammf.cn

[N10] 链表节点定义
来源：http://npc.fktsv.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hui.fanxiaobao.xyz

PHP:  class Node { public $v; public $next = null; }
来源：http://uhv.shuidangran.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wcv.mhx1999.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://fam.cqqwz.cn

Java: class Node { int v; Node next; }
来源：http://brq.jlsjyb.cn

Go:   type Node struct { V int; Next *Node }
来源：http://eyx.zycfv.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://pim.cdnleiting.top

C#:   class Node { public int V; public Node? Next; }
来源：http://ghm.iojbl.cn

[N11] 二叉树中序遍历
来源：http://llz.cqqwz.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://fxh.gogol.net.cn

PHP:  // 手写递归函数
来源：http://bzv.fktsv.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://vrw.ydzc1.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blf.hfpthk.cn

Java: // 手写递归
来源：http://ujm.quarkkingdee.top


<!-- 参考信息 -->