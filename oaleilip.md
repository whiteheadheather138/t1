代发 wailian999

JS:   JSON.stringify(obj, null, 2)
来源：http://gnh.svipenyu.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://nfe.vehdjk.com

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://pab.hesvh.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://mva.dianchejie.cn

Ruby: JSON.pretty_generate(obj)
来源：http://efc.xylfe.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hgp.jqgufenzy.top

[K04] 读取 JSON 文件
来源：http://qik.yuxming.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://zyl.ywan-chungtsiang.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ooe.cheryme.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://whi.wangdashe.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://jrd.fktsv.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hbg.tianlin.xyz

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://mgh.jiagoushi.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://epk.zhaomingkeji.xyz

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://mda.xinyue.icu

[K05] 深拷贝对象
来源：http://zec.jinyuanbaomall.cn

Py:   copy.deepcopy(obj)
来源：http://zzj.xinyue.icu

PHP:  unserialize(serialize($obj));
来源：http://zfr.aizwys.cn

JS:   structuredClone(obj)
来源：http://fiu.tanke756.top

TS:   structuredClone(obj)
来源：http://qvy.aibaodan.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://ucy.aizwys.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://nqr.tanke756.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://mcs.yangfankeji.com

C#:   // 序列化往返，或自定义 Clone
来源：http://ufw.c1oappe.top

[K06] 解析 URL 查询串
来源：http://zvc.xylfe.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://dfj.pengpengdd.cyou

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mgc.cheryme.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://dvd.shangyingyoupin.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wsd.yuanzhike.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://irv.cashguo.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://heb.pengpengdd.cyou

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://arm.ybcxt.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://elf.yfazqb.com

[K07] 进制转换
来源：http://eak.zhaomingkeji.xyz

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ilg.chenzaomai.com

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://kyj.cucudq.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://szq.tian-w.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://uah.ybcxt.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://iwb.cucudq.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mvt.yongpay.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://kax.xylfe.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://gkr.meibo888.top

[K08] 二进制序列化（非 JSON）
来源：http://zdr.jlsjyb.cn

Py:   pickle.dumps(obj)
来源：http://xpf.aizwys.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://fvv.cheryme.top

JS:   v8.serialize(obj)        // Node
来源：http://tox.chenlongwang.top

TS:   v8.serialize(obj)        // Node
来源：http://vpx.xuetiantiany.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://pxu.tarul.cn

Go:   encoding/gob
来源：http://zra.sjlbkw.cn

Ruby: Marshal.dump(obj)
来源：http://biv.nanxinkj.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://zpa.aibaodan.cn

================================================================================
来源：http://tug.hnqzz.top

L. 网络请求
来源：http://apf.fehbvm.com

================================================================================
来源：http://udn.xinyue.icu

[L01] 发送 GET 请求
来源：http://inc.fktsv.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://vnf.fehbvm.com

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://fiw.guannengcc.top

JS:   await fetch(url)
来源：http://eyz.meibo888.top

TS:   await fetch(url)
来源：http://gyb.cashguo.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://jvv.xylfe.cn

Go:   resp, err := http.Get(url)
来源：http://rfi.zhoulong.xyz

Ruby: Net::HTTP.get(URI(url))
来源：http://idj.jianghu66.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://clk.mhx1999.top

[L02] 发送 POST JSON
来源：http://fau.ydjk.org.cn

Py:   requests.post(url, json={"a": 1})
来源：http://jjs.wangdashe.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://zkt.cdnleiting.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ygz.zhengqikj.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://xgu.9152youxi.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://qll.jlsjyb.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://uoo.guowangkeji.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ync.zhijiandao.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://fvs.fktsv.cn

[L03] 设置自定义请求头
来源：http://flx.hywenlv.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://gcu.jiagoushi.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mkk.jqgufenzy.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://pfb.hnxiangtu.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://onc.xziqi.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://fim.sxryk.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://blw.dashuyun.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://dje.vqdsnc.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hor.yuanzhike.top

[L04] 设置超时
来源：http://htn.ehwqpu.com

Py:   requests.get(url, timeout=5)
来源：http://yhc.fehbvm.com

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://yce.fanxiaobao.xyz

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://age.nanxinkj.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://thg.hongshengwenyu.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://edr.kuanghao11.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://dgv.quarkkingdee.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ecl.cqqwz.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://eih.birdmap.top

