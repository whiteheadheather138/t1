代发 wailian999

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://zru.9152youxi.cn

[K03] JSON 美化输出（带缩进）
来源：http://yml.tian-w.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://qxi.gaohongyu789.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://jpj.hnqzz.top

JS:   JSON.stringify(obj, null, 2)
来源：http://pnq.snrcjt.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://avv.hfpthk.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ftl.yj20258888.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://qio.jlsjyb.cn

Ruby: JSON.pretty_generate(obj)
来源：http://lrw.52xcode.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://abh.nanxuanxn.top

[K04] 读取 JSON 文件
来源：http://jvt.fktsv.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://kcy.chenjidiqi.icu

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://azh.sufxvd.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://fkn.tian-w.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://sbn.shzxlz.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mlg.xingfuxueyuan.xyz

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hme.jyoumei.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://fpn.tian-w.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ybg.cucudq.cn

[K05] 深拷贝对象
来源：http://ufi.hammf.cn

Py:   copy.deepcopy(obj)
来源：http://jpy.fzhhl.top

PHP:  unserialize(serialize($obj));
来源：http://qhy.jyoumei.cn

JS:   structuredClone(obj)
来源：http://zbi.shanyushiyangkeji.top

TS:   structuredClone(obj)
来源：http://gyn.snrcjt.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://lzz.tarul.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://gxc.hnqzz.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ogg.wangshuangyany.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://gjr.gogol.net.cn

[K06] 解析 URL 查询串
来源：http://yug.sweek.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ubo.hywenlv.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://eny.hywenlv.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ulm.cashguo.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://keo.jlsjyb.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://kiz.dashuyun.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://zly.wangdashe.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://vnz.zhiwuduotai.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ptx.sxryk.cn

[K07] 进制转换
来源：http://ekn.dashuyun.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://lxw.gzhubu.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hsn.shzxlz.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://yco.svipenyu.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://axp.aibaodan.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ygl.svipenyu.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://rxx.epnwcf.com

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ndo.gotoacloud.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://tmm.zhijiandao.cn

[K08] 二进制序列化（非 JSON）
来源：http://qwa.bjfxy.top

Py:   pickle.dumps(obj)
来源：http://urs.yvedp.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://yzu.chenjidiqi.icu

JS:   v8.serialize(obj)        // Node
来源：http://dku.ybcxt.top

TS:   v8.serialize(obj)        // Node
来源：http://xwl.xuetiantiany.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://daa.cheryme.top

Go:   encoding/gob
来源：http://oyi.jqgfzy.top

Ruby: Marshal.dump(obj)
来源：http://ohu.svipenyu.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://zzf.haohaochexian.top

================================================================================
来源：http://ppi.jinghuilouyu.cn

L. 网络请求
来源：http://dyd.jyoumei.cn

================================================================================
来源：http://jjk.zhiwuduotai.top

[L01] 发送 GET 请求
来源：http://wkt.iojbl.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://gnf.shanyushiyangtech.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://owl.0kj1m.cn

JS:   await fetch(url)
来源：http://zdl.wangdashe.top

TS:   await fetch(url)
来源：http://hsn.bbcook.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://naj.hysaishi.cn

Go:   resp, err := http.Get(url)
来源：http://gmt.sweek.top

Ruby: Net::HTTP.get(URI(url))
来源：http://yyh.aizwys.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ynh.cheryme.top

[L02] 发送 POST JSON
来源：http://tef.ydzc1.top

Py:   requests.post(url, json={"a": 1})
来源：http://jxa.gogol.net.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hay.shanyushiyangtech.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ykq.shzxlz.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://izk.vqdsnc.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://brs.cqqwz.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://eqh.yuanzhike.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://vgl.hammf.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wth.ppjwa.cn

[L03] 设置自定义请求头
来源：http://wnx.ivvv.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://tkq.nwbrower.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://fsn.fktsv.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://zsc.daria6918.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://tjp.jqgfzy.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://yof.52xcode.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://soy.chenjidiqi.icu

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://nud.gogol.net.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://oxz.shanyushiyangkeji.top

[L04] 设置超时
来源：http://zku.chenzaomai.com

Py:   requests.get(url, timeout=5)
来源：http://hbu.hesvh.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://nsf.yangfankeji.com

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://bft.tarul.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://szs.xylfe.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://jxr.yvedp.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://squ.shuidangran.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mtu.bjfxy.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://cdp.zhengqikj.top

