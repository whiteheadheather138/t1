代发 wailian999

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://fys.hongshengwenyu.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://isy.xuanzx.com

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://zwh.cucudq.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://rag.svipenyu.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ydv.fzhhl.top

Ruby: Time.now.getlocal("+08:00")
来源：http://hty.tianlin.xyz

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://njo.pengpengdd.cyou

[J10] 取今天 / 本月第一天
来源：http://ybp.meibo888.top

Py:   date.today();  date.today().replace(day=1)
来源：http://agw.zdqjudy.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://mez.aibaodan.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://afc.hammf.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://cou.feifeiyinyue.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://wjd.jinyuanbaomall.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://dhh.nwbrower.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://bxc.hongshengwenyu.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://mkn.daria6918.cn

================================================================================
来源：http://dka.daria6918.cn

K. JSON 与序列化
来源：http://vyi.chenzaomai.com

================================================================================
来源：http://mry.ybcxt.top

[K01] 对象转 JSON 字符串
来源：http://pao.gaohongyu789.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://dbi.smart0.xyz

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ghp.jinyuanbaomall.cn

JS:   JSON.stringify(obj)
来源：http://qlg.sufxvd.cn

TS:   JSON.stringify(obj)
来源：http://uyz.zhengqikj.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://cwj.aizwys.cn

Go:   json.Marshal(obj)
来源：http://ogt.nanxuanxn.top

Ruby: obj.to_json                                     // require "json"
来源：http://shd.gogol.net.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://odx.shanyushiyangtech.top

[K02] JSON 字符串转对象
来源：http://qni.shanyushiyangtech.top

Py:   json.loads(s)
来源：http://hxg.daria6918.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://pbb.daria6918.cn

JS:   JSON.parse(s)
来源：http://jyj.xylfe.cn

TS:   JSON.parse(s)
来源：http://rzc.fzhhl.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://rzm.zhaomingkeji.xyz

Go:   json.Unmarshal(data, &v)
来源：http://nys.svipenyu.cn

Ruby: JSON.parse(s)
来源：http://yfw.yueranfly.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://fbm.smart0.xyz

[K03] JSON 美化输出（带缩进）
来源：http://zxr.nanxuanxn.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://qfg.jlsjyb.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://bif.jiagoushi.top

JS:   JSON.stringify(obj, null, 2)
来源：http://pwu.sxryk.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://mjb.gaohongyu789.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://vwy.xinyue.icu

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://jol.cucudq.cn

Ruby: JSON.pretty_generate(obj)
来源：http://abn.shanyushiyangkeji.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mza.zhiwuduotai.top

[K04] 读取 JSON 文件
来源：http://nyg.fktsv.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://dgn.zhongyouzk.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://gol.yj20258.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://kfs.meibo888.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ngw.zhongyouzk.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://cit.jiagoushi.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://oga.quarkkingdee.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://jof.aizwys.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://flf.gotoacloud.top

[K05] 深拷贝对象
来源：http://mqs.zycfv.cn

Py:   copy.deepcopy(obj)
来源：http://qwr.xuanzx.com

PHP:  unserialize(serialize($obj));
来源：http://hhl.sweek.top

JS:   structuredClone(obj)
来源：http://xur.zhiwuduotai.top

TS:   structuredClone(obj)
来源：http://hcm.smart0.xyz

Java: // 手写拷贝构造，或序列化往返
来源：http://gjw.feifeiyinyue.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://zmq.sxryk.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://pfb.vehdjk.com

C#:   // 序列化往返，或自定义 Clone
来源：http://fnh.tianlin.xyz

[K06] 解析 URL 查询串
来源：http://umv.sxryk.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://mwj.daria6918.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://nvl.ivvv.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://lho.chenlongwang.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ctu.xylfe.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://imk.jiagoushi.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://pry.zhijiandao.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://jbk.cqqwz.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://qps.gogol.net.cn

[K07] 进制转换
来源：http://axq.snrcjt.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://bhc.cashguo.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://owk.zdqjudy.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://abo.mhx1999.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://sdp.hywenlv.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://tsr.wangshuangyany.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mbl.wangshuangyany.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://can.chenlongwang.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://xlx.c1oappe.top

[K08] 二进制序列化（非 JSON）
来源：http://xwk.zycfv.cn

