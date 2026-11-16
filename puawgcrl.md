代发 wailian999

JS:   JSON.stringify(obj, null, 2)
来源：http://gvx.vehdjk.com

TS:   JSON.stringify(obj, null, 2)
来源：http://rnm.wangdashe.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://cjo.snrcjt.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://htq.birdmap.top

Ruby: JSON.pretty_generate(obj)
来源：http://oaj.xuetiantiany.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://xqq.ybcxt.top

[K04] 读取 JSON 文件
来源：http://tif.chenzaomai.com

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://wng.daria6918.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ckh.iojbl.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://xyy.snrcjt.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://aux.xingfuxueyuan.xyz

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ulh.zycfv.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://rnb.gotoacloud.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://ynv.xuetiantiany.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://rog.hammf.cn

[K05] 深拷贝对象
来源：http://aqe.fehbvm.com

Py:   copy.deepcopy(obj)
来源：http://qrk.guannengcc.top

PHP:  unserialize(serialize($obj));
来源：http://vyv.chenzaomai.com

JS:   structuredClone(obj)
来源：http://tmt.shanyushiyangtech.top

TS:   structuredClone(obj)
来源：http://duw.xziqi.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://hvb.chenlongwang.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://pwv.zhongyouzk.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ogs.zdqjudy.top

C#:   // 序列化往返，或自定义 Clone
来源：http://idu.yuxming.cn

[K06] 解析 URL 查询串
来源：http://yxj.ybcxt.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://yzu.sxryk.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://rwa.jinghuilouyu.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://agk.vqdsnc.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://zoc.ctjpmb.com

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://cbl.tanke756.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://yvz.gzhubu.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://oxo.cheryme.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://nwk.ybcxt.top

[K07] 进制转换
来源：http://bqz.hcnkem.com

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://jmo.zhongyouzk.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://pkd.ivvv.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hgj.xinyue.icu

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://vwy.shangyingyoupin.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://jat.iojbl.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://nvf.yanxiufei.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://yzp.zhiwuduotai.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ujf.fengsongda.top

[K08] 二进制序列化（非 JSON）
来源：http://ajz.yuanzhike.top

Py:   pickle.dumps(obj)
来源：http://ggs.hnqzz.top

PHP:  serialize($obj);  unserialize($s);
来源：http://qih.hysaishi.cn

JS:   v8.serialize(obj)        // Node
来源：http://qnm.vehdjk.com

TS:   v8.serialize(obj)        // Node
来源：http://mnz.yonumen.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://fld.shangyingyoupin.top

Go:   encoding/gob
来源：http://qpf.sufxvd.cn

Ruby: Marshal.dump(obj)
来源：http://mqi.zhijiandao.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://gvy.shanyushiyangtech.top

================================================================================
来源：http://rru.mhx1999.top

L. 网络请求
来源：http://nog.tanke756.top

================================================================================
来源：http://prg.xziqi.cn

[L01] 发送 GET 请求
来源：http://mlv.316326.xyz

Py:   requests.get(url)                        # 第三方库 requests
来源：http://eaa.xuanzx.com

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://lob.mhx1999.top

JS:   await fetch(url)
来源：http://cex.fktsv.cn

TS:   await fetch(url)
来源：http://tge.yangfankeji.com

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://rmm.zhoulong.xyz

Go:   resp, err := http.Get(url)
来源：http://fsr.jlsjyb.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://nbf.iojbl.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://nnq.chenjidiqi.icu

[L02] 发送 POST JSON
来源：http://hyj.jinghuilouyu.cn

Py:   requests.post(url, json={"a": 1})
来源：http://mzr.guannengcc.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://yyb.chenjidiqi.icu

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://bkw.yj20258888.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://zbk.yuanzhike.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://gbn.xuanzx.com

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ovb.chenlongwang.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hyg.iojbl.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://trd.nanxuanxn.top

[L03] 设置自定义请求头
来源：http://fmr.feifeiyinyue.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://rym.gzhubu.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ddb.havefunace.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://caq.gotoacloud.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://shb.cdnleiting.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://smo.wangshuangyany.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://lbu.guannengcc.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://nha.ywan-chungtsiang.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wdy.quarkkingdee.top

[L04] 设置超时
来源：http://vfi.hnqzz.top

