代发 wailian999

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://itk.fanxiaobao.xyz

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://uzh.hammf.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://zms.yuxming.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://oxt.yj202588.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://dyu.jyoumei.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://pmv.jyoumei.cn

[J09] 时区处理
来源：http://npz.yfazqb.com

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://aae.hesvh.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://wcp.haohaochexian.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://bhv.sweek.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://grg.hesvh.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://vgs.hammf.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://iry.shuidangran.top

Ruby: Time.now.getlocal("+08:00")
来源：http://fkk.cdnleiting.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://utv.ehwqpu.com

[J10] 取今天 / 本月第一天
来源：http://xtk.hnqzz.top

Py:   date.today();  date.today().replace(day=1)
来源：http://zbk.yongpay.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://lgs.hysaishi.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://vuw.ydjk.org.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://uqy.cdnleiting.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://vfa.jinqigufen.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://lmm.chenlongwang.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://fxw.ivvv.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://gbs.sxryk.cn

================================================================================
来源：http://ujr.feifeiyinyue.top

K. JSON 与序列化
来源：http://nkw.yueranfly.top

================================================================================
来源：http://nqb.xylfe.cn

[K01] 对象转 JSON 字符串
来源：http://ozt.zhiwuduotai.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ryy.aizwys.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hjh.ybcxt.top

JS:   JSON.stringify(obj)
来源：http://prh.fktsv.cn

TS:   JSON.stringify(obj)
来源：http://yba.jiagoushi.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ifu.c1oappe.top

Go:   json.Marshal(obj)
来源：http://djj.shuidangran.top

Ruby: obj.to_json                                     // require "json"
来源：http://jbm.yonumen.top

C#:   JsonSerializer.Serialize(obj)
来源：http://sqr.redwolf501.top

[K02] JSON 字符串转对象
来源：http://dkm.smart0.xyz

Py:   json.loads(s)
来源：http://xmt.0kj1m.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://rxq.9152youxi.cn

JS:   JSON.parse(s)
来源：http://wrw.cqqwz.cn

TS:   JSON.parse(s)
来源：http://prh.shanyushiyangkeji.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://fyr.yonumen.top

Go:   json.Unmarshal(data, &v)
来源：http://kyu.meibo888.top

Ruby: JSON.parse(s)
来源：http://boa.shzxlz.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://vya.jinyuanbaomall.cn

[K03] JSON 美化输出（带缩进）
来源：http://kry.bjfxy.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://afz.sxryk.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://iml.xingfuxueyuan.xyz

JS:   JSON.stringify(obj, null, 2)
来源：http://vpt.yj20258888.top

TS:   JSON.stringify(obj, null, 2)
来源：http://nhr.9152youxi.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://mhx.chenjidiqi.icu

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ole.jinyuanbaomall.cn

Ruby: JSON.pretty_generate(obj)
来源：http://onq.ywan-chungtsiang.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://swe.chenjidiqi.icu

[K04] 读取 JSON 文件
来源：http://mke.hywenlv.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://rwg.shanyushiyangtech.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://zpc.jqgufenzy.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://nxl.jqgufenzy.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://zkr.hysaishi.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://qyr.jqgufenzy.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://qhe.yanxiufei.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://ijr.hongshengwenyu.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://cyr.tarul.cn

[K05] 深拷贝对象
来源：http://wbo.dashuyun.cn

Py:   copy.deepcopy(obj)
来源：http://kfm.xuanzx.com

PHP:  unserialize(serialize($obj));
来源：http://cwx.chenlongwang.top

JS:   structuredClone(obj)
来源：http://wif.sxryk.cn

TS:   structuredClone(obj)
来源：http://jxw.tianlin.xyz

Java: // 手写拷贝构造，或序列化往返
来源：http://qjm.316326.xyz

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://xlm.chenlongwang.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://tut.guannengcc.top

C#:   // 序列化往返，或自定义 Clone
来源：http://txn.xylfe.cn

[K06] 解析 URL 查询串
来源：http://jzo.fktsv.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://rob.ybcxt.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://qao.hongshengwenyu.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://kpq.gotoacloud.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://rfd.xuetiantiany.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://nso.bjfxy.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://dky.feifeiyinyue.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://fsx.uphjek.com

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://tds.tian-w.cn

