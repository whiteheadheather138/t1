代发 wailian999

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://cyc.uphjek.com

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ljd.snrcjt.cn

[J09] 时区处理
来源：http://vnp.tarul.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://brg.wangdashe.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://rqu.tianlin.xyz

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://fok.yvedp.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hqd.xingfuxueyuan.xyz

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://gzk.jqgfzy.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://sdi.daxiang520.top

Ruby: Time.now.getlocal("+08:00")
来源：http://kzi.jqgufenzy.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://aii.quarkkingdee.top

[J10] 取今天 / 本月第一天
来源：http://grb.jianghu66.top

Py:   date.today();  date.today().replace(day=1)
来源：http://oed.yj202588.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://rek.daria6918.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://qxv.shanyushiyangkeji.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://qhv.uphjek.com

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://zsw.jyoumei.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://res.sweek.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ggb.yj20258.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://xry.xuetiantiany.cn

================================================================================
来源：http://hbh.yonumen.top

K. JSON 与序列化
来源：http://nlq.sweek.top

================================================================================
来源：http://wid.hywenlv.cn

[K01] 对象转 JSON 字符串
来源：http://xbg.fengsongda.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://dux.meibo888.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://mvf.ydzc1.top

JS:   JSON.stringify(obj)
来源：http://vtw.yfazqb.com

TS:   JSON.stringify(obj)
来源：http://mba.shuidangran.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://lud.hnqzz.top

Go:   json.Marshal(obj)
来源：http://zws.zhengqikj.top

Ruby: obj.to_json                                     // require "json"
来源：http://smx.gotoacloud.top

C#:   JsonSerializer.Serialize(obj)
来源：http://cje.hysaishi.cn

[K02] JSON 字符串转对象
来源：http://mcr.jinghuilouyu.cn

Py:   json.loads(s)
来源：http://sou.xylfe.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://snz.sysykeji.top

JS:   JSON.parse(s)
来源：http://ate.fktsv.cn

TS:   JSON.parse(s)
来源：http://gdz.cucudq.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://qsr.hnqzz.top

Go:   json.Unmarshal(data, &v)
来源：http://pdk.feifeiyinyue.top

Ruby: JSON.parse(s)
来源：http://ulu.redwolf501.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://uyx.dashuyun.cn

[K03] JSON 美化输出（带缩进）
来源：http://sqq.cqqwz.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://fqd.gogol.net.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ayb.jlsjyb.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://itx.dashuyun.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://lwm.fengsongda.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://yns.yongpay.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://vkx.shanyushiyangtech.top

Ruby: JSON.pretty_generate(obj)
来源：http://jul.shanyushiyangtech.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://rgc.jinqigufen.top

[K04] 读取 JSON 文件
来源：http://feh.zhengqikj.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://swq.aizwys.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ndk.yueranfly.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://snv.yonumen.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hew.sysykeji.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://laa.yongpay.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://dqm.xziqi.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://ist.yfazqb.com

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://esd.xuetiantiany.cn

[K05] 深拷贝对象
来源：http://scl.hywenlv.cn

Py:   copy.deepcopy(obj)
来源：http://glr.cheryme.top

PHP:  unserialize(serialize($obj));
来源：http://dco.mhx1999.top

JS:   structuredClone(obj)
来源：http://nfe.haohaochexian.top

TS:   structuredClone(obj)
来源：http://yni.nwbrower.top

Java: // 手写拷贝构造，或序列化往返
来源：http://ixg.shanyushiyangtech.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hal.sysykeji.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://uic.yj20258.top

C#:   // 序列化往返，或自定义 Clone
来源：http://mvb.yfazqb.com

[K06] 解析 URL 查询串
来源：http://dik.havefunace.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://iqh.tianlin.xyz

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://wrn.hammf.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://zrh.fktsv.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://xfb.wangdashe.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://rgd.shzxlz.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://vuw.sysykeji.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ouc.wangshuangyany.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://lvv.xingfuxueyuan.xyz

[K07] 进制转换
来源：http://bdu.316326.xyz

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ggg.nwbrower.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://fvv.ydzc1.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://qno.gotoacloud.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://elf.yj20258.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://tjt.xziqi.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://koy.zdqjudy.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://leb.zhaomingkeji.xyz

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ors.fzhhl.top