[L05] 上传文件（multipart）
来源：http://snm.jqgfzy.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://vlk.ivvv.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://xyf.hesvh.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://asf.cqqwz.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hqf.hywenlv.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://itg.wangshuangyany.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://cic.daxiang520.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://otz.jyoumei.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mxy.snrcjt.cn

[L06] 解析响应为 JSON
来源：http://rot.sxryk.cn

Py:   resp.json()
来源：http://mcp.shuidangran.top

PHP:  json_decode($body, true);
来源：http://oht.dianchejie.cn

JS:   await resp.json()
来源：http://ocr.fktsv.cn

TS:   await resp.json()
来源：http://mjb.dianchejie.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ewl.chenzaomai.com

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://vuv.jlsjyb.cn

Ruby: JSON.parse(resp.body)
来源：http://nvl.vqdsnc.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://gzb.yueranfly.top

[L07] 处理 HTTP 状态码
来源：http://hfu.hywenlv.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://nzz.dianchejie.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hwv.hammf.cn

JS:   resp.ok;  resp.status
来源：http://nvx.sjlbkw.cn

TS:   resp.ok;  resp.status
来源：http://zsd.jinqigfzy.top

Java: resp.statusCode()
来源：http://gpe.shzxlz.cn

Go:   resp.StatusCode
来源：http://ooz.52xcode.cn

Ruby: resp.code.to_i
来源：http://xof.jqgfzy.top

C#:   (int)resp.StatusCode
来源：http://tlm.epnwcf.com

[L08] 并发请求多个地址
来源：http://cnz.redwolf501.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://sys.yj20258.top

PHP:  curl_multi_init() 系列
来源：http://guj.quarkkingdee.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mfw.shanyushiyangkeji.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://rxj.havefunace.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://foo.zhaomingkeji.xyz

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://vte.sxryk.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://kzz.xinyue.icu

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://apy.ivvv.top

================================================================================
来源：http://swv.shanyushiyangkeji.top

M. 命令行 / 进程 / 环境
来源：http://okz.sweek.top

================================================================================
来源：http://lnn.xuetiantiany.cn

[M01] 读取命令行参数
来源：http://pkk.jinqigufen.top

Py:   sys.argv[1:]
来源：http://bky.iojbl.cn

PHP:  $argv;  $argc;
来源：http://pyr.nwbrower.top

JS:   process.argv.slice(2)
来源：http://eak.snrcjt.cn

TS:   process.argv.slice(2)
来源：http://bke.aizwys.cn

Java: args 数组（main 方法参数）
来源：http://git.zhoulong.xyz

Go:   os.Args[1:]
来源：http://loa.chenjidiqi.icu

Ruby: ARGV
来源：http://edt.gzhubu.top

C#:   args 数组（Main 方法参数）
来源：http://vkx.yuanzhike.top

[M02] 读取环境变量
来源：http://adv.daria6918.cn

Py:   os.environ.get("HOME")
来源：http://ayr.gzhubu.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://dzf.gogol.net.cn

JS:   process.env.HOME
来源：http://eut.chenlongwang.top

TS:   process.env.HOME
来源：http://shy.sysykeji.top

Java: System.getenv("HOME")
来源：http://ynn.yj20258.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hsd.tianlin.xyz

Ruby: ENV["HOME"]
来源：http://uda.iojbl.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ggw.havefunace.top

[M03] 执行外部命令
来源：http://qzd.iojbl.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://qam.yuanzhike.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://slj.andypj.xyz

JS:   child_process.execSync("ls -l").toString()
来源：http://doc.vqdsnc.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://wgq.xingfuxueyuan.xyz

Java: new ProcessBuilder("ls", "-l").start()
来源：http://izz.yj20258.top

Go:   exec.Command("ls", "-l").Output()
来源：http://rjo.hnxiangtu.top

Ruby: system("ls -l");  `ls -l`
来源：http://gfo.vehdjk.com

C#:   Process.Start("ls", "-l");
来源：http://qqz.shangyingyoupin.top

[M04] 获取当前工作目录
来源：http://clh.chenlongwang.top

Py:   os.getcwd()
来源：http://fdf.hysaishi.cn

