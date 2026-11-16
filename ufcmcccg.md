代发 wailian999

C#:   d1 < d2;  d1 == d2
来源：http://mka.birdmap.top

[J08] 提取年月日与星期
来源：http://xrz.sjlbkw.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://dlq.zhengqikj.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://caz.ehwqpu.com

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://zwz.xuanzx.com

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://azw.fanxiaobao.xyz

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hnx.yj202588.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://vsp.fengsongda.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://pie.yonumen.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ogp.hcnkem.com

[J09] 时区处理
来源：http://ihu.yonumen.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://zho.zycfv.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://kqj.bbcook.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://bqk.shangyingyoupin.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://qje.zhixingplan.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://brh.ydzc1.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://zuf.fengsongda.top

Ruby: Time.now.getlocal("+08:00")
来源：http://teu.yangfankeji.com

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ypz.gaohongyu789.top

[J10] 取今天 / 本月第一天
来源：http://jwp.hesvh.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://xpq.pengpengdd.cyou

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://rer.kuanghao11.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://zqz.fengsongda.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ahe.uphjek.com

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://dvb.fehbvm.com

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://jcn.nanxuanxn.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ssq.zhengqikj.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://wnx.hnxiangtu.top

================================================================================
来源：http://iqc.gaohongyu789.top

K. JSON 与序列化
来源：http://ffy.hnxiangtu.top

================================================================================
来源：http://yft.redwolf501.top

[K01] 对象转 JSON 字符串
来源：http://xws.guowangkeji.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://eaw.yongpay.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://vnp.ydjk.org.cn

JS:   JSON.stringify(obj)
来源：http://mal.fengsongda.top

TS:   JSON.stringify(obj)
来源：http://ewx.gotoacloud.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://wyv.kuanghao11.cn

Go:   json.Marshal(obj)
来源：http://qog.fanxiaobao.xyz

Ruby: obj.to_json                                     // require "json"
来源：http://scf.fanxiaobao.xyz

C#:   JsonSerializer.Serialize(obj)
来源：http://wwr.cashguo.top

[K02] JSON 字符串转对象
来源：http://kfa.yj20258888.top

Py:   json.loads(s)
来源：http://ihr.cdnleiting.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://lin.xuetiantiany.cn

JS:   JSON.parse(s)
来源：http://jli.fengsongda.top

TS:   JSON.parse(s)
来源：http://fkf.zhengqikj.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://fvr.9152youxi.cn

Go:   json.Unmarshal(data, &v)
来源：http://nrn.yj202588.top

Ruby: JSON.parse(s)
来源：http://qxy.0kj1m.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://lfl.fehbvm.com

[K03] JSON 美化输出（带缩进）
来源：http://zbk.yangfankeji.com

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://zht.zhijiandao.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://mjy.aibaodan.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://iqx.sjlbkw.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://env.fehbvm.com

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://enz.hcnkem.com

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://jaz.vehdjk.com

Ruby: JSON.pretty_generate(obj)
来源：http://wev.ywan-chungtsiang.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://jqx.sysykeji.top

[K04] 读取 JSON 文件
来源：http://xxv.chenlongwang.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://uqk.jiagoushi.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://oun.bbcook.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ega.fzhhl.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mfa.52xcode.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://nkx.zycfv.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hef.aibaodan.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://eoq.yj202588.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://buy.c1oappe.top

[K05] 深拷贝对象
来源：http://fzd.pengpengdd.cyou

Py:   copy.deepcopy(obj)
来源：http://mta.aizwys.cn

PHP:  unserialize(serialize($obj));
来源：http://tdt.tian-w.cn

JS:   structuredClone(obj)
来源：http://rez.nwbrower.top

TS:   structuredClone(obj)
来源：http://dlv.cheryme.top

Java: // 手写拷贝构造，或序列化往返
来源：http://psw.aibaodan.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://lny.xingfuxueyuan.xyz

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://uza.fktsv.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://zyp.yj202588.top

[K06] 解析 URL 查询串
来源：http://ftn.wangdashe.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://iql.zhoulong.xyz

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://dzv.shanyushiyangkeji.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wyl.yueranfly.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hvx.fengsongda.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://tvp.tanke756.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://tfy.aibaodan.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://qdt.haohaochexian.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://opu.zhengqikj.top