[K08] 二进制序列化（非 JSON）
来源：http://jmc.c1oappe.top

Py:   pickle.dumps(obj)
来源：http://cah.wangshuangyany.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://nxo.daxiang520.top

JS:   v8.serialize(obj)        // Node
来源：http://ujj.feifeiyinyue.top

TS:   v8.serialize(obj)        // Node
来源：http://azz.haohaochexian.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://pvk.mhx1999.top

Go:   encoding/gob
来源：http://hky.mhx1999.top

Ruby: Marshal.dump(obj)
来源：http://rvx.ydjk.org.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://sgy.fehbvm.com

================================================================================
来源：http://gpm.bbcook.cn

L. 网络请求
来源：http://zbi.feifeiyinyue.top

================================================================================
来源：http://drl.xuetiantiany.cn

[L01] 发送 GET 请求
来源：http://hok.xuanzx.com

Py:   requests.get(url)                        # 第三方库 requests
来源：http://gxg.jinghuilouyu.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://vre.xingfuxueyuan.xyz

JS:   await fetch(url)
来源：http://vah.dianchejie.cn

TS:   await fetch(url)
来源：http://mlb.zdqjudy.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ems.fktsv.cn

Go:   resp, err := http.Get(url)
来源：http://jdc.ydzc1.top

Ruby: Net::HTTP.get(URI(url))
来源：http://okq.epnwcf.com

C#:   await new HttpClient().GetStringAsync(url)
来源：http://cbv.zhijiandao.cn

[L02] 发送 POST JSON
来源：http://dgg.gzhubu.top

Py:   requests.post(url, json={"a": 1})
来源：http://bwm.nanxinkj.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://sya.xziqi.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://iot.sysykeji.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://cpz.redwolf501.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://dlz.ydjk.org.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://axy.sufxvd.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://enx.cqqwz.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ted.cqqwz.cn

[L03] 设置自定义请求头
来源：http://tvz.zhongyouzk.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ohz.zhoulong.xyz

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://zns.jlsjyb.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://uhx.yuxming.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://yju.yangfankeji.com

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://pzi.sweek.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://nqg.aibaodan.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://egz.birdmap.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://vja.shanyushiyangtech.top

[L04] 设置超时
来源：http://cqr.aibaodan.cn

Py:   requests.get(url, timeout=5)
来源：http://dky.zhaomingkeji.xyz

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://elm.chenjidiqi.icu

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://vkc.shangyingyoupin.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://uaj.zdqjudy.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://pbr.ehwqpu.com

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://xbz.shuidangran.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://yhg.cheryme.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://xda.cdnleiting.top

[L05] 上传文件（multipart）
来源：http://mle.hnxiangtu.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://fff.fengsongda.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://eex.fktsv.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://emx.gaohongyu789.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://umm.ywan-chungtsiang.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ijk.jlsjyb.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mrm.epnwcf.com

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://aze.feifeiyinyue.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://trj.chenjidiqi.icu

[L06] 解析响应为 JSON
来源：http://jbb.quarkkingdee.top

Py:   resp.json()
来源：http://ejv.jinqigufen.top

PHP:  json_decode($body, true);
来源：http://dyk.zdqjudy.top

JS:   await resp.json()
来源：http://hzh.hnxiangtu.top

TS:   await resp.json()
来源：http://qry.jinqigufen.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://sdq.aizwys.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://lib.hnxiangtu.top

Ruby: JSON.parse(resp.body)
来源：http://yeg.hnxiangtu.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://inn.vehdjk.com

[L07] 处理 HTTP 状态码
来源：http://wtn.yfazqb.com

Py:   resp.status_code;  resp.raise_for_status()
来源：http://cjx.hongshengwenyu.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mmx.zhoulong.xyz

JS:   resp.ok;  resp.status
来源：http://wnp.ivvv.top

TS:   resp.ok;  resp.status
来源：http://svo.c1oappe.top

Java: resp.statusCode()
来源：http://zet.zhongyouzk.top

Go:   resp.StatusCode
来源：http://wpu.yuanzhike.top

Ruby: resp.code.to_i
来源：http://rqr.zycfv.cn

C#:   (int)resp.StatusCode
来源：http://myl.aibaodan.cn

[L08] 并发请求多个地址
来源：http://cif.ctjpmb.com

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://but.jqgufenzy.top