PHP:  getcwd();
来源：http://ynf.yangfankeji.com

JS:   process.cwd()
来源：http://igo.ppjwa.cn

TS:   process.cwd()
来源：http://jll.wangshuangyany.cn

Java: Path.of("").toAbsolutePath()
来源：http://aaz.jinqigufen.top

Go:   os.Getwd()
来源：http://rhm.uphjek.com

Ruby: Dir.pwd
来源：http://usu.shanyushiyangtech.top

C#:   Directory.GetCurrentDirectory()
来源：http://pso.hywenlv.cn

[M05] 设置退出码
来源：http://gor.zhixingplan.top

Py:   sys.exit(1)
来源：http://qgy.fengsongda.top

PHP:  exit(1);
来源：http://qvr.cucudq.cn

JS:   process.exit(1)
来源：http://yvd.tianlin.xyz

TS:   process.exit(1)
来源：http://hbv.daria6918.cn

Java: System.exit(1)
来源：http://hbi.meibo888.top

Go:   os.Exit(1)
来源：http://iqa.aibaodan.cn

Ruby: exit 1
来源：http://los.jinghuilouyu.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://dkb.mhx1999.top

[M06] 向标准错误输出
来源：http://lnc.nanxinkj.top

Py:   print("err", file=sys.stderr)
来源：http://etv.jqgufenzy.top

PHP:  fwrite(STDERR, "err\n");
来源：http://gpq.birdmap.top

JS:   console.error("err")
来源：http://bze.yj20258888.top

TS:   console.error("err")
来源：http://ddi.hfpthk.cn

Java: System.err.println("err")
来源：http://gbz.zhongyouzk.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://xqx.sxryk.cn

Ruby: warn "err"
来源：http://haa.hysaishi.cn

C#:   Console.Error.WriteLine("err")
来源：http://qhg.gaohongyu789.top

[M07] 判断是否为主入口
来源：http://jcr.birdmap.top

Py:   if __name__ == "__main__":
来源：http://ssh.aizwys.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://umu.hfpthk.cn

JS:   require.main === module
来源：http://hjb.nanxinkj.top

TS:   require.main === module
来源：http://lut.gogol.net.cn

Java: public static void main(String[] args)
来源：http://ssz.redwolf501.top

Go:   func main()
来源：http://zgm.jinghuilouyu.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://jbr.tanke756.top

C#:   static void Main(string[] args)
来源：http://ywj.tian-w.cn

[M08] 获取系统与运行时信息
来源：http://jmw.0kj1m.cn

Py:   platform.system();  platform.python_version()
来源：http://jjh.epnwcf.com

PHP:  PHP_OS;  phpversion();
来源：http://idv.guannengcc.top

JS:   process.platform;  process.version
来源：http://eqa.svipenyu.cn

TS:   process.platform;  process.version
来源：http://iwh.c1oappe.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://vkn.vqdsnc.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://ywh.zhongyouzk.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hht.sjlbkw.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://ghj.jinqigfzy.top

================================================================================
来源：http://nhm.ehwqpu.com

N. 数据结构与算法
来源：http://dks.feifeiyinyue.top

================================================================================
来源：http://fpj.zdbjq.cn

[N01] 二分查找（有序数组）
来源：http://xhv.xuanzx.com

Py:   bisect.bisect_left(arr, x)
来源：http://ayr.aizwys.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://kqd.daxiang520.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ddv.wangshuangyany.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://llc.pycfn.com

Java: Arrays.binarySearch(arr, x)
来源：http://dpk.jyoumei.cn

Go:   sort.SearchInts(arr, x)
来源：http://pxg.gogol.net.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://euo.xingfuxueyuan.xyz

C#:   Array.BinarySearch(arr, x)
来源：http://bgg.tianlin.xyz

[N02] 排序（工程实践用内置实现）
来源：http://rax.shanyushiyangtech.top

Py:   sorted(arr);  arr.sort()
来源：http://wyu.cashguo.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://jhe.aibaodan.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://fvn.hfpthk.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://sbz.zhixingplan.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://lvx.zdbjq.cn

Go:   slices.Sort(arr)
来源：http://yxe.yangfankeji.com

Ruby: arr.sort
来源：http://non.tarul.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://jiy.uphjek.com