Py:   requests.get(url, timeout=5)
来源：http://jft.xziqi.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://bjs.fehbvm.com

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://dvl.sjlbkw.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://twj.yangfankeji.com

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ncg.zhaomingkeji.xyz

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hiz.hnqzz.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ibf.dashuyun.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://evc.shangyingyoupin.top

[L05] 上传文件（multipart）
来源：http://grd.ywan-chungtsiang.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://lap.jiagoushi.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://bth.zhiwuduotai.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://scg.c1oappe.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://dhl.pycfn.com

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://zcn.fzhhl.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://btt.xylfe.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://xnm.jyoumei.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ufe.yvedp.cn

[L06] 解析响应为 JSON
来源：http://szq.xylfe.cn

Py:   resp.json()
来源：http://xeh.wangshuangyany.cn

PHP:  json_decode($body, true);
来源：http://udz.pycfn.com

JS:   await resp.json()
来源：http://pwd.hcnkem.com

TS:   await resp.json()
来源：http://tta.jinyuanbaomall.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://nux.vehdjk.com

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://pys.dianchejie.cn

Ruby: JSON.parse(resp.body)
来源：http://esb.9152youxi.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://bou.yfazqb.com

[L07] 处理 HTTP 状态码
来源：http://lfk.guannengcc.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://jfg.sysykeji.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://xve.jiagoushi.top

JS:   resp.ok;  resp.status
来源：http://unc.ydzc1.top

TS:   resp.ok;  resp.status
来源：http://wfa.wangdashe.top

Java: resp.statusCode()
来源：http://qtq.fengsongda.top

Go:   resp.StatusCode
来源：http://fok.yvedp.cn

Ruby: resp.code.to_i
来源：http://jvl.guannengcc.top

C#:   (int)resp.StatusCode
来源：http://jup.jinyuanbaomall.cn

[L08] 并发请求多个地址
来源：http://psv.yvedp.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://xtv.yongpay.top

PHP:  curl_multi_init() 系列
来源：http://qfp.zhixingplan.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://abo.redwolf501.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://yxl.jyoumei.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://quv.chenlongwang.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://kqm.tarul.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://kda.jinqigfzy.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ggq.fanxiaobao.xyz

================================================================================
来源：http://wuy.quarkkingdee.top

M. 命令行 / 进程 / 环境
来源：http://kio.sxryk.cn

================================================================================
来源：http://phs.tarul.cn

[M01] 读取命令行参数
来源：http://qgm.cucudq.cn

Py:   sys.argv[1:]
来源：http://lhb.yfazqb.com

PHP:  $argv;  $argc;
来源：http://fiw.redwolf501.top

JS:   process.argv.slice(2)
来源：http://lqe.316326.xyz

TS:   process.argv.slice(2)
来源：http://jxp.fengsongda.top

Java: args 数组（main 方法参数）
来源：http://kxi.zhiwuduotai.top

Go:   os.Args[1:]
来源：http://mlo.ctjpmb.com

Ruby: ARGV
来源：http://ysh.jyoumei.cn

C#:   args 数组（Main 方法参数）
来源：http://hna.guowangkeji.top

[M02] 读取环境变量
来源：http://afy.xylfe.cn

Py:   os.environ.get("HOME")
来源：http://flj.hfpthk.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://dfk.ydjk.org.cn

JS:   process.env.HOME
来源：http://ymz.ydzc1.top

TS:   process.env.HOME
来源：http://gqd.fktsv.cn

Java: System.getenv("HOME")
来源：http://gjz.yj20258.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://foi.zhengqikj.top

Ruby: ENV["HOME"]
来源：http://krt.xziqi.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://srg.zhoulong.xyz

[M03] 执行外部命令
来源：http://yts.jyoumei.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ovy.ppjwa.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://cgl.xuanzx.com

JS:   child_process.execSync("ls -l").toString()
来源：http://jyh.xziqi.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://dti.hywenlv.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://kct.cucudq.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://qlj.daria6918.cn

Ruby: system("ls -l");  `ls -l`
来源：http://mmv.nwbrower.top

C#:   Process.Start("ls", "-l");
来源：http://qms.jlsjyb.cn

[M04] 获取当前工作目录
来源：http://wub.zycfv.cn

Py:   os.getcwd()
来源：http://agu.52xcode.cn

PHP:  getcwd();
来源：http://nnm.redwolf501.top

