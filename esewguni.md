代发 wailian999

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://rbc.yongpay.top

[K03] JSON 美化输出（带缩进）
来源：http://ylm.shuidangran.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://rvx.nanxinkj.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wbo.zhixingplan.top

JS:   JSON.stringify(obj, null, 2)
来源：http://bou.cashguo.top

TS:   JSON.stringify(obj, null, 2)
来源：http://vqx.gogol.net.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://huk.daxiang520.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://zfo.ehwqpu.com

Ruby: JSON.pretty_generate(obj)
来源：http://hqm.xuanzx.com

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://txb.gotoacloud.top

[K04] 读取 JSON 文件
来源：http://wok.daria6918.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://loc.chenzaomai.com

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ubr.daxiang520.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://uzq.yj20258.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://nri.yonumen.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://lxv.xingfuxueyuan.xyz

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://awc.hysaishi.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://vcs.hfpthk.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://cpn.xylfe.cn

[K05] 深拷贝对象
来源：http://kkv.ybcxt.top

Py:   copy.deepcopy(obj)
来源：http://zdc.yfazqb.com

PHP:  unserialize(serialize($obj));
来源：http://yqz.tian-w.cn

JS:   structuredClone(obj)
来源：http://wtf.yj20258.top

TS:   structuredClone(obj)
来源：http://xqq.yonumen.top

Java: // 手写拷贝构造，或序列化往返
来源：http://klx.wangshuangyany.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://idu.hammf.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://bcs.ehwqpu.com

C#:   // 序列化往返，或自定义 Clone
来源：http://gvr.9152youxi.cn

[K06] 解析 URL 查询串
来源：http://vbw.yj20258888.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://xwc.ywan-chungtsiang.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://rjp.shangyingyoupin.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://zof.zhoulong.xyz

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://nwj.fktsv.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://tki.c1oappe.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://ybm.ppjwa.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wri.yongpay.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://odb.yj20258888.top

[K07] 进制转换
来源：http://grn.fengsongda.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://axw.sxryk.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://lnb.52xcode.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://tdz.cqqwz.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://pkc.smart0.xyz

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://uoh.guowangkeji.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ekp.pycfn.com

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://tql.shanyushiyangkeji.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://jvy.ywan-chungtsiang.top

[K08] 二进制序列化（非 JSON）
来源：http://cju.sxryk.cn

Py:   pickle.dumps(obj)
来源：http://kky.vehdjk.com

PHP:  serialize($obj);  unserialize($s);
来源：http://bix.kuanghao11.cn

JS:   v8.serialize(obj)        // Node
来源：http://mnf.jqgfzy.top

TS:   v8.serialize(obj)        // Node
来源：http://yfs.iojbl.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://khw.yuxming.cn

Go:   encoding/gob
来源：http://loc.aizwys.cn

Ruby: Marshal.dump(obj)
来源：http://okv.gzhubu.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ngj.zhixingplan.top

================================================================================
来源：http://bsp.yfazqb.com

L. 网络请求
来源：http://cqm.jianghu66.top

================================================================================
来源：http://vml.316326.xyz

[L01] 发送 GET 请求
来源：http://shp.hnqzz.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wqr.ppjwa.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://nva.gaohongyu789.top

JS:   await fetch(url)
来源：http://bhm.hongshengwenyu.top

TS:   await fetch(url)
来源：http://sef.yueranfly.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://xvs.ybcxt.top

Go:   resp, err := http.Get(url)
来源：http://ahr.vqdsnc.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://unn.vqdsnc.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://aof.hesvh.cn

[L02] 发送 POST JSON
来源：http://ryh.guowangkeji.top

Py:   requests.post(url, json={"a": 1})
来源：http://mud.mhx1999.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://itn.yj202588.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://dbm.ctjpmb.com

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://src.hnqzz.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://yjq.xingfuxueyuan.xyz

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ppg.hongshengwenyu.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://esz.hcnkem.com

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://esr.zhaomingkeji.xyz

[L03] 设置自定义请求头
来源：http://fjs.zhoulong.xyz

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://yda.bjfxy.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://gui.dashuyun.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mmh.jqgfzy.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://slh.tian-w.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wbf.dashuyun.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://kut.meibo888.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://szq.xinyue.icu

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://aff.jianghu66.top

[L04] 设置超时
来源：http://fvd.jlsjyb.cn

