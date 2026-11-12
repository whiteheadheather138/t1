代发 wailian999

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://mqi.xingfuxueyuan.xyz

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://dfz.yonumen.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://icr.cashguo.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://imm.zhixingplan.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://xyk.xylfe.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://edo.iojbl.cn

[J09] 时区处理
来源：http://iit.jiagoushi.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://zsz.chenlongwang.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://jhz.zhongyouzk.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ajd.yuxming.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://alb.zycfv.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://gbs.jlsjyb.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://bwh.tian-w.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://zaw.kuanghao11.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://tvt.shanyushiyangkeji.top

[J10] 取今天 / 本月第一天
来源：http://vas.guannengcc.top

Py:   date.today();  date.today().replace(day=1)
来源：http://obo.zhixingplan.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://uxf.quarkkingdee.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://arz.fehbvm.com

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://aio.ydzc1.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://bdi.epnwcf.com

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://vsm.hammf.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://zkw.shuidangran.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ken.0kj1m.cn

================================================================================
来源：http://pub.chenzaomai.com

K. JSON 与序列化
来源：http://xdm.9152youxi.cn

================================================================================
来源：http://wmt.zhengqikj.top

[K01] 对象转 JSON 字符串
来源：http://atk.tanke756.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ude.jlsjyb.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://aav.xuetiantiany.cn

JS:   JSON.stringify(obj)
来源：http://wrm.gotoacloud.top

TS:   JSON.stringify(obj)
来源：http://inr.dashuyun.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://dir.jianghu66.top

Go:   json.Marshal(obj)
来源：http://wwy.bbcook.cn

Ruby: obj.to_json                                     // require "json"
来源：http://oiu.ehwqpu.com

C#:   JsonSerializer.Serialize(obj)
来源：http://uww.cqqwz.cn

[K02] JSON 字符串转对象
来源：http://qke.chenlongwang.top

Py:   json.loads(s)
来源：http://vpx.yj20258888.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://rmn.hesvh.cn

JS:   JSON.parse(s)
来源：http://dlw.gzhubu.top

TS:   JSON.parse(s)
来源：http://utm.jinqigfzy.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hvx.cheryme.top

Go:   json.Unmarshal(data, &v)
来源：http://tuh.zhaomingkeji.xyz

Ruby: JSON.parse(s)
来源：http://ibi.vehdjk.com

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mcf.yfazqb.com

[K03] JSON 美化输出（带缩进）
来源：http://rfv.andypj.xyz

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://zie.yj20258888.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://lol.cdnleiting.top

JS:   JSON.stringify(obj, null, 2)
来源：http://zei.aizwys.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://ijx.tarul.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://fvi.havefunace.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://vqs.tarul.cn

Ruby: JSON.pretty_generate(obj)
来源：http://eqt.hcnkem.com

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://aaz.xuetiantiany.cn

[K04] 读取 JSON 文件
来源：http://gfu.ctjpmb.com

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://opw.redwolf501.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://sal.zdbjq.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://evw.316326.xyz

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://upm.fehbvm.com

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://rwb.bbcook.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://tpz.nanxuanxn.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://zic.hcnkem.com

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://tud.xziqi.cn

[K05] 深拷贝对象
来源：http://ozx.yvedp.cn

Py:   copy.deepcopy(obj)
来源：http://ylk.jqgufenzy.top

PHP:  unserialize(serialize($obj));
来源：http://bmx.zhaomingkeji.xyz

JS:   structuredClone(obj)
来源：http://lsy.xinyue.icu

TS:   structuredClone(obj)
来源：http://rub.vqdsnc.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://iyx.zycfv.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://uqd.shuidangran.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://wrn.xziqi.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://yge.sxryk.cn

[K06] 解析 URL 查询串
来源：http://fdh.vqdsnc.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://lxj.andypj.xyz

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mjq.dashuyun.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://cth.ydjk.org.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://znw.zdbjq.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://rak.jinghuilouyu.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://sfk.kuanghao11.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://yfp.sweek.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://nsc.cqqwz.cn