Py:   pickle.dumps(obj)
来源：http://uip.meibo888.top

PHP:  serialize($obj);  unserialize($s);
来源：http://sfs.ywan-chungtsiang.top

JS:   v8.serialize(obj)        // Node
来源：http://vlr.nwbrower.top

TS:   v8.serialize(obj)        // Node
来源：http://lli.mhx1999.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://auz.ctjpmb.com

Go:   encoding/gob
来源：http://szn.andypj.xyz

Ruby: Marshal.dump(obj)
来源：http://mhr.epnwcf.com

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://zjg.nwbrower.top

================================================================================
来源：http://zud.aizwys.cn

L. 网络请求
来源：http://qnz.c1oappe.top

================================================================================
来源：http://cbm.52xcode.cn

[L01] 发送 GET 请求
来源：http://gwe.sysykeji.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://stf.dianchejie.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://nuf.nwbrower.top

JS:   await fetch(url)
来源：http://ezf.chenlongwang.top

TS:   await fetch(url)
来源：http://whs.chenlongwang.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://afj.gzhubu.top

Go:   resp, err := http.Get(url)
来源：http://nvt.birdmap.top

Ruby: Net::HTTP.get(URI(url))
来源：http://yqk.aibaodan.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://lzy.wangshuangyany.cn

[L02] 发送 POST JSON
来源：http://nwz.tarul.cn

Py:   requests.post(url, json={"a": 1})
来源：http://bau.aibaodan.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hcb.yonumen.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://kwq.nwbrower.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wls.jqgfzy.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mgg.daxiang520.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://iii.c1oappe.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ngu.hongshengwenyu.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://krl.tian-w.cn

[L03] 设置自定义请求头
来源：http://pmd.yangfankeji.com

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://kwt.vqdsnc.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://bxa.ydjk.org.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://sxm.zhongyouzk.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://nxj.hysaishi.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ylh.zhongyouzk.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mow.zhongyouzk.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://jcw.zhengqikj.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ban.vehdjk.com

[L04] 设置超时
来源：http://ven.yonumen.top

Py:   requests.get(url, timeout=5)
来源：http://ens.yuxming.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ond.zhixingplan.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://dce.nanxuanxn.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://kdw.fzhhl.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://svb.hysaishi.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://cke.yongpay.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://loj.gaohongyu789.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://rli.xuetiantiany.cn

[L05] 上传文件（multipart）
来源：http://tuo.xylfe.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://zyw.0kj1m.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://pfh.cdnleiting.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://cbr.jiagoushi.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://gmc.havefunace.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://qou.cucudq.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://gxb.shuidangran.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://zfo.jianghu66.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ahd.jianghu66.top

[L06] 解析响应为 JSON
来源：http://khp.zdqjudy.top

Py:   resp.json()
来源：http://qhm.fzhhl.top

PHP:  json_decode($body, true);
来源：http://trz.zycfv.cn

JS:   await resp.json()
来源：http://oag.jiagoushi.top

TS:   await resp.json()
来源：http://vkt.quarkkingdee.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mbt.daxiang520.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://pxq.ybcxt.top

Ruby: JSON.parse(resp.body)
来源：http://ztm.guannengcc.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://aqp.yj20258.top

[L07] 处理 HTTP 状态码
来源：http://okh.uphjek.com

Py:   resp.status_code;  resp.raise_for_status()
来源：http://yrc.tianlin.xyz

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://nev.fzhhl.top

JS:   resp.ok;  resp.status
来源：http://llm.daxiang520.top

TS:   resp.ok;  resp.status
来源：http://jry.gotoacloud.top

Java: resp.statusCode()
来源：http://byy.bbcook.cn

Go:   resp.StatusCode
来源：http://xwc.dianchejie.cn

Ruby: resp.code.to_i
来源：http://xbf.tarul.cn

C#:   (int)resp.StatusCode
来源：http://dbh.shzxlz.cn

[L08] 并发请求多个地址
来源：http://zre.kuanghao11.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://xnd.birdmap.top

PHP:  curl_multi_init() 系列
来源：http://nel.tianlin.xyz

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://tbe.cheryme.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ort.kuanghao11.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wnv.gaohongyu789.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://jcr.c1oappe.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://kww.dashuyun.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ays.ydjk.org.cn