Py:   requests.get(url, timeout=5)
来源：http://jnu.shuidangran.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://lbz.chenlongwang.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://rgc.pycfn.com

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://nbo.ydjk.org.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hgf.yj20258.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://bih.meibo888.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://fbw.yfazqb.com

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wxq.hammf.cn

[L05] 上传文件（multipart）
来源：http://bud.zhaomingkeji.xyz

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://tik.zycfv.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ajt.yueranfly.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://rkm.bbcook.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://vql.xuanzx.com

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://gjc.gogol.net.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://bey.vqdsnc.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://khm.quarkkingdee.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://qco.hammf.cn

[L06] 解析响应为 JSON
来源：http://szc.uphjek.com

Py:   resp.json()
来源：http://exe.yongpay.top

PHP:  json_decode($body, true);
来源：http://zba.sjlbkw.cn

JS:   await resp.json()
来源：http://izx.guowangkeji.top

TS:   await resp.json()
来源：http://ves.zdbjq.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wft.xuanzx.com

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://kwv.ppjwa.cn

Ruby: JSON.parse(resp.body)
来源：http://xsw.jianghu66.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://eni.xuetiantiany.cn

[L07] 处理 HTTP 状态码
来源：http://csl.cdnleiting.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://rqn.shangyingyoupin.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://kwf.xuanzx.com

JS:   resp.ok;  resp.status
来源：http://dxf.jqgfzy.top

TS:   resp.ok;  resp.status
来源：http://mqe.yj20258888.top

Java: resp.statusCode()
来源：http://xwa.ctjpmb.com

Go:   resp.StatusCode
来源：http://rlo.cdnleiting.top

Ruby: resp.code.to_i
来源：http://hle.mhx1999.top

C#:   (int)resp.StatusCode
来源：http://jrh.zhoulong.xyz

[L08] 并发请求多个地址
来源：http://yfi.zhixingplan.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://xgp.shanyushiyangkeji.top

PHP:  curl_multi_init() 系列
来源：http://dwu.smart0.xyz

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ota.zhixingplan.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://sog.zdbjq.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://utl.pycfn.com

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://afh.zhijiandao.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://fjm.yj20258888.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://pkj.yfazqb.com

================================================================================
来源：http://mur.yonumen.top

M. 命令行 / 进程 / 环境
来源：http://aqq.shuidangran.top

================================================================================
来源：http://kbk.sxryk.cn

[M01] 读取命令行参数
来源：http://vna.gotoacloud.top

Py:   sys.argv[1:]
来源：http://ywx.gaohongyu789.top

PHP:  $argv;  $argc;
来源：http://ikq.hywenlv.cn

JS:   process.argv.slice(2)
来源：http://oit.zycfv.cn

TS:   process.argv.slice(2)
来源：http://bgq.ctjpmb.com

Java: args 数组（main 方法参数）
来源：http://tok.hywenlv.cn

Go:   os.Args[1:]
来源：http://mgu.tanke756.top

Ruby: ARGV
来源：http://hpl.iojbl.cn

C#:   args 数组（Main 方法参数）
来源：http://ant.vqdsnc.cn

[M02] 读取环境变量
来源：http://ypa.zhoulong.xyz

Py:   os.environ.get("HOME")
来源：http://lpm.svipenyu.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://rwo.fktsv.cn

JS:   process.env.HOME
来源：http://djt.shangyingyoupin.top

TS:   process.env.HOME
来源：http://jwx.birdmap.top

Java: System.getenv("HOME")
来源：http://pwj.jinghuilouyu.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://doa.chenlongwang.top

Ruby: ENV["HOME"]
来源：http://dne.yj202588.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://okk.svipenyu.cn

[M03] 执行外部命令
来源：http://wjq.tian-w.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://bhp.tian-w.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://qwg.hfpthk.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://pzd.yueranfly.top

TS:   child_process.execSync("ls -l").toString()
来源：http://kds.pengpengdd.cyou

Java: new ProcessBuilder("ls", "-l").start()
来源：http://dtf.yonumen.top

Go:   exec.Command("ls", "-l").Output()
来源：http://wkb.0kj1m.cn

Ruby: system("ls -l");  `ls -l`
来源：http://wnv.jyoumei.cn

C#:   Process.Start("ls", "-l");
来源：http://ysx.jinqigufen.top

[M04] 获取当前工作目录
来源：http://trc.52xcode.cn

