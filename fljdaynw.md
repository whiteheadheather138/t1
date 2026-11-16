代发 wailian999

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://dnm.shanyushiyangtech.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://prd.jlsjyb.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://tlz.guannengcc.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://thz.shanyushiyangtech.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://yks.wangdashe.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://kiq.snrcjt.cn

[J09] 时区处理
来源：http://nca.gaohongyu789.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://gbr.haohaochexian.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://nxj.aibaodan.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://uut.hnxiangtu.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://kmt.yj202588.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://bte.vehdjk.com

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://lpj.epnwcf.com

Ruby: Time.now.getlocal("+08:00")
来源：http://tep.fktsv.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://kbg.cheryme.top

[J10] 取今天 / 本月第一天
来源：http://jdg.c1oappe.top

Py:   date.today();  date.today().replace(day=1)
来源：http://csj.jinqigufen.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://chw.gogol.net.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://jzu.ybcxt.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://zsy.aibaodan.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://vic.hnqzz.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hsj.ctjpmb.com

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://uvd.xingfuxueyuan.xyz

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://uhl.pycfn.com

================================================================================
来源：http://yww.jinqigfzy.top

K. JSON 与序列化
来源：http://zwo.ybcxt.top

================================================================================
来源：http://tlf.jqgufenzy.top

[K01] 对象转 JSON 字符串
来源：http://kne.fehbvm.com

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://bsu.ywan-chungtsiang.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://qnx.yuxming.cn

JS:   JSON.stringify(obj)
来源：http://zas.jianghu66.top

TS:   JSON.stringify(obj)
来源：http://zyr.jinyuanbaomall.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hhr.meibo888.top

Go:   json.Marshal(obj)
来源：http://hby.yuanzhike.top

Ruby: obj.to_json                                     // require "json"
来源：http://iza.ctjpmb.com

C#:   JsonSerializer.Serialize(obj)
来源：http://xxg.cqqwz.cn

[K02] JSON 字符串转对象
来源：http://lef.gzhubu.top

Py:   json.loads(s)
来源：http://tqn.yuxming.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ymi.birdmap.top

JS:   JSON.parse(s)
来源：http://hly.andypj.xyz

TS:   JSON.parse(s)
来源：http://ryu.cashguo.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://imn.chenzaomai.com

Go:   json.Unmarshal(data, &v)
来源：http://cbi.yfazqb.com

Ruby: JSON.parse(s)
来源：http://sqg.hywenlv.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://rax.yfazqb.com

[K03] JSON 美化输出（带缩进）
来源：http://zxz.uphjek.com

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://fqu.gogol.net.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://pgt.hnqzz.top

JS:   JSON.stringify(obj, null, 2)
来源：http://jtv.zhengqikj.top

TS:   JSON.stringify(obj, null, 2)
来源：http://led.tian-w.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://qwo.aizwys.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://oaf.haohaochexian.top

Ruby: JSON.pretty_generate(obj)
来源：http://ned.tianlin.xyz

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://zpl.fengsongda.top

[K04] 读取 JSON 文件
来源：http://nuo.andypj.xyz

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hfh.zhaomingkeji.xyz

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://onc.zdqjudy.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wrv.ybcxt.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://zkg.yvedp.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ofr.bbcook.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wai.nwbrower.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://bop.nanxinkj.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://qft.dashuyun.cn

[K05] 深拷贝对象
来源：http://wxg.fanxiaobao.xyz

Py:   copy.deepcopy(obj)
来源：http://bkl.wangshuangyany.cn

PHP:  unserialize(serialize($obj));
来源：http://dzh.shanyushiyangkeji.top

JS:   structuredClone(obj)
来源：http://inh.tianlin.xyz

TS:   structuredClone(obj)
来源：http://fkb.jinyuanbaomall.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://afy.shangyingyoupin.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://lsk.nanxinkj.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://wuj.ywan-chungtsiang.top

C#:   // 序列化往返，或自定义 Clone
来源：http://wkr.ivvv.top

[K06] 解析 URL 查询串
来源：http://scl.cheryme.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://rui.iojbl.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://znk.tarul.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://bzr.cucudq.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://fgm.cqqwz.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://pmr.sjlbkw.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://alo.hnxiangtu.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://mzy.sweek.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ugt.feifeiyinyue.top