[K07] 进制转换
来源：http://vkc.52xcode.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://dti.hnqzz.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://gpp.svipenyu.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://anp.pycfn.com

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://plv.hywenlv.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://sjf.snrcjt.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://raf.birdmap.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://pyu.hywenlv.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wkn.cqqwz.cn

[K08] 二进制序列化（非 JSON）
来源：http://hzx.jinghuilouyu.cn

Py:   pickle.dumps(obj)
来源：http://xbg.hywenlv.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://jmp.jiagoushi.top

JS:   v8.serialize(obj)        // Node
来源：http://ljg.ydzc1.top

TS:   v8.serialize(obj)        // Node
来源：http://llg.tian-w.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://zfr.sjlbkw.cn

Go:   encoding/gob
来源：http://lcl.yuanzhike.top

Ruby: Marshal.dump(obj)
来源：http://hyp.316326.xyz

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ecs.dashuyun.cn

================================================================================
来源：http://gus.ydzc1.top

L. 网络请求
来源：http://bbg.52xcode.cn

================================================================================
来源：http://bpt.zdbjq.cn

[L01] 发送 GET 请求
来源：http://oxi.9152youxi.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://zfe.fanxiaobao.xyz

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://abx.snrcjt.cn

JS:   await fetch(url)
来源：http://gis.0kj1m.cn

TS:   await fetch(url)
来源：http://ptu.hnqzz.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://cya.tian-w.cn

Go:   resp, err := http.Get(url)
来源：http://uxj.guowangkeji.top

Ruby: Net::HTTP.get(URI(url))
来源：http://wvj.hesvh.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://efz.fzhhl.top

[L02] 发送 POST JSON
来源：http://yxu.vqdsnc.cn

Py:   requests.post(url, json={"a": 1})
来源：http://nwj.shanyushiyangtech.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://dmu.dianchejie.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://jrp.nwbrower.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://rnt.sjlbkw.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://udi.nwbrower.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ekl.iojbl.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wsm.epnwcf.com

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ain.nanxinkj.top

[L03] 设置自定义请求头
来源：http://rfm.hammf.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hya.jqgfzy.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hoi.yonumen.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://xco.shzxlz.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ihl.zdqjudy.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://nkx.cdnleiting.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://rxt.sweek.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://vwe.jyoumei.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://sto.wangdashe.top

[L04] 设置超时
来源：http://jxi.daxiang520.top

Py:   requests.get(url, timeout=5)
来源：http://qqn.hesvh.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://cmd.nanxinkj.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://jgh.cheryme.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://lfr.gotoacloud.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://lch.yfazqb.com

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://qtn.xuanzx.com

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://eof.mhx1999.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hpg.yj202588.top

[L05] 上传文件（multipart）
来源：http://qoe.hcnkem.com

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://krd.nanxuanxn.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://orq.tian-w.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://uzh.yuxming.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://orc.vqdsnc.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://erh.hnxiangtu.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://zal.hammf.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hyb.xuanzx.com

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://yma.316326.xyz

[L06] 解析响应为 JSON
来源：http://bpw.ybcxt.top

Py:   resp.json()
来源：http://feq.ivvv.top

PHP:  json_decode($body, true);
来源：http://uaw.svipenyu.cn

JS:   await resp.json()
来源：http://tix.redwolf501.top

TS:   await resp.json()
来源：http://evh.fanxiaobao.xyz

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://vbe.jqgfzy.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ucs.fzhhl.top

Ruby: JSON.parse(resp.body)
来源：http://tgu.zhongyouzk.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://waq.epnwcf.com

[L07] 处理 HTTP 状态码
来源：http://qle.tarul.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://bxr.jqgufenzy.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://odb.gogol.net.cn

JS:   resp.ok;  resp.status
来源：http://zpj.tianlin.xyz

TS:   resp.ok;  resp.status
来源：http://jte.fktsv.cn

Java: resp.statusCode()
来源：http://ekf.jianghu66.top

Go:   resp.StatusCode
来源：http://zuw.nanxinkj.top