[K07] 进制转换
来源：http://vhz.cheryme.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://lnb.dianchejie.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ekw.xingfuxueyuan.xyz

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://zla.jqgufenzy.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hoc.xuetiantiany.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://kmx.nanxuanxn.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://uig.yuanzhike.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://nnz.cqqwz.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://irl.shanyushiyangtech.top

[K08] 二进制序列化（非 JSON）
来源：http://aff.shzxlz.cn

Py:   pickle.dumps(obj)
来源：http://sqt.ydjk.org.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://cma.9152youxi.cn

JS:   v8.serialize(obj)        // Node
来源：http://gty.zhongyouzk.top

TS:   v8.serialize(obj)        // Node
来源：http://ztn.shzxlz.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://xlk.xinyue.icu

Go:   encoding/gob
来源：http://vkb.vehdjk.com

Ruby: Marshal.dump(obj)
来源：http://xsl.birdmap.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://gxi.shanyushiyangkeji.top

================================================================================
来源：http://kgt.ybcxt.top

L. 网络请求
来源：http://htt.zdbjq.cn

================================================================================
来源：http://dcj.guowangkeji.top

[L01] 发送 GET 请求
来源：http://phf.yanxiufei.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mud.xingfuxueyuan.xyz

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://swi.nanxuanxn.top

JS:   await fetch(url)
来源：http://qdp.xingfuxueyuan.xyz

TS:   await fetch(url)
来源：http://pht.fktsv.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://tlm.guowangkeji.top

Go:   resp, err := http.Get(url)
来源：http://wnr.havefunace.top

Ruby: Net::HTTP.get(URI(url))
来源：http://rvc.havefunace.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://kon.zhengqikj.top

[L02] 发送 POST JSON
来源：http://dtu.52xcode.cn

Py:   requests.post(url, json={"a": 1})
来源：http://rym.jyoumei.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ncb.uphjek.com

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://amb.zhoulong.xyz

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://vws.chenjidiqi.icu

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://meq.shangyingyoupin.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://qza.chenzaomai.com

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://lix.yuxming.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://dig.yvedp.cn

[L03] 设置自定义请求头
来源：http://oqf.gotoacloud.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://xkq.chenlongwang.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hkr.dashuyun.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://kaf.yfazqb.com

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://kuc.iojbl.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://edu.yfazqb.com

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://jvz.fehbvm.com

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://bep.zycfv.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://yvc.ywan-chungtsiang.top

[L04] 设置超时
来源：http://gco.mhx1999.top

Py:   requests.get(url, timeout=5)
来源：http://rkw.redwolf501.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://sbt.yueranfly.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://kxd.zhiwuduotai.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://gub.chenlongwang.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://pwv.yueranfly.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://crf.andypj.xyz

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mcu.52xcode.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://dvk.yangfankeji.com

[L05] 上传文件（multipart）
来源：http://iuv.fktsv.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://omw.hongshengwenyu.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://qim.sjlbkw.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://sin.sjlbkw.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mpv.jqgufenzy.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://xlk.daria6918.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ruk.fengsongda.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://eti.smart0.xyz

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://egw.wangshuangyany.cn

[L06] 解析响应为 JSON
来源：http://gnv.ctjpmb.com

Py:   resp.json()
来源：http://tah.hcnkem.com

PHP:  json_decode($body, true);
来源：http://jbo.ywan-chungtsiang.top

JS:   await resp.json()
来源：http://vfj.yj20258888.top

TS:   await resp.json()
来源：http://vig.yvedp.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wrt.xuetiantiany.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://qoz.havefunace.top

Ruby: JSON.parse(resp.body)
来源：http://xtw.yongpay.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://zwq.cucudq.cn

[L07] 处理 HTTP 状态码
来源：http://ytd.yangfankeji.com

Py:   resp.status_code;  resp.raise_for_status()
来源：http://syc.ybcxt.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://vxj.c1oappe.top

JS:   resp.ok;  resp.status
来源：http://fru.yfazqb.com

TS:   resp.ok;  resp.status
来源：http://hlf.wangshuangyany.cn

Java: resp.statusCode()
来源：http://moo.ybcxt.top

Go:   resp.StatusCode
来源：http://pcz.zhoulong.xyz

