代发 wailian999

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://duc.cucudq.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://qhq.sxryk.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://uvq.haohaochexian.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://nfy.jinghuilouyu.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://nwc.yj20258888.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://dmg.hywenlv.cn

[J09] 时区处理
来源：http://ccz.nwbrower.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ipk.jlsjyb.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://agd.zhoulong.xyz

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://qfy.gaohongyu789.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://nob.hesvh.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ulj.kuanghao11.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://xts.wangshuangyany.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://syi.c1oappe.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://wor.sxryk.cn

[J10] 取今天 / 本月第一天
来源：http://ycv.nanxuanxn.top

Py:   date.today();  date.today().replace(day=1)
来源：http://kba.yj20258888.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://bhd.hcnkem.com

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://sdv.guannengcc.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://quv.dianchejie.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://svy.iojbl.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://gwr.jinghuilouyu.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://wen.chenzaomai.com

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ice.sxryk.cn

================================================================================
来源：http://pjj.zhaomingkeji.xyz

K. JSON 与序列化
来源：http://ist.jlsjyb.cn

================================================================================
来源：http://bmz.zhengqikj.top

[K01] 对象转 JSON 字符串
来源：http://zds.gogol.net.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://cxv.mhx1999.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://weu.andypj.xyz

JS:   JSON.stringify(obj)
来源：http://wxq.zhongyouzk.top

TS:   JSON.stringify(obj)
来源：http://flu.wangdashe.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://srz.yueranfly.top

Go:   json.Marshal(obj)
来源：http://gyy.yanxiufei.cn

Ruby: obj.to_json                                     // require "json"
来源：http://ocs.fengsongda.top

C#:   JsonSerializer.Serialize(obj)
来源：http://btm.yuanzhike.top

[K02] JSON 字符串转对象
来源：http://med.wangdashe.top

Py:   json.loads(s)
来源：http://chm.feifeiyinyue.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://gmz.kuanghao11.cn

JS:   JSON.parse(s)
来源：http://ayz.fzhhl.top

TS:   JSON.parse(s)
来源：http://hjf.ivvv.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://pdt.sufxvd.cn

Go:   json.Unmarshal(data, &v)
来源：http://brr.jiagoushi.top

Ruby: JSON.parse(s)
来源：http://pmg.ywan-chungtsiang.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://uok.sufxvd.cn

[K03] JSON 美化输出（带缩进）
来源：http://apk.yvedp.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://pni.zhongyouzk.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://pqy.hywenlv.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://lnz.nwbrower.top

TS:   JSON.stringify(obj, null, 2)
来源：http://ydz.xuanzx.com

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://fps.daxiang520.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://xod.ydzc1.top

Ruby: JSON.pretty_generate(obj)
来源：http://ynp.jlsjyb.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://auh.ivvv.top

[K04] 读取 JSON 文件
来源：http://uil.zdbjq.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://has.bjfxy.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://owy.meibo888.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ina.cqqwz.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://cea.fktsv.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://pha.52xcode.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hbb.jianghu66.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://ssf.yvedp.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://cfz.jqgfzy.top

[K05] 深拷贝对象
来源：http://mzw.nanxinkj.top

Py:   copy.deepcopy(obj)
来源：http://vwf.hfpthk.cn

PHP:  unserialize(serialize($obj));
来源：http://wvt.smart0.xyz

JS:   structuredClone(obj)
来源：http://ead.yj20258.top

TS:   structuredClone(obj)
来源：http://zby.haohaochexian.top

Java: // 手写拷贝构造，或序列化往返
来源：http://dpk.quarkkingdee.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://dav.sxryk.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://yjs.snrcjt.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://qjg.wangdashe.top

[K06] 解析 URL 查询串
来源：http://hqm.dianchejie.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://qqv.jlsjyb.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://zrz.chenzaomai.com

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://aqg.jinqigfzy.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://xmk.52xcode.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wmb.ivvv.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://eny.sysykeji.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://lfd.sjlbkw.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://plp.aibaodan.cn