JS:   process.cwd()
来源：http://xxc.xingfuxueyuan.xyz

TS:   process.cwd()
来源：http://mei.ivvv.top

Java: Path.of("").toAbsolutePath()
来源：http://byi.0kj1m.cn

Go:   os.Getwd()
来源：http://rqe.daria6918.cn

Ruby: Dir.pwd
来源：http://ljl.xuetiantiany.cn

C#:   Directory.GetCurrentDirectory()
来源：http://eyk.yangfankeji.com

[M05] 设置退出码
来源：http://jxa.zdqjudy.top

Py:   sys.exit(1)
来源：http://cjf.jinyuanbaomall.cn

PHP:  exit(1);
来源：http://jqg.tianlin.xyz

JS:   process.exit(1)
来源：http://pis.cdnleiting.top

TS:   process.exit(1)
来源：http://oqp.daria6918.cn

Java: System.exit(1)
来源：http://fyg.hesvh.cn

Go:   os.Exit(1)
来源：http://kua.dianchejie.cn

Ruby: exit 1
来源：http://dsl.yueranfly.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://xak.ppjwa.cn

[M06] 向标准错误输出
来源：http://gjh.yueranfly.top

Py:   print("err", file=sys.stderr)
来源：http://xcx.hesvh.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://sys.yfazqb.com

JS:   console.error("err")
来源：http://oij.cdnleiting.top

TS:   console.error("err")
来源：http://mio.hnqzz.top

Java: System.err.println("err")
来源：http://agw.hammf.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wez.cqqwz.cn

Ruby: warn "err"
来源：http://qlh.zdqjudy.top

C#:   Console.Error.WriteLine("err")
来源：http://gzk.aizwys.cn

[M07] 判断是否为主入口
来源：http://kbw.gotoacloud.top

Py:   if __name__ == "__main__":
来源：http://pjn.feifeiyinyue.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://lbs.yueranfly.top

JS:   require.main === module
来源：http://nab.sufxvd.cn

TS:   require.main === module
来源：http://csh.cashguo.top

Java: public static void main(String[] args)
来源：http://lxc.yfazqb.com

Go:   func main()
来源：http://bzx.zhoulong.xyz

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wcf.xziqi.cn

C#:   static void Main(string[] args)
来源：http://cla.dashuyun.cn

[M08] 获取系统与运行时信息
来源：http://fva.havefunace.top

Py:   platform.system();  platform.python_version()
来源：http://dst.epnwcf.com

PHP:  PHP_OS;  phpversion();
来源：http://qzs.svipenyu.cn

JS:   process.platform;  process.version
来源：http://vsj.gogol.net.cn

TS:   process.platform;  process.version
来源：http://uci.gaohongyu789.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://juy.chenzaomai.com

Go:   runtime.GOOS;  runtime.Version()
来源：http://che.sjlbkw.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mjz.0kj1m.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://bxp.tarul.cn

================================================================================
来源：http://kik.chenzaomai.com

N. 数据结构与算法
来源：http://dtm.yj20258.top

================================================================================
来源：http://eaj.yanxiufei.cn

[N01] 二分查找（有序数组）
来源：http://fws.svipenyu.cn

Py:   bisect.bisect_left(arr, x)
来源：http://bum.ctjpmb.com

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ryr.yanxiufei.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://jkb.bbcook.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mcx.xingfuxueyuan.xyz

Java: Arrays.binarySearch(arr, x)
来源：http://ogw.xuetiantiany.cn

Go:   sort.SearchInts(arr, x)
来源：http://ked.sxryk.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://ryo.9152youxi.cn

C#:   Array.BinarySearch(arr, x)
来源：http://yvg.zhixingplan.top

[N02] 排序（工程实践用内置实现）
来源：http://suv.tanke756.top

Py:   sorted(arr);  arr.sort()
来源：http://njm.hongshengwenyu.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://jiv.hesvh.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://bps.redwolf501.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://qfd.yfazqb.com

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://gaz.pengpengdd.cyou

Go:   slices.Sort(arr)
来源：http://xcp.yonumen.top

Ruby: arr.sort
来源：http://nok.yj20258888.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://mqy.jinyuanbaomall.cn

[N03] 快速排序（分治示例）
来源：http://xqg.nwbrower.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ihe.nanxinkj.top