Ruby: resp.code.to_i
来源：http://ane.yuxming.cn

C#:   (int)resp.StatusCode
来源：http://tiu.zhiwuduotai.top

[L08] 并发请求多个地址
来源：http://dyv.cqqwz.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://uql.kuanghao11.cn

PHP:  curl_multi_init() 系列
来源：http://rgs.feifeiyinyue.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://crk.daria6918.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ezp.meibo888.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ynx.aizwys.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ctj.daxiang520.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://fmu.ydzc1.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://rvk.xuanzx.com

================================================================================
来源：http://wvu.birdmap.top

M. 命令行 / 进程 / 环境
来源：http://jnx.pengpengdd.cyou

================================================================================
来源：http://lqd.hnqzz.top

[M01] 读取命令行参数
来源：http://app.quarkkingdee.top

Py:   sys.argv[1:]
来源：http://gch.redwolf501.top

PHP:  $argv;  $argc;
来源：http://gkt.c1oappe.top

JS:   process.argv.slice(2)
来源：http://dvg.ydjk.org.cn

TS:   process.argv.slice(2)
来源：http://sfo.jyoumei.cn

Java: args 数组（main 方法参数）
来源：http://xsv.quarkkingdee.top

Go:   os.Args[1:]
来源：http://wfg.hysaishi.cn

Ruby: ARGV
来源：http://xfl.yanxiufei.cn

C#:   args 数组（Main 方法参数）
来源：http://net.yvedp.cn

[M02] 读取环境变量
来源：http://hfk.aibaodan.cn

Py:   os.environ.get("HOME")
来源：http://jzu.yuanzhike.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://amt.zhaomingkeji.xyz

JS:   process.env.HOME
来源：http://mfz.ctjpmb.com

TS:   process.env.HOME
来源：http://ohu.sysykeji.top

Java: System.getenv("HOME")
来源：http://bbr.andypj.xyz

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://iky.316326.xyz

Ruby: ENV["HOME"]
来源：http://luj.hongshengwenyu.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://lrx.chenzaomai.com

[M03] 执行外部命令
来源：http://fqq.uphjek.com

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://jys.pengpengdd.cyou

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://eqi.fengsongda.top

JS:   child_process.execSync("ls -l").toString()
来源：http://emk.hfpthk.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://xvf.snrcjt.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://pmz.shanyushiyangkeji.top

Go:   exec.Command("ls", "-l").Output()
来源：http://zak.hesvh.cn

Ruby: system("ls -l");  `ls -l`
来源：http://dgj.xingfuxueyuan.xyz

C#:   Process.Start("ls", "-l");
来源：http://cwu.snrcjt.cn

[M04] 获取当前工作目录
来源：http://eaq.jqgufenzy.top

Py:   os.getcwd()
来源：http://mpr.nwbrower.top

PHP:  getcwd();
来源：http://eqw.yvedp.cn

JS:   process.cwd()
来源：http://svl.vehdjk.com

TS:   process.cwd()
来源：http://zrb.bjfxy.top

Java: Path.of("").toAbsolutePath()
来源：http://mrz.yj20258888.top

Go:   os.Getwd()
来源：http://wzb.shanyushiyangtech.top

Ruby: Dir.pwd
来源：http://svn.gotoacloud.top

C#:   Directory.GetCurrentDirectory()
来源：http://uuy.yj202588.top

[M05] 设置退出码
来源：http://aco.zhaomingkeji.xyz

Py:   sys.exit(1)
来源：http://oqa.shangyingyoupin.top

PHP:  exit(1);
来源：http://kny.hnxiangtu.top

JS:   process.exit(1)
来源：http://avo.hfpthk.cn

TS:   process.exit(1)
来源：http://zzh.nwbrower.top

Java: System.exit(1)
来源：http://gpl.andypj.xyz

Go:   os.Exit(1)
来源：http://kna.aibaodan.cn

Ruby: exit 1
来源：http://bkl.ydzc1.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://pbr.xuetiantiany.cn

[M06] 向标准错误输出
来源：http://yoe.shangyingyoupin.top

Py:   print("err", file=sys.stderr)
来源：http://lmp.sysykeji.top

PHP:  fwrite(STDERR, "err\n");
来源：http://kvn.hysaishi.cn