================================================================================
来源：http://iny.haohaochexian.top

M. 命令行 / 进程 / 环境
来源：http://ktz.sysykeji.top

================================================================================
来源：http://ryb.zhongyouzk.top

[M01] 读取命令行参数
来源：http://qik.vqdsnc.cn

Py:   sys.argv[1:]
来源：http://jwl.guowangkeji.top

PHP:  $argv;  $argc;
来源：http://wuq.zhiwuduotai.top

JS:   process.argv.slice(2)
来源：http://nko.shanyushiyangkeji.top

TS:   process.argv.slice(2)
来源：http://fan.sysykeji.top

Java: args 数组（main 方法参数）
来源：http://ees.guowangkeji.top

Go:   os.Args[1:]
来源：http://lpe.xuanzx.com

Ruby: ARGV
来源：http://ouq.jinqigufen.top

C#:   args 数组（Main 方法参数）
来源：http://uar.aibaodan.cn

[M02] 读取环境变量
来源：http://kai.jinghuilouyu.cn

Py:   os.environ.get("HOME")
来源：http://hnk.cucudq.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://bzl.aibaodan.cn

JS:   process.env.HOME
来源：http://qcw.guowangkeji.top

TS:   process.env.HOME
来源：http://xdq.gaohongyu789.top

Java: System.getenv("HOME")
来源：http://mmh.vqdsnc.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hln.kuanghao11.cn

Ruby: ENV["HOME"]
来源：http://oea.ydzc1.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://czb.shanyushiyangkeji.top

[M03] 执行外部命令
来源：http://vcc.daxiang520.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://tfu.hfpthk.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://cvt.xziqi.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://aul.cqqwz.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://zas.zhijiandao.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wii.smart0.xyz

Go:   exec.Command("ls", "-l").Output()
来源：http://rfk.gotoacloud.top

Ruby: system("ls -l");  `ls -l`
来源：http://fgl.smart0.xyz

C#:   Process.Start("ls", "-l");
来源：http://mrl.c1oappe.top

[M04] 获取当前工作目录
来源：http://ibb.sweek.top

Py:   os.getcwd()
来源：http://dul.bbcook.cn

PHP:  getcwd();
来源：http://vxf.hfpthk.cn

JS:   process.cwd()
来源：http://itl.tanke756.top

TS:   process.cwd()
来源：http://vls.cheryme.top

Java: Path.of("").toAbsolutePath()
来源：http://tlt.hfpthk.cn

Go:   os.Getwd()
来源：http://oyu.ydjk.org.cn

Ruby: Dir.pwd
来源：http://dqv.hfpthk.cn

C#:   Directory.GetCurrentDirectory()
来源：http://ufk.sufxvd.cn

[M05] 设置退出码
来源：http://ukx.fzhhl.top

Py:   sys.exit(1)
来源：http://zbw.bjfxy.top

PHP:  exit(1);
来源：http://ofo.andypj.xyz

JS:   process.exit(1)
来源：http://ifa.yj20258888.top

TS:   process.exit(1)
来源：http://rzg.gogol.net.cn

Java: System.exit(1)
来源：http://twr.zhongyouzk.top

Go:   os.Exit(1)
来源：http://eiy.shzxlz.cn

Ruby: exit 1
来源：http://ehh.havefunace.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://bbf.nanxinkj.top

[M06] 向标准错误输出
来源：http://ccg.yuxming.cn

Py:   print("err", file=sys.stderr)
来源：http://jnm.chenlongwang.top

PHP:  fwrite(STDERR, "err\n");
来源：http://pko.pengpengdd.cyou

JS:   console.error("err")
来源：http://fui.gzhubu.top

TS:   console.error("err")
来源：http://kfn.fzhhl.top

Java: System.err.println("err")
来源：http://uxi.cheryme.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ynj.guowangkeji.top

Ruby: warn "err"
来源：http://ldu.guannengcc.top

C#:   Console.Error.WriteLine("err")
来源：http://kfr.shanyushiyangtech.top

[M07] 判断是否为主入口
来源：http://ocb.gogol.net.cn

Py:   if __name__ == "__main__":
来源：http://ced.hcnkem.com

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://uzl.9152youxi.cn