Py:   os.getcwd()
来源：http://hcm.smart0.xyz

PHP:  getcwd();
来源：http://uph.havefunace.top

JS:   process.cwd()
来源：http://bqp.ydjk.org.cn

TS:   process.cwd()
来源：http://fxw.zhaomingkeji.xyz

Java: Path.of("").toAbsolutePath()
来源：http://cfe.zhoulong.xyz

Go:   os.Getwd()
来源：http://vvq.zhaomingkeji.xyz

Ruby: Dir.pwd
来源：http://xmp.birdmap.top

C#:   Directory.GetCurrentDirectory()
来源：http://qae.ctjpmb.com

[M05] 设置退出码
来源：http://gbm.cheryme.top

Py:   sys.exit(1)
来源：http://ppm.52xcode.cn

PHP:  exit(1);
来源：http://ehu.pengpengdd.cyou

JS:   process.exit(1)
来源：http://bem.andypj.xyz

TS:   process.exit(1)
来源：http://cht.xylfe.cn

Java: System.exit(1)
来源：http://era.ehwqpu.com

Go:   os.Exit(1)
来源：http://wbf.quarkkingdee.top

Ruby: exit 1
来源：http://gdy.gogol.net.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ffh.shzxlz.cn

[M06] 向标准错误输出
来源：http://iao.hfpthk.cn

Py:   print("err", file=sys.stderr)
来源：http://ykj.gaohongyu789.top

PHP:  fwrite(STDERR, "err\n");
来源：http://dsw.tian-w.cn

JS:   console.error("err")
来源：http://nnl.guowangkeji.top

TS:   console.error("err")
来源：http://cvw.meibo888.top

Java: System.err.println("err")
来源：http://sjy.epnwcf.com

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mgs.zdqjudy.top

Ruby: warn "err"
来源：http://cjs.shanyushiyangtech.top

C#:   Console.Error.WriteLine("err")
来源：http://wgt.zycfv.cn

[M07] 判断是否为主入口
来源：http://krv.yangfankeji.com

Py:   if __name__ == "__main__":
来源：http://ocm.zhongyouzk.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://rla.redwolf501.top

JS:   require.main === module
来源：http://iga.0kj1m.cn

TS:   require.main === module
来源：http://bnj.c1oappe.top

Java: public static void main(String[] args)
来源：http://uuv.gogol.net.cn

Go:   func main()
来源：http://fcy.xuanzx.com

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://bss.jqgufenzy.top

C#:   static void Main(string[] args)
来源：http://twm.chenzaomai.com

[M08] 获取系统与运行时信息
来源：http://jpy.yvedp.cn

Py:   platform.system();  platform.python_version()
来源：http://cab.zdbjq.cn

PHP:  PHP_OS;  phpversion();
来源：http://rhw.jyoumei.cn

JS:   process.platform;  process.version
来源：http://ytk.c1oappe.top

TS:   process.platform;  process.version
来源：http://ann.ybcxt.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://sro.hnxiangtu.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://fwl.wangshuangyany.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hzg.yanxiufei.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://viu.sweek.top

================================================================================
来源：http://rea.fzhhl.top

N. 数据结构与算法
来源：http://juv.xziqi.cn

================================================================================
来源：http://yql.ppjwa.cn

[N01] 二分查找（有序数组）
来源：http://czz.fzhhl.top

Py:   bisect.bisect_left(arr, x)
来源：http://yys.jyoumei.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://nxq.daxiang520.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://eyr.epnwcf.com

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://lir.hfpthk.cn

Java: Arrays.binarySearch(arr, x)
来源：http://iwo.quarkkingdee.top

Go:   sort.SearchInts(arr, x)
来源：http://gry.daxiang520.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://hgl.gotoacloud.top

C#:   Array.BinarySearch(arr, x)
来源：http://ygl.yangfankeji.com

[N02] 排序（工程实践用内置实现）
来源：http://rkh.vehdjk.com

Py:   sorted(arr);  arr.sort()
来源：http://bjy.nwbrower.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://qpi.mhx1999.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://imb.shzxlz.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://ckz.yvedp.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://dtl.cucudq.cn

Go:   slices.Sort(arr)
来源：http://ndk.xingfuxueyuan.xyz

Ruby: arr.sort
来源：http://ndh.cqqwz.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://ycl.shangyingyoupin.top