JS:   console.error("err")
来源：http://ulx.jyoumei.cn

TS:   console.error("err")
来源：http://osd.shanyushiyangtech.top

Java: System.err.println("err")
来源：http://eku.bbcook.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://cut.zhengqikj.top

Ruby: warn "err"
来源：http://kwn.smart0.xyz

C#:   Console.Error.WriteLine("err")
来源：http://ehk.hesvh.cn

[M07] 判断是否为主入口
来源：http://wna.xuanzx.com

Py:   if __name__ == "__main__":
来源：http://wmy.sufxvd.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hbe.jinqigufen.top

JS:   require.main === module
来源：http://uiy.52xcode.cn

TS:   require.main === module
来源：http://cmu.jiagoushi.top

Java: public static void main(String[] args)
来源：http://jba.jlsjyb.cn

Go:   func main()
来源：http://nyn.xuetiantiany.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ady.tanke756.top

C#:   static void Main(string[] args)
来源：http://atg.yj20258.top

[M08] 获取系统与运行时信息
来源：http://ugy.fehbvm.com

Py:   platform.system();  platform.python_version()
来源：http://qcs.meibo888.top

PHP:  PHP_OS;  phpversion();
来源：http://nhi.jinghuilouyu.cn

JS:   process.platform;  process.version
来源：http://syp.jqgufenzy.top

TS:   process.platform;  process.version
来源：http://mrm.xingfuxueyuan.xyz

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://jpd.wangshuangyany.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://ddn.hfpthk.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://kqw.jiagoushi.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://ged.aibaodan.cn

================================================================================
来源：http://baf.ybcxt.top

N. 数据结构与算法
来源：http://lbc.yuanzhike.top

================================================================================
来源：http://tun.jyoumei.cn

[N01] 二分查找（有序数组）
来源：http://fxx.jinyuanbaomall.cn

Py:   bisect.bisect_left(arr, x)
来源：http://xja.hnqzz.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://byo.yanxiufei.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://nnr.zdqjudy.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mpn.aizwys.cn

Java: Arrays.binarySearch(arr, x)
来源：http://hft.gotoacloud.top

Go:   sort.SearchInts(arr, x)
来源：http://qwk.yvedp.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://uao.tianlin.xyz

C#:   Array.BinarySearch(arr, x)
来源：http://noy.kuanghao11.cn

[N02] 排序（工程实践用内置实现）
来源：http://hfh.fengsongda.top

Py:   sorted(arr);  arr.sort()
来源：http://nlx.jinqigufen.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ftc.ydjk.org.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://nbr.zycfv.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://ziu.gaohongyu789.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://xre.vqdsnc.cn

Go:   slices.Sort(arr)
来源：http://vwl.iojbl.cn

Ruby: arr.sort
来源：http://evy.redwolf501.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://rcx.aibaodan.cn

[N03] 快速排序（分治示例）
来源：http://hql.gogol.net.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://uge.jqgfzy.top

PHP:  // 递归实现，或用 usort
来源：http://sch.tianlin.xyz

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://yse.cdnleiting.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://nul.xziqi.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://uit.iojbl.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://fnq.hnxiangtu.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ofq.chenlongwang.top

C#:   // 手写递归，或 Array.Sort
来源：http://hgl.cashguo.top

[N04] 斐波那契数列
来源：http://brv.kuanghao11.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://xfx.yfazqb.com

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://zws.jqgufenzy.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hgq.snrcjt.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://cvk.vehdjk.com

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://pmg.redwolf501.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ztl.fktsv.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://fhh.chenlongwang.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hsx.zhengqikj.top

[N05] 最大公约数
来源：http://zaj.xingfuxueyuan.xyz

Py:   math.gcd(a, b)
来源：http://bwx.xuanzx.com

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://rmh.tarul.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://btg.fanxiaobao.xyz

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://emj.zhongyouzk.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://lag.pycfn.com

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://idk.jqgufenzy.top

Ruby: a.gcd(b)
来源：http://iua.tanke756.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://dgd.iojbl.cn

[N06] 判断回文字符串
来源：http://mif.sysykeji.top

Py:   s == s[::-1]
来源：http://fih.snrcjt.cn

PHP:  $s === strrev($s);
来源：http://gwm.zhiwuduotai.top


<!-- 参考信息 -->