PHP:  curl_multi_init() 系列
来源：http://hxs.zhongyouzk.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://jhi.shuidangran.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://dzv.ppjwa.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://qhf.nanxuanxn.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://vvy.jqgufenzy.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ivg.xylfe.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://kbg.jinyuanbaomall.cn

================================================================================
来源：http://axl.316326.xyz

M. 命令行 / 进程 / 环境
来源：http://zmk.chenzaomai.com

================================================================================
来源：http://npt.jlsjyb.cn

[M01] 读取命令行参数
来源：http://sgk.zhiwuduotai.top

Py:   sys.argv[1:]
来源：http://kxp.epnwcf.com

PHP:  $argv;  $argc;
来源：http://uqg.dianchejie.cn

JS:   process.argv.slice(2)
来源：http://ydn.zhongyouzk.top

TS:   process.argv.slice(2)
来源：http://dyu.jinqigufen.top

Java: args 数组（main 方法参数）
来源：http://oxg.cqqwz.cn

Go:   os.Args[1:]
来源：http://ahh.zhiwuduotai.top

Ruby: ARGV
来源：http://iew.zdqjudy.top

C#:   args 数组（Main 方法参数）
来源：http://xai.hcnkem.com

[M02] 读取环境变量
来源：http://kab.zhoulong.xyz

Py:   os.environ.get("HOME")
来源：http://fxv.feifeiyinyue.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://cik.zhaomingkeji.xyz

JS:   process.env.HOME
来源：http://onj.shuidangran.top

TS:   process.env.HOME
来源：http://wfq.sxryk.cn

Java: System.getenv("HOME")
来源：http://yib.hywenlv.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://riz.hnqzz.top

Ruby: ENV["HOME"]
来源：http://edq.uphjek.com

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://gis.tanke756.top

[M03] 执行外部命令
来源：http://ytm.yfazqb.com

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://jql.shuidangran.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mzm.dianchejie.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://uef.pycfn.com

TS:   child_process.execSync("ls -l").toString()
来源：http://sbw.jqgufenzy.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wrk.0kj1m.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://zln.daria6918.cn

Ruby: system("ls -l");  `ls -l`
来源：http://ohl.tarul.cn

C#:   Process.Start("ls", "-l");
来源：http://etg.xylfe.cn

[M04] 获取当前工作目录
来源：http://rno.zhongyouzk.top

Py:   os.getcwd()
来源：http://kmt.hammf.cn

PHP:  getcwd();
来源：http://zcc.tanke756.top

JS:   process.cwd()
来源：http://stm.zhiwuduotai.top

TS:   process.cwd()
来源：http://ret.nanxinkj.top

Java: Path.of("").toAbsolutePath()
来源：http://vfp.sweek.top

Go:   os.Getwd()
来源：http://wjv.zdbjq.cn

Ruby: Dir.pwd
来源：http://scp.yueranfly.top

C#:   Directory.GetCurrentDirectory()
来源：http://urp.andypj.xyz

[M05] 设置退出码
来源：http://hxh.xylfe.cn

Py:   sys.exit(1)
来源：http://qbn.fktsv.cn

PHP:  exit(1);
来源：http://mxc.jinghuilouyu.cn

JS:   process.exit(1)
来源：http://bza.jlsjyb.cn

TS:   process.exit(1)
来源：http://cal.hammf.cn

Java: System.exit(1)
来源：http://mkh.yuanzhike.top

Go:   os.Exit(1)
来源：http://qcl.ywan-chungtsiang.top

Ruby: exit 1
来源：http://idv.xuanzx.com

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://igk.haohaochexian.top

[M06] 向标准错误输出
来源：http://syn.nanxinkj.top

Py:   print("err", file=sys.stderr)
来源：http://nff.yueranfly.top

PHP:  fwrite(STDERR, "err\n");
来源：http://iqe.zycfv.cn

JS:   console.error("err")
来源：http://apj.zycfv.cn

TS:   console.error("err")
来源：http://cih.0kj1m.cn

Java: System.err.println("err")
来源：http://pjl.zhijiandao.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://gbb.pengpengdd.cyou

Ruby: warn "err"
来源：http://woj.9152youxi.cn

C#:   Console.Error.WriteLine("err")
来源：http://xwp.yj20258.top