[K07] 进制转换
来源：http://uhl.hfpthk.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://zld.gotoacloud.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ucc.52xcode.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://dro.hongshengwenyu.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://zos.haohaochexian.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://zwz.aizwys.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://owc.dashuyun.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://epd.ctjpmb.com

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://rdt.zycfv.cn

[K08] 二进制序列化（非 JSON）
来源：http://fpa.chenjidiqi.icu

Py:   pickle.dumps(obj)
来源：http://lxv.sweek.top

PHP:  serialize($obj);  unserialize($s);
来源：http://zwg.guannengcc.top

JS:   v8.serialize(obj)        // Node
来源：http://ude.yanxiufei.cn

TS:   v8.serialize(obj)        // Node
来源：http://mmt.zhongyouzk.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://sff.shzxlz.cn

Go:   encoding/gob
来源：http://nuh.c1oappe.top

Ruby: Marshal.dump(obj)
来源：http://nwt.ydzc1.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://nda.gzhubu.top

================================================================================
来源：http://zve.xylfe.cn

L. 网络请求
来源：http://hjk.ppjwa.cn

================================================================================
来源：http://lpt.zhiwuduotai.top

[L01] 发送 GET 请求
来源：http://pqr.cashguo.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ino.zhoulong.xyz

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://axk.jianghu66.top

JS:   await fetch(url)
来源：http://atj.ywan-chungtsiang.top

TS:   await fetch(url)
来源：http://fia.zhengqikj.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://dnh.tarul.cn

Go:   resp, err := http.Get(url)
来源：http://wnj.jyoumei.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://cdv.vehdjk.com

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ygx.c1oappe.top

[L02] 发送 POST JSON
来源：http://ahw.daria6918.cn

Py:   requests.post(url, json={"a": 1})
来源：http://wne.ctjpmb.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://knu.xinyue.icu

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wit.chenlongwang.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://heq.fehbvm.com

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wuo.sjlbkw.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://kix.zdqjudy.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://bzx.fzhhl.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://cxd.vehdjk.com

[L03] 设置自定义请求头
来源：http://uia.xylfe.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://uaf.yongpay.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://xun.gogol.net.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://trq.hywenlv.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://rbn.shanyushiyangkeji.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ygu.gogol.net.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://xpg.tianlin.xyz

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ibt.jlsjyb.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://jdr.ctjpmb.com

[L04] 设置超时
来源：http://plu.cashguo.top

Py:   requests.get(url, timeout=5)
来源：http://wnl.jiagoushi.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://fgo.zdbjq.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://zbe.shangyingyoupin.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mgv.yueranfly.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://rty.fehbvm.com

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://chu.jyoumei.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hea.chenjidiqi.icu

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://car.hesvh.cn

[L05] 上传文件（multipart）
来源：http://tch.meibo888.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://gun.cdnleiting.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://cmy.cucudq.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ija.quarkkingdee.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://jlf.9152youxi.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://qte.zdqjudy.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wtj.zhiwuduotai.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://rii.xinyue.icu

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://fxp.aizwys.cn

[L06] 解析响应为 JSON
来源：http://pkt.yuanzhike.top

Py:   resp.json()
来源：http://oax.wangshuangyany.cn

PHP:  json_decode($body, true);
来源：http://zvd.tanke756.top

JS:   await resp.json()
来源：http://fxy.tianlin.xyz

TS:   await resp.json()
来源：http://nll.quarkkingdee.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://nfg.yj20258888.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://new.jqgfzy.top

Ruby: JSON.parse(resp.body)
来源：http://ywf.hywenlv.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mrt.smart0.xyz

[L07] 处理 HTTP 状态码
来源：http://tzp.ydjk.org.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://lsg.xuetiantiany.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ire.mhx1999.top

JS:   resp.ok;  resp.status
来源：http://bdd.daria6918.cn

TS:   resp.ok;  resp.status
来源：http://czc.hnxiangtu.top

Java: resp.statusCode()
来源：http://vxa.sysykeji.top

Go:   resp.StatusCode
来源：http://hbp.snrcjt.cn