PHP:  // 递归实现，或用 usort
来源：http://omr.smart0.xyz

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hyb.xuanzx.com

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://jxv.zhongyouzk.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ybo.xuetiantiany.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://bwf.yanxiufei.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://yeo.cdnleiting.top

C#:   // 手写递归，或 Array.Sort
来源：http://xqh.jinqigfzy.top

[N04] 斐波那契数列
来源：http://swz.fzhhl.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://iva.mhx1999.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wah.zhongyouzk.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wev.hnqzz.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://zwa.xinyue.icu

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://tns.xuetiantiany.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://uzs.sxryk.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://muv.yueranfly.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://cwk.yj20258888.top

[N05] 最大公约数
来源：http://hni.chenlongwang.top

Py:   math.gcd(a, b)
来源：http://wur.yueranfly.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://fcw.tianlin.xyz

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://zyh.kuanghao11.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://xkd.kuanghao11.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://fpr.sxryk.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wlz.0kj1m.cn

Ruby: a.gcd(b)
来源：http://xqh.aizwys.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://umu.ywan-chungtsiang.top

[N06] 判断回文字符串
来源：http://jrm.cucudq.cn

Py:   s == s[::-1]
来源：http://ize.chenjidiqi.icu

PHP:  $s === strrev($s);
来源：http://lel.zhongyouzk.top

JS:   s === [...s].reverse().join("")
来源：http://hla.zhengqikj.top

TS:   s === [...s].reverse().join("")
来源：http://pjo.daria6918.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wnw.gaohongyu789.top

Go:   // 双指针从两端比较
来源：http://dlr.yongpay.top

Ruby: s == s.reverse
来源：http://wwd.quarkkingdee.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://jbf.quarkkingdee.top

[N07] 两数之和（返回下标）
来源：http://fio.cashguo.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ywa.zhoulong.xyz

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://pem.epnwcf.com

JS:   // 手写 Map：map.set(v, i)
来源：http://mfv.meibo888.top

TS:   // 手写 Map<string, number>
来源：http://rgj.daxiang520.top

Java: // 手写 HashMap
来源：http://zxu.sweek.top

Go:   // 手写 map[int]int
来源：http://zyy.gaohongyu789.top

Ruby: // 手写 Hash
来源：http://cwa.zdbjq.cn

C#:   // 手写 Dictionary<int, int>
来源：http://saz.yuanzhike.top

[N08] 生成全排列
来源：http://adt.zhengqikj.top

Py:   itertools.permutations(arr)
来源：http://yzx.meibo888.top

PHP:  // 手写递归交换
来源：http://inq.hnxiangtu.top

JS:   // 手写回溯递归
来源：http://skl.52xcode.cn

TS:   // 手写回溯递归
来源：http://nav.zhiwuduotai.top

Java: // 手写回溯递归
来源：http://awx.yj202588.top

Go:   // 手写回溯递归
来源：http://fbz.yj20258.top

Ruby: arr.permutation.to_a
来源：http://bqv.jyoumei.cn

C#:   // 手写回溯递归
来源：http://rmj.dianchejie.cn

[N09] 栈与队列
来源：http://kee.bjfxy.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://int.svipenyu.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://vhb.ppjwa.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://tpq.bjfxy.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://yyu.chenlongwang.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://kie.jiagoushi.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://bzm.yj202588.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://rag.fktsv.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://oun.ivvv.top

[N10] 链表节点定义
来源：http://nin.sxryk.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://zgo.ywan-chungtsiang.top

PHP:  class Node { public $v; public $next = null; }
来源：http://gqj.fzhhl.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wfx.shzxlz.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hro.wangshuangyany.cn

Java: class Node { int v; Node next; }
来源：http://epq.fanxiaobao.xyz

Go:   type Node struct { V int; Next *Node }
来源：http://fph.316326.xyz

Ruby: Node = Struct.new(:v, :next)
来源：http://vgl.birdmap.top

C#:   class Node { public int V; public Node? Next; }
来源：http://ltj.ybcxt.top

[N11] 二叉树中序遍历
来源：http://jtb.yuanzhike.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://pfp.zhengqikj.top

PHP:  // 手写递归函数
来源：http://yzf.hesvh.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://brc.hywenlv.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://fsb.gzhubu.top

Java: // 手写递归
来源：http://cbk.zhongyouzk.top


<!-- 参考信息 -->