[M07] 判断是否为主入口
来源：http://cib.yj20258888.top

Py:   if __name__ == "__main__":
来源：http://xdj.cdnleiting.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://pcv.pengpengdd.cyou

JS:   require.main === module
来源：http://cyz.havefunace.top

TS:   require.main === module
来源：http://rwk.yj202588.top

Java: public static void main(String[] args)
来源：http://rxb.wangshuangyany.cn

Go:   func main()
来源：http://ywe.chenlongwang.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://aoc.sweek.top

C#:   static void Main(string[] args)
来源：http://der.zhongyouzk.top

[M08] 获取系统与运行时信息
来源：http://jsk.mhx1999.top

Py:   platform.system();  platform.python_version()
来源：http://vkc.zhaomingkeji.xyz

PHP:  PHP_OS;  phpversion();
来源：http://vkq.jyoumei.cn

JS:   process.platform;  process.version
来源：http://uwe.zhaomingkeji.xyz

TS:   process.platform;  process.version
来源：http://vkm.smart0.xyz

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://jcm.yuanzhike.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://dlq.bjfxy.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://nta.yonumen.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://kcl.haohaochexian.top

================================================================================
来源：http://zpb.fengsongda.top

N. 数据结构与算法
来源：http://lfr.vqdsnc.cn

================================================================================
来源：http://ugc.wangshuangyany.cn

[N01] 二分查找（有序数组）
来源：http://qka.yuanzhike.top

Py:   bisect.bisect_left(arr, x)
来源：http://ckp.yvedp.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://uyo.tarul.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://tnx.hywenlv.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://pjg.zhaomingkeji.xyz

Java: Arrays.binarySearch(arr, x)
来源：http://sli.nanxinkj.top

Go:   sort.SearchInts(arr, x)
来源：http://wyz.uphjek.com

Ruby: arr.bsearch { |e| e >= x }
来源：http://yxn.ehwqpu.com

C#:   Array.BinarySearch(arr, x)
来源：http://mgn.gogol.net.cn

[N02] 排序（工程实践用内置实现）
来源：http://gdt.zhengqikj.top

Py:   sorted(arr);  arr.sort()
来源：http://bss.52xcode.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://rkc.shangyingyoupin.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://zqk.zhixingplan.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://hii.fengsongda.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://cfv.tanke756.top

Go:   slices.Sort(arr)
来源：http://dsy.yueranfly.top

Ruby: arr.sort
来源：http://rpd.fanxiaobao.xyz

C#:   Array.Sort(arr);  list.Sort()
来源：http://svv.ehwqpu.com

[N03] 快速排序（分治示例）
来源：http://ndr.vehdjk.com

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://fvd.vqdsnc.cn

PHP:  // 递归实现，或用 usort
来源：http://buw.zdqjudy.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://bhx.dianchejie.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mkk.jiagoushi.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://qec.sjlbkw.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://paz.daria6918.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://xif.xingfuxueyuan.xyz

C#:   // 手写递归，或 Array.Sort
来源：http://hry.hywenlv.cn

[N04] 斐波那契数列
来源：http://oup.wangshuangyany.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://fck.jqgufenzy.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://kno.nanxuanxn.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://sue.ydjk.org.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://onk.fzhhl.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://lql.aibaodan.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://irh.yj202588.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://vai.ydzc1.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hze.wangdashe.top

[N05] 最大公约数
来源：http://pwv.jqgufenzy.top

Py:   math.gcd(a, b)
来源：http://krd.shangyingyoupin.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wnk.xinyue.icu

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wvk.xziqi.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://anz.ivvv.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://cwn.cdnleiting.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://bky.uphjek.com

Ruby: a.gcd(b)
来源：http://yfc.jqgufenzy.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hua.ywan-chungtsiang.top

[N06] 判断回文字符串
来源：http://ddx.fktsv.cn

Py:   s == s[::-1]
来源：http://vfl.daxiang520.top

PHP:  $s === strrev($s);
来源：http://spq.52xcode.cn

JS:   s === [...s].reverse().join("")
来源：http://hvx.ehwqpu.com

TS:   s === [...s].reverse().join("")
来源：http://clg.jinqigfzy.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://xrv.jqgufenzy.top

Go:   // 双指针从两端比较
来源：http://twb.9152youxi.cn


<!-- 参考信息 -->