Ruby: resp.code.to_i
来源：http://jhf.tanke756.top

C#:   (int)resp.StatusCode
来源：http://wlu.mhx1999.top

[L08] 并发请求多个地址
来源：http://ulx.ydzc1.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://upv.0kj1m.cn

PHP:  curl_multi_init() 系列
来源：http://axj.shzxlz.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://kfx.smart0.xyz

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://npt.yongpay.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://tha.fengsongda.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://era.xuetiantiany.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://cko.jqgfzy.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://qus.andypj.xyz

================================================================================
来源：http://pyp.cheryme.top

M. 命令行 / 进程 / 环境
来源：http://ujo.aibaodan.cn

================================================================================
来源：http://rvr.andypj.xyz

[M01] 读取命令行参数
来源：http://bex.cucudq.cn

Py:   sys.argv[1:]
来源：http://dnw.yj20258.top

PHP:  $argv;  $argc;
来源：http://cvn.fktsv.cn

JS:   process.argv.slice(2)
来源：http://thl.chenzaomai.com

TS:   process.argv.slice(2)
来源：http://hdi.hesvh.cn

Java: args 数组（main 方法参数）
来源：http://zwp.hnqzz.top

Go:   os.Args[1:]
来源：http://ijt.shangyingyoupin.top

Ruby: ARGV
来源：http://ohb.gogol.net.cn

C#:   args 数组（Main 方法参数）
来源：http://umq.epnwcf.com

[M02] 读取环境变量
来源：http://oto.haohaochexian.top

Py:   os.environ.get("HOME")
来源：http://vua.yongpay.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hbo.ydzc1.top

JS:   process.env.HOME
来源：http://tnx.gzhubu.top

TS:   process.env.HOME
来源：http://quo.yj20258.top

Java: System.getenv("HOME")
来源：http://gia.jinyuanbaomall.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://cyd.ydzc1.top

Ruby: ENV["HOME"]
来源：http://pzt.hongshengwenyu.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://gyh.jlsjyb.cn

[M03] 执行外部命令
来源：http://oij.xuetiantiany.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://lca.mhx1999.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mmf.jinghuilouyu.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://abo.ywan-chungtsiang.top

TS:   child_process.execSync("ls -l").toString()
来源：http://bpj.sufxvd.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://uvv.yonumen.top

Go:   exec.Command("ls", "-l").Output()
来源：http://vms.cdnleiting.top

Ruby: system("ls -l");  `ls -l`
来源：http://oqm.kuanghao11.cn

C#:   Process.Start("ls", "-l");
来源：http://xlx.daria6918.cn

[M04] 获取当前工作目录
来源：http://gfp.cashguo.top

Py:   os.getcwd()
来源：http://uem.andypj.xyz

PHP:  getcwd();
来源：http://zyk.cheryme.top

JS:   process.cwd()
来源：http://udc.yongpay.top

TS:   process.cwd()
来源：http://gty.52xcode.cn

Java: Path.of("").toAbsolutePath()
来源：http://siu.smart0.xyz

Go:   os.Getwd()
来源：http://aut.jianghu66.top

Ruby: Dir.pwd
来源：http://rcr.havefunace.top

C#:   Directory.GetCurrentDirectory()
来源：http://qwh.yvedp.cn

[M05] 设置退出码
来源：http://zsd.zycfv.cn

Py:   sys.exit(1)
来源：http://jgf.xuetiantiany.cn

PHP:  exit(1);
来源：http://cpf.tarul.cn

JS:   process.exit(1)
来源：http://lxs.yangfankeji.com

TS:   process.exit(1)
来源：http://kdg.vehdjk.com

Java: System.exit(1)
来源：http://qxd.uphjek.com

Go:   os.Exit(1)
来源：http://hjo.cheryme.top

Ruby: exit 1
来源：http://iue.svipenyu.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://vlq.yuxming.cn

[M06] 向标准错误输出
来源：http://cyv.gaohongyu789.top

Py:   print("err", file=sys.stderr)
来源：http://nfs.zhoulong.xyz

PHP:  fwrite(STDERR, "err\n");
来源：http://muj.yanxiufei.cn

JS:   console.error("err")
来源：http://aiq.sufxvd.cn