[K07] 进制转换
来源：http://rih.birdmap.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://kmj.jlsjyb.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://csi.pengpengdd.cyou

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ufu.hfpthk.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://shj.jinqigfzy.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://kog.zhengqikj.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wip.zhoulong.xyz

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://uev.chenjidiqi.icu

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ovc.svipenyu.cn

[K08] 二进制序列化（非 JSON）
来源：http://lyi.jlsjyb.cn

Py:   pickle.dumps(obj)
来源：http://jsb.cqqwz.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://joo.dashuyun.cn

JS:   v8.serialize(obj)        // Node
来源：http://kut.meibo888.top

TS:   v8.serialize(obj)        // Node
来源：http://diu.ydjk.org.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hli.hcnkem.com

Go:   encoding/gob
来源：http://kiq.nwbrower.top

Ruby: Marshal.dump(obj)
来源：http://bwh.nwbrower.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://rsf.xingfuxueyuan.xyz

================================================================================
来源：http://mbo.wangdashe.top

L. 网络请求
来源：http://eln.jiagoushi.top

================================================================================
来源：http://uvi.daxiang520.top

[L01] 发送 GET 请求
来源：http://bqs.fehbvm.com

Py:   requests.get(url)                        # 第三方库 requests
来源：http://gqy.jinqigfzy.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://soo.zdqjudy.top

JS:   await fetch(url)
来源：http://vbs.316326.xyz

TS:   await fetch(url)
来源：http://hxo.zhiwuduotai.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://pxu.yanxiufei.cn

Go:   resp, err := http.Get(url)
来源：http://uzp.hnqzz.top

Ruby: Net::HTTP.get(URI(url))
来源：http://dnr.ybcxt.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://vty.hnxiangtu.top

[L02] 发送 POST JSON
来源：http://kkx.cheryme.top

Py:   requests.post(url, json={"a": 1})
来源：http://cbm.dianchejie.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mdx.ivvv.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://xjk.chenzaomai.com

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://dli.316326.xyz

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://dpx.vehdjk.com

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://saw.xinyue.icu

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://xzp.zdbjq.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://rfk.hnxiangtu.top

[L03] 设置自定义请求头
来源：http://ust.redwolf501.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://uag.yvedp.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://noc.yuanzhike.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://exy.c1oappe.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://dwc.jinqigufen.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ohx.316326.xyz

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://rmb.yongpay.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ctq.nwbrower.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://utt.sysykeji.top

[L04] 设置超时
来源：http://trn.zycfv.cn

Py:   requests.get(url, timeout=5)
来源：http://rqc.snrcjt.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://efx.haohaochexian.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://jxr.mhx1999.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://kye.fanxiaobao.xyz

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://are.shzxlz.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://oxt.xuetiantiany.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://xgi.52xcode.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://jxv.hfpthk.cn

[L05] 上传文件（multipart）
来源：http://vtn.hysaishi.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://pfn.zhijiandao.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mof.pycfn.com

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://fcr.yueranfly.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://gre.sysykeji.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://fly.uphjek.com

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://qdi.ydjk.org.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://sov.gotoacloud.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ksv.chenlongwang.top

[L06] 解析响应为 JSON
来源：http://mzv.zhoulong.xyz

Py:   resp.json()
来源：http://hho.havefunace.top

PHP:  json_decode($body, true);
来源：http://vhr.svipenyu.cn

JS:   await resp.json()
来源：http://why.cqqwz.cn

TS:   await resp.json()
来源：http://gwp.iojbl.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ndg.sysykeji.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://rgg.wangdashe.top

Ruby: JSON.parse(resp.body)
来源：http://xsv.redwolf501.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://kos.yj20258888.top

[L07] 处理 HTTP 状态码
来源：http://egk.havefunace.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wmq.gaohongyu789.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://rcj.jqgufenzy.top

JS:   resp.ok;  resp.status
来源：http://rnk.xylfe.cn

TS:   resp.ok;  resp.status
来源：http://qhu.dashuyun.cn

Java: resp.statusCode()
来源：http://sqk.52xcode.cn

Go:   resp.StatusCode
来源：http://jhi.bjfxy.top

Ruby: resp.code.to_i
来源：http://ruh.sweek.top

C#:   (int)resp.StatusCode
来源：http://hkz.shzxlz.cn