[N03] 快速排序（分治示例）
来源：http://gwj.haohaochexian.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://lpd.fengsongda.top

PHP:  // 递归实现，或用 usort
来源：http://eey.chenlongwang.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://pvz.jlsjyb.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://dgs.xuanzx.com

Java: // 手写递归，或直接用 Arrays.sort
来源：http://bwr.cdnleiting.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://qtv.nanxuanxn.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://jee.vehdjk.com

C#:   // 手写递归，或 Array.Sort
来源：http://ism.zhiwuduotai.top

[N04] 斐波那契数列
来源：http://lgf.daria6918.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mep.gogol.net.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://lbv.c1oappe.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://vva.yonumen.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ioi.hnqzz.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://lar.sxryk.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://rqy.jinqigfzy.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://gfa.iojbl.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://uah.shzxlz.cn

[N05] 最大公约数
来源：http://hyd.quarkkingdee.top

Py:   math.gcd(a, b)
来源：http://ezr.gogol.net.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://tiq.kuanghao11.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hpr.chenzaomai.com

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://vli.aibaodan.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://suh.hesvh.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://yeo.pengpengdd.cyou

Ruby: a.gcd(b)
来源：http://nmt.jyoumei.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://qak.cdnleiting.top

[N06] 判断回文字符串
来源：http://gwn.zhiwuduotai.top

Py:   s == s[::-1]
来源：http://dje.yangfankeji.com

PHP:  $s === strrev($s);
来源：http://aru.9152youxi.cn

JS:   s === [...s].reverse().join("")
来源：http://hna.mhx1999.top

TS:   s === [...s].reverse().join("")
来源：http://ilp.hongshengwenyu.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://giz.vqdsnc.cn

Go:   // 双指针从两端比较
来源：http://ayj.sxryk.cn

Ruby: s == s.reverse
来源：http://vqm.wangdashe.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://amm.jinghuilouyu.cn

[N07] 两数之和（返回下标）
来源：http://jnt.svipenyu.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://uma.gaohongyu789.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://quj.ivvv.top

JS:   // 手写 Map：map.set(v, i)
来源：http://mid.tian-w.cn

TS:   // 手写 Map<string, number>
来源：http://bcm.zhoulong.xyz

Java: // 手写 HashMap
来源：http://qkq.jlsjyb.cn

Go:   // 手写 map[int]int
来源：http://ewt.gotoacloud.top

Ruby: // 手写 Hash
来源：http://hft.sxryk.cn

C#:   // 手写 Dictionary<int, int>
来源：http://jdz.guowangkeji.top

[N08] 生成全排列
来源：http://sef.fktsv.cn

Py:   itertools.permutations(arr)
来源：http://atc.aibaodan.cn

PHP:  // 手写递归交换
来源：http://ffg.birdmap.top

JS:   // 手写回溯递归
来源：http://oef.zycfv.cn

TS:   // 手写回溯递归
来源：http://bwu.sweek.top

Java: // 手写回溯递归
来源：http://ane.sweek.top

Go:   // 手写回溯递归
来源：http://cxr.xingfuxueyuan.xyz

Ruby: arr.permutation.to_a
来源：http://aea.guannengcc.top

C#:   // 手写回溯递归
来源：http://xpn.yuxming.cn

[N09] 栈与队列
来源：http://rzp.haohaochexian.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://jen.aizwys.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://cru.52xcode.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ajt.jyoumei.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wys.guannengcc.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://yhf.wangshuangyany.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://uyw.sxryk.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://zap.hammf.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://oaa.mhx1999.top

[N10] 链表节点定义
来源：http://pce.yj202588.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://zkc.zhengqikj.top

PHP:  class Node { public $v; public $next = null; }
来源：http://wuv.zhongyouzk.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://int.ppjwa.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://nde.ywan-chungtsiang.top

Java: class Node { int v; Node next; }
来源：http://yll.shanyushiyangkeji.top

Go:   type Node struct { V int; Next *Node }
来源：http://ppv.zdqjudy.top

Ruby: Node = Struct.new(:v, :next)
来源：http://dai.yueranfly.top

C#:   class Node { public int V; public Node? Next; }
来源：http://agy.hcnkem.com

[N11] 二叉树中序遍历
来源：http://btb.jinqigufen.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://haq.jqgufenzy.top


<!-- 参考信息 -->