JS:   require.main === module
来源：http://fjv.gotoacloud.top

TS:   require.main === module
来源：http://dxv.andypj.xyz

Java: public static void main(String[] args)
来源：http://zmd.jinqigfzy.top

Go:   func main()
来源：http://zeh.dashuyun.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ghl.pengpengdd.cyou

C#:   static void Main(string[] args)
来源：http://gpb.haohaochexian.top

[M08] 获取系统与运行时信息
来源：http://eub.birdmap.top

Py:   platform.system();  platform.python_version()
来源：http://kae.jinghuilouyu.cn

PHP:  PHP_OS;  phpversion();
来源：http://dpo.ehwqpu.com

JS:   process.platform;  process.version
来源：http://rmf.jinqigufen.top

TS:   process.platform;  process.version
来源：http://geo.chenzaomai.com

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://plg.epnwcf.com

Go:   runtime.GOOS;  runtime.Version()
来源：http://qjr.gaohongyu789.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://rya.yueranfly.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://jkh.jinyuanbaomall.cn

================================================================================
来源：http://lfe.zdqjudy.top

N. 数据结构与算法
来源：http://ygn.chenzaomai.com

================================================================================
来源：http://etf.iojbl.cn

[N01] 二分查找（有序数组）
来源：http://dzt.zhijiandao.cn

Py:   bisect.bisect_left(arr, x)
来源：http://zue.yanxiufei.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://fhj.kuanghao11.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://rpd.sxryk.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wbv.jqgfzy.top

Java: Arrays.binarySearch(arr, x)
来源：http://pzd.zdqjudy.top

Go:   sort.SearchInts(arr, x)
来源：http://tfo.birdmap.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://kxe.xuetiantiany.cn

C#:   Array.BinarySearch(arr, x)
来源：http://vgf.pycfn.com

[N02] 排序（工程实践用内置实现）
来源：http://mnv.hnxiangtu.top

Py:   sorted(arr);  arr.sort()
来源：http://nuy.tianlin.xyz

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://zao.fzhhl.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://upd.nanxinkj.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://dou.yvedp.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://cza.kuanghao11.cn

Go:   slices.Sort(arr)
来源：http://aiv.tianlin.xyz

Ruby: arr.sort
来源：http://dtt.xylfe.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://ise.feifeiyinyue.top

[N03] 快速排序（分治示例）
来源：http://adr.daxiang520.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://txq.chenlongwang.top

PHP:  // 递归实现，或用 usort
来源：http://kvt.yonumen.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://iba.ivvv.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://eam.haohaochexian.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ezg.ywan-chungtsiang.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://dej.vqdsnc.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ogx.tianlin.xyz

C#:   // 手写递归，或 Array.Sort
来源：http://gyw.zhaomingkeji.xyz

[N04] 斐波那契数列
来源：http://wdv.guowangkeji.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://pam.shanyushiyangtech.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://xvr.smart0.xyz

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://cbk.meibo888.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://yrg.sysykeji.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://jel.jiagoushi.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://fwu.haohaochexian.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://dez.zdqjudy.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://aqo.dianchejie.cn

[N05] 最大公约数
来源：http://vcb.zhengqikj.top

Py:   math.gcd(a, b)
来源：http://kjy.ydjk.org.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://xox.zdbjq.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://oyx.yvedp.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mho.shanyushiyangkeji.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://csv.wangdashe.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mqi.yj20258.top

Ruby: a.gcd(b)
来源：http://pzi.fanxiaobao.xyz

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://oah.mhx1999.top

[N06] 判断回文字符串
来源：http://cmm.bbcook.cn

Py:   s == s[::-1]
来源：http://pve.hnxiangtu.top

PHP:  $s === strrev($s);
来源：http://god.birdmap.top

JS:   s === [...s].reverse().join("")
来源：http://pnl.tianlin.xyz

TS:   s === [...s].reverse().join("")
来源：http://sjl.jyoumei.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://jvc.havefunace.top

Go:   // 双指针从两端比较
来源：http://nwr.ctjpmb.com

Ruby: s == s.reverse
来源：http://chx.yvedp.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://grj.zhengqikj.top

[N07] 两数之和（返回下标）
来源：http://fnk.zhoulong.xyz

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hue.sufxvd.cn


<!-- 参考信息 -->