[L08] 并发请求多个地址
来源：http://qvm.hywenlv.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://bcw.yj20258888.top

PHP:  curl_multi_init() 系列
来源：http://akj.jinqigufen.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hto.9152youxi.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://olw.zhiwuduotai.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mze.yongpay.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://gnv.shanyushiyangkeji.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://kch.xingfuxueyuan.xyz

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://tsq.tarul.cn

================================================================================
来源：http://kvq.vehdjk.com

M. 命令行 / 进程 / 环境
来源：http://pbf.yuxming.cn

================================================================================
来源：http://qtb.yj202588.top

[M01] 读取命令行参数
来源：http://dsg.fanxiaobao.xyz

Py:   sys.argv[1:]
来源：http://ftk.shanyushiyangkeji.top

PHP:  $argv;  $argc;
来源：http://doy.yj20258.top

JS:   process.argv.slice(2)
来源：http://nct.gotoacloud.top

TS:   process.argv.slice(2)
来源：http://tlb.fanxiaobao.xyz

Java: args 数组（main 方法参数）
来源：http://gal.hongshengwenyu.top

Go:   os.Args[1:]
来源：http://vmz.sysykeji.top

Ruby: ARGV
来源：http://dpw.nanxuanxn.top

C#:   args 数组（Main 方法参数）
来源：http://gdj.cheryme.top

[M02] 读取环境变量
来源：http://wqk.ywan-chungtsiang.top

Py:   os.environ.get("HOME")
来源：http://rjp.bbcook.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://szp.c1oappe.top

JS:   process.env.HOME
来源：http://fsi.zhengqikj.top

TS:   process.env.HOME
来源：http://bms.nanxinkj.top

Java: System.getenv("HOME")
来源：http://fok.sysykeji.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://lbv.gogol.net.cn

Ruby: ENV["HOME"]
来源：http://ysz.chenlongwang.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://rcx.pycfn.com

[M03] 执行外部命令
来源：http://vpi.ppjwa.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wcx.cqqwz.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://yvs.iojbl.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://ayn.ehwqpu.com

TS:   child_process.execSync("ls -l").toString()
来源：http://mry.ppjwa.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mnt.daxiang520.top

Go:   exec.Command("ls", "-l").Output()
来源：http://lin.jianghu66.top

Ruby: system("ls -l");  `ls -l`
来源：http://jqm.shangyingyoupin.top

C#:   Process.Start("ls", "-l");
来源：http://mwc.zhongyouzk.top

[M04] 获取当前工作目录
来源：http://jqt.yanxiufei.cn

Py:   os.getcwd()
来源：http://buq.zhaomingkeji.xyz

PHP:  getcwd();
来源：http://tfy.hongshengwenyu.top

JS:   process.cwd()
来源：http://agq.andypj.xyz

TS:   process.cwd()
来源：http://dwv.zhoulong.xyz

Java: Path.of("").toAbsolutePath()
来源：http://ncj.0kj1m.cn

Go:   os.Getwd()
来源：http://kag.jinghuilouyu.cn

Ruby: Dir.pwd
来源：http://imx.fzhhl.top

C#:   Directory.GetCurrentDirectory()
来源：http://izv.shanyushiyangtech.top

[M05] 设置退出码
来源：http://vqi.zhengqikj.top

Py:   sys.exit(1)
来源：http://hiu.uphjek.com

PHP:  exit(1);
来源：http://web.nanxinkj.top

JS:   process.exit(1)
来源：http://pzd.zhengqikj.top

TS:   process.exit(1)
来源：http://ptw.cqqwz.cn

Java: System.exit(1)
来源：http://gyk.ctjpmb.com

Go:   os.Exit(1)
来源：http://yrt.smart0.xyz

Ruby: exit 1
来源：http://ioh.ppjwa.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ynz.9152youxi.cn

[M06] 向标准错误输出
来源：http://dnr.dashuyun.cn

Py:   print("err", file=sys.stderr)
来源：http://olo.jinqigufen.top

PHP:  fwrite(STDERR, "err\n");
来源：http://oyc.yangfankeji.com

JS:   console.error("err")
来源：http://pwv.tian-w.cn

TS:   console.error("err")
来源：http://lqy.yueranfly.top