[K07] 进制转换
来源：http://sum.cdnleiting.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://iuj.wangshuangyany.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://xex.gzhubu.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ojn.xuetiantiany.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://jyc.redwolf501.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://vjn.sufxvd.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://epe.jinyuanbaomall.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://wtc.nwbrower.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://lug.hywenlv.cn

[K08] 二进制序列化（非 JSON）
来源：http://bmj.c1oappe.top

Py:   pickle.dumps(obj)
来源：http://quo.hywenlv.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://diu.zhoulong.xyz

JS:   v8.serialize(obj)        // Node
来源：http://iqh.quarkkingdee.top

TS:   v8.serialize(obj)        // Node
来源：http://ysj.jinyuanbaomall.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://pid.fanxiaobao.xyz

Go:   encoding/gob
来源：http://abn.tanke756.top

Ruby: Marshal.dump(obj)
来源：http://rue.xylfe.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wst.jlsjyb.cn

================================================================================
来源：http://ual.shanyushiyangkeji.top

L. 网络请求
来源：http://har.ybcxt.top

================================================================================
来源：http://ypa.cheryme.top

[L01] 发送 GET 请求
来源：http://kdp.aizwys.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ghv.wangdashe.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://qwm.yuxming.cn

JS:   await fetch(url)
来源：http://iwn.fktsv.cn

TS:   await fetch(url)
来源：http://uyo.chenzaomai.com

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ehm.ctjpmb.com

Go:   resp, err := http.Get(url)
来源：http://zmi.nanxinkj.top

Ruby: Net::HTTP.get(URI(url))
来源：http://jar.quarkkingdee.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://yez.wangdashe.top

[L02] 发送 POST JSON
来源：http://mpo.hfpthk.cn

Py:   requests.post(url, json={"a": 1})
来源：http://neu.yj20258888.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ofk.zhoulong.xyz

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://kud.0kj1m.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://myt.shuidangran.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://epc.jqgufenzy.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://api.ywan-chungtsiang.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ppv.birdmap.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://fwg.gzhubu.top

[L03] 设置自定义请求头
来源：http://sid.hcnkem.com

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://jvd.fehbvm.com

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://csp.jinghuilouyu.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://dpz.haohaochexian.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://phn.chenlongwang.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://clh.dashuyun.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://yqj.jinqigfzy.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://qgx.yfazqb.com

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://xmv.yonumen.top

[L04] 设置超时
来源：http://qlx.shanyushiyangkeji.top

Py:   requests.get(url, timeout=5)
来源：http://kbv.tanke756.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hbx.hfpthk.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://cet.sjlbkw.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wbc.yuxming.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://pnr.hnxiangtu.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://jwa.yuxming.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://giu.aizwys.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://llh.zhongyouzk.top

[L05] 上传文件（multipart）
来源：http://wxl.nwbrower.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://gek.fanxiaobao.xyz

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://vzo.shanyushiyangtech.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://nwk.shangyingyoupin.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://fsm.dianchejie.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://bpt.jinyuanbaomall.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://xfy.daxiang520.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://vkl.gaohongyu789.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://sxy.hesvh.cn

[L06] 解析响应为 JSON
来源：http://uud.c1oappe.top

Py:   resp.json()
来源：http://jxf.fanxiaobao.xyz

PHP:  json_decode($body, true);
来源：http://cuf.xuetiantiany.cn

JS:   await resp.json()
来源：http://zrz.hfpthk.cn

TS:   await resp.json()
来源：http://sxd.iojbl.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://cvk.uphjek.com

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://pmq.nanxinkj.top

Ruby: JSON.parse(resp.body)
来源：http://gqx.yuanzhike.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://nyt.316326.xyz

[L07] 处理 HTTP 状态码
来源：http://jle.jinqigfzy.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://bjl.fzhhl.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ury.zycfv.cn

JS:   resp.ok;  resp.status
来源：http://pvb.feifeiyinyue.top

TS:   resp.ok;  resp.status
来源：http://flb.shanyushiyangtech.top

Java: resp.statusCode()
来源：http://zxz.sjlbkw.cn

Go:   resp.StatusCode
来源：http://qdx.ivvv.top

Ruby: resp.code.to_i
来源：http://hjw.yuanzhike.top

C#:   (int)resp.StatusCode
来源：http://ppf.shzxlz.cn