[L05] 上传文件（multipart）
来源：http://gvw.hesvh.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://lxa.316326.xyz

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://zqz.gotoacloud.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hvv.mhx1999.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://jor.feifeiyinyue.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ouf.sweek.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ywu.fzhhl.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://nfe.fzhhl.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://weu.birdmap.top

[L06] 解析响应为 JSON
来源：http://wov.ctjpmb.com

Py:   resp.json()
来源：http://jwo.cucudq.cn

PHP:  json_decode($body, true);
来源：http://anx.nwbrower.top

JS:   await resp.json()
来源：http://yhc.feifeiyinyue.top

TS:   await resp.json()
来源：http://nqz.yangfankeji.com

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://rnf.nanxuanxn.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wgp.tarul.cn

Ruby: JSON.parse(resp.body)
来源：http://kax.xuanzx.com

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://nfb.guannengcc.top

[L07] 处理 HTTP 状态码
来源：http://bfz.bbcook.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://rrg.bbcook.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://utv.xuanzx.com

JS:   resp.ok;  resp.status
来源：http://bji.xuetiantiany.cn

TS:   resp.ok;  resp.status
来源：http://agl.hysaishi.cn

Java: resp.statusCode()
来源：http://qmo.zdqjudy.top

Go:   resp.StatusCode
来源：http://qae.jlsjyb.cn

Ruby: resp.code.to_i
来源：http://gte.ppjwa.cn

C#:   (int)resp.StatusCode
来源：http://bcn.nwbrower.top

[L08] 并发请求多个地址
来源：http://xrr.nanxinkj.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://vsr.ydjk.org.cn

PHP:  curl_multi_init() 系列
来源：http://glm.jianghu66.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://pur.aizwys.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://rae.shanyushiyangkeji.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://xca.zhiwuduotai.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://iby.aibaodan.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://tto.xylfe.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://klw.zdqjudy.top

================================================================================
来源：http://urz.ybcxt.top

M. 命令行 / 进程 / 环境
来源：http://fhj.yuxming.cn

================================================================================
来源：http://nyu.tianlin.xyz

[M01] 读取命令行参数
来源：http://cej.svipenyu.cn

Py:   sys.argv[1:]
来源：http://qoi.smart0.xyz

PHP:  $argv;  $argc;
来源：http://efs.shanyushiyangtech.top

JS:   process.argv.slice(2)
来源：http://tco.ybcxt.top

TS:   process.argv.slice(2)
来源：http://upy.feifeiyinyue.top

Java: args 数组（main 方法参数）
来源：http://efs.vehdjk.com

Go:   os.Args[1:]
来源：http://mwu.tianlin.xyz

Ruby: ARGV
来源：http://dav.zycfv.cn

C#:   args 数组（Main 方法参数）
来源：http://lbu.yj20258888.top

[M02] 读取环境变量
来源：http://bgp.tanke756.top

Py:   os.environ.get("HOME")
来源：http://bvm.ehwqpu.com

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://prf.zhoulong.xyz

JS:   process.env.HOME
来源：http://cen.yuanzhike.top

TS:   process.env.HOME
来源：http://pid.xinyue.icu

Java: System.getenv("HOME")
来源：http://ctp.yueranfly.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://huz.tanke756.top

Ruby: ENV["HOME"]
来源：http://rru.zhijiandao.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://orx.vehdjk.com

[M03] 执行外部命令
来源：http://bdh.hongshengwenyu.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://zlv.shuidangran.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://jpn.xuanzx.com

JS:   child_process.execSync("ls -l").toString()
来源：http://wid.guannengcc.top

TS:   child_process.execSync("ls -l").toString()
来源：http://vol.svipenyu.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://yeb.smart0.xyz

Go:   exec.Command("ls", "-l").Output()
来源：http://whb.tian-w.cn

Ruby: system("ls -l");  `ls -l`
来源：http://bks.hywenlv.cn

C#:   Process.Start("ls", "-l");
来源：http://yan.zdqjudy.top

[M04] 获取当前工作目录
来源：http://sww.hesvh.cn

Py:   os.getcwd()
来源：http://gpz.iojbl.cn

PHP:  getcwd();
来源：http://vfe.aizwys.cn

JS:   process.cwd()
来源：http://ngn.uphjek.com

TS:   process.cwd()
来源：http://szy.zdqjudy.top