Ruby: resp.code.to_i
来源：http://lmr.snrcjt.cn

C#:   (int)resp.StatusCode
来源：http://zal.smart0.xyz

[L08] 并发请求多个地址
来源：http://agh.havefunace.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mfu.sxryk.cn

PHP:  curl_multi_init() 系列
来源：http://gbs.zhongyouzk.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://vop.jqgufenzy.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://dfz.yvedp.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://zqs.hywenlv.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://tfz.fktsv.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wno.ywan-chungtsiang.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://kzx.birdmap.top

================================================================================
来源：http://zby.shanyushiyangtech.top

M. 命令行 / 进程 / 环境
来源：http://ubr.hongshengwenyu.top

================================================================================
来源：http://hik.hfpthk.cn

[M01] 读取命令行参数
来源：http://tqv.cdnleiting.top

Py:   sys.argv[1:]
来源：http://vzx.meibo888.top

PHP:  $argv;  $argc;
来源：http://sws.guowangkeji.top

JS:   process.argv.slice(2)
来源：http://bpl.svipenyu.cn

TS:   process.argv.slice(2)
来源：http://edd.hammf.cn

Java: args 数组（main 方法参数）
来源：http://ayj.feifeiyinyue.top

Go:   os.Args[1:]
来源：http://thn.jinyuanbaomall.cn

Ruby: ARGV
来源：http://flk.sxryk.cn

C#:   args 数组（Main 方法参数）
来源：http://crb.bbcook.cn

[M02] 读取环境变量
来源：http://xpe.sufxvd.cn

Py:   os.environ.get("HOME")
来源：http://olg.cheryme.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ezc.sweek.top

JS:   process.env.HOME
来源：http://iix.hfpthk.cn

TS:   process.env.HOME
来源：http://qgf.316326.xyz

Java: System.getenv("HOME")
来源：http://fgp.yueranfly.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://fxi.xinyue.icu

Ruby: ENV["HOME"]
来源：http://ooa.hnxiangtu.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://lyy.fzhhl.top

[M03] 执行外部命令
来源：http://ihy.yvedp.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://rpq.nanxuanxn.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://gyb.redwolf501.top

JS:   child_process.execSync("ls -l").toString()
来源：http://xhe.dashuyun.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://jew.nanxuanxn.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://sao.yonumen.top

Go:   exec.Command("ls", "-l").Output()
来源：http://yux.xuetiantiany.cn

Ruby: system("ls -l");  `ls -l`
来源：http://zks.nwbrower.top

C#:   Process.Start("ls", "-l");
来源：http://bar.snrcjt.cn

[M04] 获取当前工作目录
来源：http://wkx.aizwys.cn

Py:   os.getcwd()
来源：http://uhs.xinyue.icu

PHP:  getcwd();
来源：http://der.yangfankeji.com

JS:   process.cwd()
来源：http://dry.mhx1999.top

TS:   process.cwd()
来源：http://szs.tianlin.xyz

Java: Path.of("").toAbsolutePath()
来源：http://mim.xuetiantiany.cn

Go:   os.Getwd()
来源：http://kwi.nanxuanxn.top

Ruby: Dir.pwd
来源：http://eir.sufxvd.cn

C#:   Directory.GetCurrentDirectory()
来源：http://rum.ydjk.org.cn

[M05] 设置退出码
来源：http://jxk.kuanghao11.cn

Py:   sys.exit(1)
来源：http://vhv.zhongyouzk.top

PHP:  exit(1);
来源：http://hgz.shanyushiyangtech.top

JS:   process.exit(1)
来源：http://nqo.hfpthk.cn

TS:   process.exit(1)
来源：http://mqh.yongpay.top

Java: System.exit(1)
来源：http://zsb.yj20258888.top

Go:   os.Exit(1)
来源：http://jmx.yueranfly.top

Ruby: exit 1
来源：http://ynh.uphjek.com

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ubj.gotoacloud.top

[M06] 向标准错误输出
来源：http://utw.hnqzz.top

Py:   print("err", file=sys.stderr)
来源：http://odl.svipenyu.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://kmj.feifeiyinyue.top