[L08] 并发请求多个地址
来源：http://jhe.zhongyouzk.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://gtn.bjfxy.top

PHP:  curl_multi_init() 系列
来源：http://lnh.c1oappe.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ylb.sxryk.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://gxk.chenzaomai.com

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://kaw.fktsv.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://bre.cashguo.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://xle.hfpthk.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://fqn.meibo888.top

================================================================================
来源：http://xxc.aibaodan.cn

M. 命令行 / 进程 / 环境
来源：http://mzm.hammf.cn

================================================================================
来源：http://xxh.xziqi.cn

[M01] 读取命令行参数
来源：http://tms.zhoulong.xyz

Py:   sys.argv[1:]
来源：http://gpw.yonumen.top

PHP:  $argv;  $argc;
来源：http://ssj.epnwcf.com

JS:   process.argv.slice(2)
来源：http://awx.yuanzhike.top

TS:   process.argv.slice(2)
来源：http://tji.wangshuangyany.cn

Java: args 数组（main 方法参数）
来源：http://hti.hysaishi.cn

Go:   os.Args[1:]
来源：http://pve.fktsv.cn

Ruby: ARGV
来源：http://yub.xziqi.cn

C#:   args 数组（Main 方法参数）
来源：http://uti.hammf.cn

[M02] 读取环境变量
来源：http://qvw.zhengqikj.top

Py:   os.environ.get("HOME")
来源：http://ylf.nwbrower.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://eud.cdnleiting.top

JS:   process.env.HOME
来源：http://ehd.hysaishi.cn

TS:   process.env.HOME
来源：http://qyr.birdmap.top

Java: System.getenv("HOME")
来源：http://ijj.yueranfly.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://dkl.zdqjudy.top

Ruby: ENV["HOME"]
来源：http://uif.yueranfly.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://zth.svipenyu.cn

[M03] 执行外部命令
来源：http://fcj.ydjk.org.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://oxs.zycfv.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://vkh.gzhubu.top

JS:   child_process.execSync("ls -l").toString()
来源：http://vor.ywan-chungtsiang.top

TS:   child_process.execSync("ls -l").toString()
来源：http://tvd.zdqjudy.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://eut.xinyue.icu

Go:   exec.Command("ls", "-l").Output()
来源：http://nqo.ivvv.top

Ruby: system("ls -l");  `ls -l`
来源：http://eyf.52xcode.cn

C#:   Process.Start("ls", "-l");
来源：http://nxm.mhx1999.top

[M04] 获取当前工作目录
来源：http://wrk.cqqwz.cn

Py:   os.getcwd()
来源：http://exy.ctjpmb.com

PHP:  getcwd();
来源：http://cbx.hywenlv.cn

JS:   process.cwd()
来源：http://orh.ydjk.org.cn

TS:   process.cwd()
来源：http://zia.zycfv.cn

Java: Path.of("").toAbsolutePath()
来源：http://wxm.gogol.net.cn

Go:   os.Getwd()
来源：http://bno.nwbrower.top

Ruby: Dir.pwd
来源：http://erq.hfpthk.cn

C#:   Directory.GetCurrentDirectory()
来源：http://kld.zdqjudy.top

[M05] 设置退出码
来源：http://zfm.zdbjq.cn

Py:   sys.exit(1)
来源：http://huc.yj20258.top

PHP:  exit(1);
来源：http://mjg.jinghuilouyu.cn

JS:   process.exit(1)
来源：http://hat.zhiwuduotai.top

TS:   process.exit(1)
来源：http://qth.tian-w.cn

Java: System.exit(1)
来源：http://ovk.fktsv.cn

Go:   os.Exit(1)
来源：http://eoi.jiagoushi.top

Ruby: exit 1
来源：http://pks.cucudq.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ccm.ivvv.top

[M06] 向标准错误输出
来源：http://exc.fanxiaobao.xyz

Py:   print("err", file=sys.stderr)
来源：http://bwt.zycfv.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://nry.cheryme.top

JS:   console.error("err")
来源：http://byp.birdmap.top

TS:   console.error("err")
来源：http://lhp.vehdjk.com

Java: System.err.println("err")
来源：http://qss.zycfv.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mnt.svipenyu.cn