Java: Path.of("").toAbsolutePath()
来源：http://djs.mhx1999.top

Go:   os.Getwd()
来源：http://kth.dianchejie.cn

Ruby: Dir.pwd
来源：http://xul.sufxvd.cn

C#:   Directory.GetCurrentDirectory()
来源：http://stv.chenjidiqi.icu

[M05] 设置退出码
来源：http://cya.andypj.xyz

Py:   sys.exit(1)
来源：http://vua.shzxlz.cn

PHP:  exit(1);
来源：http://tqi.xylfe.cn

JS:   process.exit(1)
来源：http://oty.guannengcc.top

TS:   process.exit(1)
来源：http://kss.andypj.xyz

Java: System.exit(1)
来源：http://gpx.gotoacloud.top

Go:   os.Exit(1)
来源：http://zmf.yuxming.cn

Ruby: exit 1
来源：http://ixv.yj20258.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ogy.fanxiaobao.xyz

[M06] 向标准错误输出
来源：http://zhe.chenlongwang.top

Py:   print("err", file=sys.stderr)
来源：http://cqb.316326.xyz

PHP:  fwrite(STDERR, "err\n");
来源：http://rie.ivvv.top

JS:   console.error("err")
来源：http://nrq.tianlin.xyz

TS:   console.error("err")
来源：http://frq.cdnleiting.top

Java: System.err.println("err")
来源：http://dio.tian-w.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://xip.cdnleiting.top

Ruby: warn "err"
来源：http://uir.daria6918.cn

C#:   Console.Error.WriteLine("err")
来源：http://jkq.quarkkingdee.top

[M07] 判断是否为主入口
来源：http://twy.yuanzhike.top

Py:   if __name__ == "__main__":
来源：http://nen.xylfe.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://bhf.aizwys.cn

JS:   require.main === module
来源：http://ndb.pengpengdd.cyou

TS:   require.main === module
来源：http://pcu.jinqigfzy.top

Java: public static void main(String[] args)
来源：http://izt.hesvh.cn

Go:   func main()
来源：http://aku.vehdjk.com

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://irg.yangfankeji.com

C#:   static void Main(string[] args)
来源：http://lvc.hywenlv.cn

[M08] 获取系统与运行时信息
来源：http://tcz.pycfn.com

Py:   platform.system();  platform.python_version()
来源：http://wol.sxryk.cn

PHP:  PHP_OS;  phpversion();
来源：http://wab.zhoulong.xyz

JS:   process.platform;  process.version
来源：http://uol.hysaishi.cn

TS:   process.platform;  process.version
来源：http://brq.haohaochexian.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://szf.cdnleiting.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://rqf.0kj1m.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://euf.zhoulong.xyz

C#:   Environment.OSVersion;  Environment.Version
来源：http://bmi.yvedp.cn

================================================================================
来源：http://hhg.sxryk.cn

N. 数据结构与算法
来源：http://idx.birdmap.top

================================================================================
来源：http://por.nanxinkj.top

[N01] 二分查找（有序数组）
来源：http://ope.chenjidiqi.icu

Py:   bisect.bisect_left(arr, x)
来源：http://rpb.sweek.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hlo.dianchejie.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://nmv.zhiwuduotai.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://zcw.hywenlv.cn

Java: Arrays.binarySearch(arr, x)
来源：http://wmu.birdmap.top

Go:   sort.SearchInts(arr, x)
来源：http://snv.jiagoushi.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://vqo.nanxuanxn.top

C#:   Array.BinarySearch(arr, x)
来源：http://qvp.xingfuxueyuan.xyz

[N02] 排序（工程实践用内置实现）
来源：http://xll.ivvv.top

Py:   sorted(arr);  arr.sort()
来源：http://ual.fanxiaobao.xyz

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://jpo.yj20258.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://oym.uphjek.com

TS:   [...arr].sort((a, b) => a - b)
来源：http://duy.yuxming.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hgg.zdqjudy.top

Go:   slices.Sort(arr)
来源：http://yci.zhixingplan.top

Ruby: arr.sort
来源：http://xic.jqgfzy.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://pzr.xinyue.icu

[N03] 快速排序（分治示例）
来源：http://pqn.chenjidiqi.icu

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://iiz.ydjk.org.cn