JS:   console.error("err")
来源：http://eqe.fanxiaobao.xyz

TS:   console.error("err")
来源：http://kmz.316326.xyz

Java: System.err.println("err")
来源：http://cmo.shanyushiyangtech.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mqh.svipenyu.cn

Ruby: warn "err"
来源：http://osl.sxryk.cn

C#:   Console.Error.WriteLine("err")
来源：http://cyx.316326.xyz

[M07] 判断是否为主入口
来源：http://wps.dashuyun.cn

Py:   if __name__ == "__main__":
来源：http://ppo.nanxinkj.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ije.zycfv.cn

JS:   require.main === module
来源：http://xzy.hesvh.cn

TS:   require.main === module
来源：http://knb.aibaodan.cn

Java: public static void main(String[] args)
来源：http://uqx.dianchejie.cn

Go:   func main()
来源：http://fgb.gaohongyu789.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://dyx.0kj1m.cn

C#:   static void Main(string[] args)
来源：http://dkf.fehbvm.com

[M08] 获取系统与运行时信息
来源：http://num.jianghu66.top

Py:   platform.system();  platform.python_version()
来源：http://dmw.nanxuanxn.top

PHP:  PHP_OS;  phpversion();
来源：http://qjg.jinyuanbaomall.cn

JS:   process.platform;  process.version
来源：http://kat.hfpthk.cn

TS:   process.platform;  process.version
来源：http://pnb.tianlin.xyz

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://shj.nanxinkj.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://cxl.kuanghao11.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://apd.zhengqikj.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://uxw.tarul.cn

================================================================================
来源：http://usf.zhaomingkeji.xyz

N. 数据结构与算法
来源：http://tpz.chenlongwang.top

================================================================================
来源：http://njn.zhaomingkeji.xyz

[N01] 二分查找（有序数组）
来源：http://rdt.xuanzx.com

Py:   bisect.bisect_left(arr, x)
来源：http://wgy.shanyushiyangtech.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://nog.zhiwuduotai.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://zhj.hfpthk.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://qtg.yfazqb.com

Java: Arrays.binarySearch(arr, x)
来源：http://ohq.gotoacloud.top

Go:   sort.SearchInts(arr, x)
来源：http://tod.ybcxt.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://uea.fzhhl.top

C#:   Array.BinarySearch(arr, x)
来源：http://uno.cashguo.top

[N02] 排序（工程实践用内置实现）
来源：http://lus.tarul.cn

Py:   sorted(arr);  arr.sort()
来源：http://aif.xingfuxueyuan.xyz

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://kvv.hfpthk.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://qpe.zhijiandao.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://tic.sysykeji.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://jyn.quarkkingdee.top

Go:   slices.Sort(arr)
来源：http://xpv.hcnkem.com

Ruby: arr.sort
来源：http://mok.chenzaomai.com

C#:   Array.Sort(arr);  list.Sort()
来源：http://lrr.zhongyouzk.top

[N03] 快速排序（分治示例）
来源：http://dib.jqgufenzy.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ggn.ydjk.org.cn

PHP:  // 递归实现，或用 usort
来源：http://ixc.sjlbkw.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://xuu.ppjwa.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://zyc.smart0.xyz

Java: // 手写递归，或直接用 Arrays.sort
来源：http://rnt.hfpthk.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hoc.ydjk.org.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://qgh.aizwys.cn

C#:   // 手写递归，或 Array.Sort
来源：http://zrn.sufxvd.cn

[N04] 斐波那契数列
来源：http://dqm.jqgfzy.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://zvq.yj20258.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://jdo.xinyue.icu

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ump.jiagoushi.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://gzv.gzhubu.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://xsf.snrcjt.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://oyf.tarul.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://fre.nwbrower.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://emv.nwbrower.top

[N05] 最大公约数
来源：http://aaj.bbcook.cn

Py:   math.gcd(a, b)
来源：http://wno.uphjek.com

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://dyg.havefunace.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://bgn.gzhubu.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://rwj.ydjk.org.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://nub.316326.xyz

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ykx.hammf.cn

Ruby: a.gcd(b)
来源：http://tug.fzhhl.top


<!-- 参考信息 -->