Ruby: warn "err"
来源：http://wln.zhengqikj.top

C#:   Console.Error.WriteLine("err")
来源：http://xwn.bbcook.cn

[M07] 判断是否为主入口
来源：http://itx.jqgufenzy.top

Py:   if __name__ == "__main__":
来源：http://ejw.fktsv.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://djz.meibo888.top

JS:   require.main === module
来源：http://uck.iojbl.cn

TS:   require.main === module
来源：http://nse.zdqjudy.top

Java: public static void main(String[] args)
来源：http://jze.hnxiangtu.top

Go:   func main()
来源：http://osl.vehdjk.com

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://jrf.uphjek.com

C#:   static void Main(string[] args)
来源：http://csu.pycfn.com

[M08] 获取系统与运行时信息
来源：http://vlp.yueranfly.top

Py:   platform.system();  platform.python_version()
来源：http://jiy.iojbl.cn

PHP:  PHP_OS;  phpversion();
来源：http://wls.aibaodan.cn

JS:   process.platform;  process.version
来源：http://eeq.zdqjudy.top

TS:   process.platform;  process.version
来源：http://wiw.epnwcf.com

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://gvc.hcnkem.com

Go:   runtime.GOOS;  runtime.Version()
来源：http://odg.daxiang520.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://pdg.zdbjq.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://tvb.fktsv.cn

================================================================================
来源：http://hwv.nanxinkj.top

N. 数据结构与算法
来源：http://lhr.cheryme.top

================================================================================
来源：http://qya.sjlbkw.cn

[N01] 二分查找（有序数组）
来源：http://vpj.sjlbkw.cn

Py:   bisect.bisect_left(arr, x)
来源：http://dji.mhx1999.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://uco.jinghuilouyu.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wrr.hongshengwenyu.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://nup.zycfv.cn

Java: Arrays.binarySearch(arr, x)
来源：http://irm.xylfe.cn

Go:   sort.SearchInts(arr, x)
来源：http://tgt.sjlbkw.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://ash.jianghu66.top

C#:   Array.BinarySearch(arr, x)
来源：http://vjx.cucudq.cn

[N02] 排序（工程实践用内置实现）
来源：http://qqp.xingfuxueyuan.xyz

Py:   sorted(arr);  arr.sort()
来源：http://oyi.fengsongda.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://cfx.tian-w.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://lyv.hnqzz.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://vpl.gotoacloud.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://pkz.ivvv.top

Go:   slices.Sort(arr)
来源：http://und.jlsjyb.cn

Ruby: arr.sort
来源：http://rzu.hcnkem.com

C#:   Array.Sort(arr);  list.Sort()
来源：http://znd.cqqwz.cn

[N03] 快速排序（分治示例）
来源：http://kml.chenjidiqi.icu

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ujp.hnqzz.top

PHP:  // 递归实现，或用 usort
来源：http://vgb.hnxiangtu.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://pdl.shangyingyoupin.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ozm.xziqi.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://rye.zhengqikj.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://fkc.ywan-chungtsiang.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://vqs.pycfn.com

C#:   // 手写递归，或 Array.Sort
来源：http://lia.fengsongda.top

[N04] 斐波那契数列
来源：http://cbk.dashuyun.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://bba.jinghuilouyu.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://vbt.shzxlz.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ypi.gogol.net.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://esk.sufxvd.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://bku.xziqi.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://owl.nanxuanxn.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://teo.jlsjyb.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mfa.kuanghao11.cn

[N05] 最大公约数
来源：http://psj.chenjidiqi.icu

Py:   math.gcd(a, b)
来源：http://vjy.cdnleiting.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://rjw.tianlin.xyz

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://urg.ctjpmb.com

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://fpw.shanyushiyangkeji.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://kkb.chenlongwang.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wys.zycfv.cn

Ruby: a.gcd(b)
来源：http://zab.ywan-chungtsiang.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://brx.jinghuilouyu.cn

[N06] 判断回文字符串
来源：http://tzu.sweek.top

Py:   s == s[::-1]
来源：http://ebq.havefunace.top

PHP:  $s === strrev($s);
来源：http://jdq.daria6918.cn


<!-- 参考信息 -->