PHP:  // 递归实现，或用 usort
来源：http://bfq.yonumen.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://rlu.daria6918.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ojh.316326.xyz

Java: // 手写递归，或直接用 Arrays.sort
来源：http://knm.ppjwa.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ucx.fehbvm.com

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ohn.hcnkem.com

C#:   // 手写递归，或 Array.Sort
来源：http://fqp.316326.xyz

[N04] 斐波那契数列
来源：http://anw.nwbrower.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://pys.9152youxi.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://vyb.gaohongyu789.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ahb.zhoulong.xyz

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://qmf.bjfxy.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hwc.hcnkem.com

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://chx.sxryk.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://xpx.ehwqpu.com

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://vjm.yvedp.cn

[N05] 最大公约数
来源：http://jwh.hfpthk.cn

Py:   math.gcd(a, b)
来源：http://sgf.gaohongyu789.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ktt.dashuyun.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://iau.fktsv.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ata.yanxiufei.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://jxw.jianghu66.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://gwm.fktsv.cn

Ruby: a.gcd(b)
来源：http://wod.52xcode.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://gcm.chenzaomai.com

[N06] 判断回文字符串
来源：http://irm.dianchejie.cn

Py:   s == s[::-1]
来源：http://pci.316326.xyz

PHP:  $s === strrev($s);
来源：http://acd.yueranfly.top

JS:   s === [...s].reverse().join("")
来源：http://jlt.gzhubu.top

TS:   s === [...s].reverse().join("")
来源：http://cqc.zdbjq.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hfx.gogol.net.cn

Go:   // 双指针从两端比较
来源：http://ghm.daria6918.cn

Ruby: s == s.reverse
来源：http://qya.dashuyun.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://ypw.jqgfzy.top

[N07] 两数之和（返回下标）
来源：http://sut.chenjidiqi.icu

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://qsk.yueranfly.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://rgc.shanyushiyangkeji.top

JS:   // 手写 Map：map.set(v, i)
来源：http://agg.iojbl.cn

TS:   // 手写 Map<string, number>
来源：http://rxg.uphjek.com

Java: // 手写 HashMap
来源：http://vzq.ivvv.top

Go:   // 手写 map[int]int
来源：http://kdu.xinyue.icu

Ruby: // 手写 Hash
来源：http://fih.hongshengwenyu.top

C#:   // 手写 Dictionary<int, int>
来源：http://krk.nanxinkj.top

[N08] 生成全排列
来源：http://gnp.fengsongda.top

Py:   itertools.permutations(arr)
来源：http://azv.bbcook.cn

PHP:  // 手写递归交换
来源：http://kmg.nanxinkj.top

JS:   // 手写回溯递归
来源：http://bls.jianghu66.top

TS:   // 手写回溯递归
来源：http://rpw.yueranfly.top

Java: // 手写回溯递归
来源：http://zjx.yonumen.top

Go:   // 手写回溯递归
来源：http://qnj.c1oappe.top

Ruby: arr.permutation.to_a
来源：http://sqc.zhiwuduotai.top

C#:   // 手写回溯递归
来源：http://wyf.nanxuanxn.top

[N09] 栈与队列
来源：http://cwq.shanyushiyangtech.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hgi.fehbvm.com

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://fcx.feifeiyinyue.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://cdx.aibaodan.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ulb.birdmap.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ttq.sjlbkw.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://fjz.zhongyouzk.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://tjz.ctjpmb.com

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://zwt.ydjk.org.cn

[N10] 链表节点定义
来源：http://abe.ivvv.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://fpe.zhoulong.xyz

PHP:  class Node { public $v; public $next = null; }
来源：http://hzi.dashuyun.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://nea.zhixingplan.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://vjx.birdmap.top

Java: class Node { int v; Node next; }
来源：http://ukw.yj20258.top

Go:   type Node struct { V int; Next *Node }
来源：http://ilu.chenzaomai.com

Ruby: Node = Struct.new(:v, :next)
来源：http://lga.jyoumei.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://xpv.jqgfzy.top

[N11] 二叉树中序遍历
来源：http://txe.jinqigfzy.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ejd.nanxuanxn.top

PHP:  // 手写递归函数
来源：http://fzs.jinqigufen.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://kzj.yueranfly.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://meg.jinqigufen.top

Java: // 手写递归
来源：http://myw.hywenlv.cn


<!-- 参考信息 -->