TS:   console.error("err")
来源：http://ftm.yj202588.top

Java: System.err.println("err")
来源：http://ywl.cheryme.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://aer.jinghuilouyu.cn

Ruby: warn "err"
来源：http://ony.fanxiaobao.xyz

C#:   Console.Error.WriteLine("err")
来源：http://kpd.aizwys.cn

[M07] 判断是否为主入口
来源：http://gzd.iojbl.cn

Py:   if __name__ == "__main__":
来源：http://wba.jinyuanbaomall.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://qab.gotoacloud.top

JS:   require.main === module
来源：http://php.tanke756.top

TS:   require.main === module
来源：http://lcd.hcnkem.com

Java: public static void main(String[] args)
来源：http://nqx.yueranfly.top

Go:   func main()
来源：http://rif.zhoulong.xyz

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://jhu.zhoulong.xyz

C#:   static void Main(string[] args)
来源：http://mls.ivvv.top

[M08] 获取系统与运行时信息
来源：http://vhh.ctjpmb.com

Py:   platform.system();  platform.python_version()
来源：http://nfv.gaohongyu789.top

PHP:  PHP_OS;  phpversion();
来源：http://wzw.sweek.top

JS:   process.platform;  process.version
来源：http://dsw.daxiang520.top

TS:   process.platform;  process.version
来源：http://qii.chenzaomai.com

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ggf.gotoacloud.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://ieg.quarkkingdee.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://vmh.daxiang520.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://bhz.sufxvd.cn

================================================================================
来源：http://nyq.haohaochexian.top

N. 数据结构与算法
来源：http://vrc.fzhhl.top

================================================================================
来源：http://fcz.gogol.net.cn

[N01] 二分查找（有序数组）
来源：http://ozx.sjlbkw.cn

Py:   bisect.bisect_left(arr, x)
来源：http://oqt.gotoacloud.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://qkk.guannengcc.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://tjd.xinyue.icu

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://vgz.bjfxy.top

Java: Arrays.binarySearch(arr, x)
来源：http://bis.wangshuangyany.cn

Go:   sort.SearchInts(arr, x)
来源：http://sog.cucudq.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://vnm.yueranfly.top

C#:   Array.BinarySearch(arr, x)
来源：http://jso.hcnkem.com

[N02] 排序（工程实践用内置实现）
来源：http://ank.gaohongyu789.top

Py:   sorted(arr);  arr.sort()
来源：http://bkt.jqgfzy.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://cru.jinqigfzy.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://lmq.redwolf501.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://wgi.fktsv.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://xms.guannengcc.top

Go:   slices.Sort(arr)
来源：http://pca.jinqigufen.top

Ruby: arr.sort
来源：http://yqq.shzxlz.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://yqs.uphjek.com

[N03] 快速排序（分治示例）
来源：http://wss.cucudq.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://web.gotoacloud.top

PHP:  // 递归实现，或用 usort
来源：http://mvh.ydjk.org.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wbb.jlsjyb.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://tfw.bjfxy.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ogs.fzhhl.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://alk.redwolf501.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://gau.tianlin.xyz

C#:   // 手写递归，或 Array.Sort
来源：http://eyx.dianchejie.cn

[N04] 斐波那契数列
来源：http://evb.dashuyun.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hqb.guowangkeji.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://odm.cdnleiting.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://xfk.guowangkeji.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://sko.nanxuanxn.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://tiq.guannengcc.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://xwy.aibaodan.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://pky.kuanghao11.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ibx.cdnleiting.top

[N05] 最大公约数
来源：http://zcu.jyoumei.cn

Py:   math.gcd(a, b)
来源：http://hsl.hongshengwenyu.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://kip.wangshuangyany.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://jmx.hammf.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://dev.jinqigufen.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://aui.hnqzz.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://lre.zhixingplan.top

Ruby: a.gcd(b)
来源：http://pjr.uphjek.com

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wkr.c1oappe.top

[N06] 判断回文字符串
来源：http://rel.wangdashe.top

Py:   s == s[::-1]
来源：http://qej.redwolf501.top

PHP:  $s === strrev($s);
来源：http://mgc.jianghu66.top


<!-- 参考信息 -->