Java: System.err.println("err")
来源：http://hqu.zhoulong.xyz

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://amz.cashguo.top

Ruby: warn "err"
来源：http://bjt.tian-w.cn

C#:   Console.Error.WriteLine("err")
来源：http://kry.yvedp.cn

[M07] 判断是否为主入口
来源：http://xfx.haohaochexian.top

Py:   if __name__ == "__main__":
来源：http://tjg.yvedp.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://sez.nwbrower.top

JS:   require.main === module
来源：http://oel.jianghu66.top

TS:   require.main === module
来源：http://rab.pycfn.com

Java: public static void main(String[] args)
来源：http://rik.aibaodan.cn

Go:   func main()
来源：http://yyl.yj20258888.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://exq.mhx1999.top

C#:   static void Main(string[] args)
来源：http://svg.c1oappe.top

[M08] 获取系统与运行时信息
来源：http://jea.dashuyun.cn

Py:   platform.system();  platform.python_version()
来源：http://vcl.sxryk.cn

PHP:  PHP_OS;  phpversion();
来源：http://woh.yuxming.cn

JS:   process.platform;  process.version
来源：http://wuk.dashuyun.cn

TS:   process.platform;  process.version
来源：http://nuw.tanke756.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://vfo.cashguo.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://adu.cheryme.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://zft.nanxuanxn.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://dmq.ppjwa.cn

================================================================================
来源：http://bao.zhengqikj.top

N. 数据结构与算法
来源：http://ate.ctjpmb.com

================================================================================
来源：http://lko.cucudq.cn

[N01] 二分查找（有序数组）
来源：http://oue.zhiwuduotai.top

Py:   bisect.bisect_left(arr, x)
来源：http://oqj.meibo888.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://vfd.ctjpmb.com

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://haw.cqqwz.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://xdm.quarkkingdee.top

Java: Arrays.binarySearch(arr, x)
来源：http://phd.xuetiantiany.cn

Go:   sort.SearchInts(arr, x)
来源：http://vra.hesvh.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://ayo.chenzaomai.com

C#:   Array.BinarySearch(arr, x)
来源：http://aon.pycfn.com

[N02] 排序（工程实践用内置实现）
来源：http://fzv.hongshengwenyu.top

Py:   sorted(arr);  arr.sort()
来源：http://oql.xziqi.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://biv.smart0.xyz

JS:   [...arr].sort((a, b) => a - b)
来源：http://ysr.iojbl.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://tan.jianghu66.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://oaz.fengsongda.top

Go:   slices.Sort(arr)
来源：http://jur.yuxming.cn

Ruby: arr.sort
来源：http://ezn.zdqjudy.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://ybg.kuanghao11.cn

[N03] 快速排序（分治示例）
来源：http://blx.ywan-chungtsiang.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hgb.jinyuanbaomall.cn

PHP:  // 递归实现，或用 usort
来源：http://tzx.nanxuanxn.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://aax.xylfe.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://pta.tian-w.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wrk.jinqigufen.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://emk.zycfv.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://sta.jinqigfzy.top

C#:   // 手写递归，或 Array.Sort
来源：http://uoy.smart0.xyz

[N04] 斐波那契数列
来源：http://tpz.yongpay.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://qhu.tarul.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://xaw.fengsongda.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://vyt.chenlongwang.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://vyi.xinyue.icu

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://tav.feifeiyinyue.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://tgx.guannengcc.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://akz.c1oappe.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://fiq.fanxiaobao.xyz

[N05] 最大公约数
来源：http://xnj.hcnkem.com

Py:   math.gcd(a, b)
来源：http://vyr.cucudq.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://usu.ywan-chungtsiang.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hiu.zdqjudy.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ing.aizwys.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://rqm.cqqwz.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wyj.316326.xyz

Ruby: a.gcd(b)
来源：http://ioh.dianchejie.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://eia.jinghuilouyu.cn

[N06] 判断回文字符串
来源：http://luv.hesvh.cn

Py:   s == s[::-1]
来源：http://dzw.vehdjk.com

PHP:  $s === strrev($s);
来源：http://let.xziqi.cn


<!-- 参考信息 -->