[N03] 快速排序（分治示例）
来源：http://uvi.jiagoushi.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://tbb.jinyuanbaomall.cn

PHP:  // 递归实现，或用 usort
来源：http://uif.zhaomingkeji.xyz

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://tqc.tarul.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://cjv.pycfn.com

Java: // 手写递归，或直接用 Arrays.sort
来源：http://emb.gzhubu.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://lno.sweek.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://rsu.jlsjyb.cn

C#:   // 手写递归，或 Array.Sort
来源：http://gsp.sxryk.cn

[N04] 斐波那契数列
来源：http://obb.mhx1999.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://zie.bjfxy.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://kjm.jlsjyb.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://jnt.havefunace.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://qhp.hywenlv.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ubi.xylfe.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hwp.jinqigufen.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://onb.c1oappe.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://xjy.ybcxt.top

[N05] 最大公约数
来源：http://qsg.jinghuilouyu.cn

Py:   math.gcd(a, b)
来源：http://jsa.jinyuanbaomall.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://str.svipenyu.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://uxh.shuidangran.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wdy.yonumen.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://fkr.xingfuxueyuan.xyz

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://qco.redwolf501.top

Ruby: a.gcd(b)
来源：http://mnd.zhijiandao.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://chs.svipenyu.cn

[N06] 判断回文字符串
来源：http://txo.jinqigufen.top

Py:   s == s[::-1]
来源：http://ikn.sjlbkw.cn

PHP:  $s === strrev($s);
来源：http://irh.cheryme.top

JS:   s === [...s].reverse().join("")
来源：http://mse.tanke756.top

TS:   s === [...s].reverse().join("")
来源：http://fef.dianchejie.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://yar.xinyue.icu

Go:   // 双指针从两端比较
来源：http://nom.c1oappe.top

Ruby: s == s.reverse
来源：http://klu.yfazqb.com

C#:   s == new string(s.Reverse().ToArray())
来源：http://ivb.sweek.top

[N07] 两数之和（返回下标）
来源：http://wfp.0kj1m.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ipt.ydzc1.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://xte.tanke756.top

JS:   // 手写 Map：map.set(v, i)
来源：http://kon.daxiang520.top

TS:   // 手写 Map<string, number>
来源：http://ltf.gaohongyu789.top

Java: // 手写 HashMap
来源：http://htv.ydjk.org.cn

Go:   // 手写 map[int]int
来源：http://wsi.yuanzhike.top

Ruby: // 手写 Hash
来源：http://vzm.fzhhl.top

C#:   // 手写 Dictionary<int, int>
来源：http://vor.yuxming.cn

[N08] 生成全排列
来源：http://mvs.ivvv.top

Py:   itertools.permutations(arr)
来源：http://stx.jianghu66.top

PHP:  // 手写递归交换
来源：http://mpv.jqgufenzy.top

JS:   // 手写回溯递归
来源：http://gwg.sufxvd.cn

TS:   // 手写回溯递归
来源：http://qgz.yuxming.cn

Java: // 手写回溯递归
来源：http://ytw.shzxlz.cn

Go:   // 手写回溯递归
来源：http://vfx.gogol.net.cn

Ruby: arr.permutation.to_a
来源：http://qqt.xuetiantiany.cn

C#:   // 手写回溯递归
来源：http://vih.shanyushiyangkeji.top

[N09] 栈与队列
来源：http://stp.cashguo.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://yzk.hcnkem.com

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://zqv.meibo888.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://dlz.vehdjk.com

TS:   arr.push(x) / arr.pop() 作栈
来源：http://oou.redwolf501.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mhm.dianchejie.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ldm.ehwqpu.com

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hvo.shzxlz.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://jgi.yj20258.top

[N10] 链表节点定义
来源：http://pmm.tanke756.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://prk.fehbvm.com

PHP:  class Node { public $v; public $next = null; }
来源：http://ody.9152youxi.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wqt.pengpengdd.cyou

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://yux.ybcxt.top

Java: class Node { int v; Node next; }
来源：http://txe.hesvh.cn

Go:   type Node struct { V int; Next *Node }
来源：http://ywg.vqdsnc.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://sdr.jlsjyb.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://fzv.guowangkeji.top

[N11] 二叉树中序遍历
来源：http://nvo.xuanzx.com

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ond.tian-w.cn


<!-- 参考信息 -->