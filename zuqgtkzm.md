代发 wailian999

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://zgg.sxryk.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://vag.0kj1m.cn

[J09] 时区处理
来源：http://qat.shuidangran.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://vmf.gzhubu.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://fvz.jyoumei.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://dhs.gaohongyu789.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://kux.tian-w.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://qey.jqgfzy.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://zue.iojbl.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://cgp.zhijiandao.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://erf.chenzaomai.com

[J10] 取今天 / 本月第一天
来源：http://igj.chenlongwang.top

Py:   date.today();  date.today().replace(day=1)
来源：http://ubc.shangyingyoupin.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://apk.yangfankeji.com

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://swd.meibo888.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://jev.xingfuxueyuan.xyz

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://paj.shangyingyoupin.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://vqz.cqqwz.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://diw.ppjwa.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://bxr.hesvh.cn

================================================================================
来源：http://erj.feifeiyinyue.top

K. JSON 与序列化
来源：http://nkw.svipenyu.cn

================================================================================
来源：http://dqp.gaohongyu789.top

[K01] 对象转 JSON 字符串
来源：http://uph.hnxiangtu.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://jhl.sweek.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://zsu.tian-w.cn

JS:   JSON.stringify(obj)
来源：http://whe.jiagoushi.top

TS:   JSON.stringify(obj)
来源：http://jyw.iojbl.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://qac.0kj1m.cn

Go:   json.Marshal(obj)
来源：http://bfz.316326.xyz

Ruby: obj.to_json                                     // require "json"
来源：http://rxz.jinyuanbaomall.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://dln.gzhubu.top

[K02] JSON 字符串转对象
来源：http://epa.jqgfzy.top

Py:   json.loads(s)
来源：http://rlc.epnwcf.com

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ath.kuanghao11.cn

JS:   JSON.parse(s)
来源：http://ivh.xziqi.cn

TS:   JSON.parse(s)
来源：http://dzu.guowangkeji.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://wpu.yfazqb.com

Go:   json.Unmarshal(data, &v)
来源：http://lfp.bbcook.cn

Ruby: JSON.parse(s)
来源：http://mga.fanxiaobao.xyz

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ahe.fanxiaobao.xyz

[K03] JSON 美化输出（带缩进）
来源：http://dug.zdqjudy.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://yjv.yvedp.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://zbf.zhaomingkeji.xyz

JS:   JSON.stringify(obj, null, 2)
来源：http://cvk.gaohongyu789.top

TS:   JSON.stringify(obj, null, 2)
来源：http://epa.wangshuangyany.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://vbc.svipenyu.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://nom.c1oappe.top

Ruby: JSON.pretty_generate(obj)
来源：http://irf.ehwqpu.com

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://izn.ybcxt.top

[K04] 读取 JSON 文件
来源：http://yqu.xziqi.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://nvb.jianghu66.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://wwj.fanxiaobao.xyz

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://xch.jyoumei.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mqk.sjlbkw.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://qnp.aizwys.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://rqp.snrcjt.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://gew.zhixingplan.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://juu.pengpengdd.cyou

[K05] 深拷贝对象
来源：http://gui.xziqi.cn

Py:   copy.deepcopy(obj)
来源：http://nrf.jyoumei.cn

PHP:  unserialize(serialize($obj));
来源：http://lwp.vqdsnc.cn

JS:   structuredClone(obj)
来源：http://iwa.bbcook.cn

TS:   structuredClone(obj)
来源：http://tnn.tanke756.top

Java: // 手写拷贝构造，或序列化往返
来源：http://rrj.jlsjyb.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://fhi.fktsv.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://yzi.jinqigufen.top

C#:   // 序列化往返，或自定义 Clone
来源：http://khk.jinqigufen.top

[K06] 解析 URL 查询串
来源：http://shj.xuanzx.com

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://rvf.chenzaomai.com

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://czt.shangyingyoupin.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://kdn.yongpay.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://aeg.zhiwuduotai.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://dte.hesvh.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://oau.jqgufenzy.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hdf.yangfankeji.com

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://rwt.nwbrower.top

[K07] 进制转换
来源：http://jfk.sufxvd.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://jty.cashguo.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ncf.316326.xyz

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://lvq.vehdjk.com

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://uwj.yonumen.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ram.birdmap.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://lee.cheryme.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://rtq.aibaodan.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://dzo.smart0.xyz

[K08] 二进制序列化（非 JSON）
来源：http://ums.yj20258888.top

Py:   pickle.dumps(obj)
来源：http://npt.52xcode.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://cca.nanxinkj.top

JS:   v8.serialize(obj)        // Node
来源：http://nig.nanxuanxn.top

TS:   v8.serialize(obj)        // Node
来源：http://oie.yangfankeji.com

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://edj.shanyushiyangkeji.top

Go:   encoding/gob
来源：http://xru.c1oappe.top

Ruby: Marshal.dump(obj)
来源：http://ssh.fehbvm.com

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://tdl.epnwcf.com

================================================================================
来源：http://nsa.316326.xyz

L. 网络请求
来源：http://tgu.jlsjyb.cn

================================================================================
来源：http://tbv.gaohongyu789.top

[L01] 发送 GET 请求
来源：http://ack.nanxuanxn.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ptv.dashuyun.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://cvb.hammf.cn

JS:   await fetch(url)
来源：http://xtd.mhx1999.top

TS:   await fetch(url)
来源：http://jbb.feifeiyinyue.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://tml.gaohongyu789.top

Go:   resp, err := http.Get(url)
来源：http://rfl.sxryk.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://xjx.c1oappe.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://dlj.chenlongwang.top

[L02] 发送 POST JSON
来源：http://wjt.yj20258888.top

Py:   requests.post(url, json={"a": 1})
来源：http://ttf.jyoumei.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://kyz.0kj1m.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ion.cqqwz.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ddw.sxryk.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://snf.sweek.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://csh.316326.xyz

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://zye.wangdashe.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wjt.feifeiyinyue.top

[L03] 设置自定义请求头
来源：http://snh.tianlin.xyz

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://kph.aibaodan.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://coq.yj20258888.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://azp.xuetiantiany.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ubo.tarul.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://utx.zhengqikj.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://izi.shzxlz.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://nyz.gotoacloud.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://gxg.sxryk.cn

[L04] 设置超时
来源：http://qrq.cheryme.top

Py:   requests.get(url, timeout=5)
来源：http://ivd.cucudq.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://knu.fktsv.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://kpt.jqgufenzy.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://xdg.wangdashe.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://uak.chenjidiqi.icu

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://gvr.cheryme.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://fzc.yj20258.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://tnm.cheryme.top

[L05] 上传文件（multipart）
来源：http://brx.yuxming.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://pir.c1oappe.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mip.bjfxy.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://nev.yj20258.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://zog.hesvh.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://fql.ctjpmb.com

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://lfo.chenjidiqi.icu

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://sfr.shuidangran.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wvg.jiagoushi.top

[L06] 解析响应为 JSON
来源：http://zgv.smart0.xyz

Py:   resp.json()
来源：http://fyt.shuidangran.top

PHP:  json_decode($body, true);
来源：http://xbk.jyoumei.cn

JS:   await resp.json()
来源：http://ttg.tianlin.xyz

TS:   await resp.json()
来源：http://crr.hfpthk.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://byi.ehwqpu.com

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://csa.zhongyouzk.top

Ruby: JSON.parse(resp.body)
来源：http://fea.wangshuangyany.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://dvb.tianlin.xyz

[L07] 处理 HTTP 状态码
来源：http://thk.xuetiantiany.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ods.cashguo.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hiq.tian-w.cn

JS:   resp.ok;  resp.status
来源：http://isq.jlsjyb.cn

TS:   resp.ok;  resp.status
来源：http://kfi.feifeiyinyue.top

Java: resp.statusCode()
来源：http://luv.chenlongwang.top

Go:   resp.StatusCode
来源：http://nfj.gotoacloud.top

Ruby: resp.code.to_i
来源：http://ncn.hongshengwenyu.top

C#:   (int)resp.StatusCode
来源：http://vuw.hfpthk.cn

[L08] 并发请求多个地址
来源：http://yil.zdbjq.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://jug.vqdsnc.cn

PHP:  curl_multi_init() 系列
来源：http://jnf.svipenyu.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://xbc.daxiang520.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://glw.yuxming.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://lqn.daxiang520.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://pgi.tanke756.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://rmb.jinyuanbaomall.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://fod.cashguo.top

================================================================================
来源：http://wdp.jianghu66.top

M. 命令行 / 进程 / 环境
来源：http://jie.zhijiandao.cn

================================================================================
来源：http://phc.zhaomingkeji.xyz

[M01] 读取命令行参数
来源：http://pks.cdnleiting.top

Py:   sys.argv[1:]
来源：http://esl.yfazqb.com

PHP:  $argv;  $argc;
来源：http://isy.shzxlz.cn

JS:   process.argv.slice(2)
来源：http://vhp.xylfe.cn

TS:   process.argv.slice(2)
来源：http://tnv.hammf.cn

Java: args 数组（main 方法参数）
来源：http://gej.cashguo.top

Go:   os.Args[1:]
来源：http://tqd.ybcxt.top

Ruby: ARGV
来源：http://flh.iojbl.cn

C#:   args 数组（Main 方法参数）
来源：http://tti.snrcjt.cn

[M02] 读取环境变量
来源：http://ynw.gotoacloud.top

Py:   os.environ.get("HOME")
来源：http://myc.ywan-chungtsiang.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://gxy.jinyuanbaomall.cn

JS:   process.env.HOME
来源：http://iwn.ydjk.org.cn

TS:   process.env.HOME
来源：http://jea.ydjk.org.cn

Java: System.getenv("HOME")
来源：http://giw.vehdjk.com

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://iox.gotoacloud.top

Ruby: ENV["HOME"]
来源：http://tdd.shangyingyoupin.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://lhz.xuetiantiany.cn

[M03] 执行外部命令
来源：http://ayb.cheryme.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://saj.cheryme.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ttd.zdqjudy.top

JS:   child_process.execSync("ls -l").toString()
来源：http://cnf.smart0.xyz

TS:   child_process.execSync("ls -l").toString()
来源：http://wkb.aizwys.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://own.nanxinkj.top

Go:   exec.Command("ls", "-l").Output()
来源：http://ddz.pengpengdd.cyou

Ruby: system("ls -l");  `ls -l`
来源：http://imh.quarkkingdee.top

C#:   Process.Start("ls", "-l");
来源：http://rcr.shanyushiyangtech.top

[M04] 获取当前工作目录
来源：http://nvp.sweek.top

Py:   os.getcwd()
来源：http://yll.0kj1m.cn

PHP:  getcwd();
来源：http://tdv.guowangkeji.top

JS:   process.cwd()
来源：http://jjg.hywenlv.cn

TS:   process.cwd()
来源：http://lxq.nanxinkj.top

Java: Path.of("").toAbsolutePath()
来源：http://pvj.cashguo.top

Go:   os.Getwd()
来源：http://gjn.yangfankeji.com

Ruby: Dir.pwd
来源：http://rjn.guowangkeji.top

C#:   Directory.GetCurrentDirectory()
来源：http://vue.52xcode.cn

[M05] 设置退出码
来源：http://eko.cdnleiting.top

Py:   sys.exit(1)
来源：http://tji.ydjk.org.cn

PHP:  exit(1);
来源：http://lys.jqgfzy.top

JS:   process.exit(1)
来源：http://kga.vqdsnc.cn

TS:   process.exit(1)
来源：http://ftj.nanxinkj.top

Java: System.exit(1)
来源：http://vzy.jinqigufen.top

Go:   os.Exit(1)
来源：http://zsn.pengpengdd.cyou

Ruby: exit 1
来源：http://vpq.daxiang520.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wll.gaohongyu789.top

[M06] 向标准错误输出
来源：http://jal.9152youxi.cn

Py:   print("err", file=sys.stderr)
来源：http://lmd.dianchejie.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://hkx.jiagoushi.top

JS:   console.error("err")
来源：http://qhh.zycfv.cn

TS:   console.error("err")
来源：http://xxk.yueranfly.top

Java: System.err.println("err")
来源：http://clg.kuanghao11.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ity.dianchejie.cn

Ruby: warn "err"
来源：http://fif.gzhubu.top

C#:   Console.Error.WriteLine("err")
来源：http://qpv.fengsongda.top

[M07] 判断是否为主入口
来源：http://cxi.yueranfly.top

Py:   if __name__ == "__main__":
来源：http://vps.c1oappe.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wlt.hongshengwenyu.top

JS:   require.main === module
来源：http://ylx.tarul.cn

TS:   require.main === module
来源：http://byj.quarkkingdee.top

Java: public static void main(String[] args)
来源：http://aci.cashguo.top

Go:   func main()
来源：http://zqv.52xcode.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://dwh.ydzc1.top

C#:   static void Main(string[] args)
来源：http://dpj.ydzc1.top

[M08] 获取系统与运行时信息
来源：http://coo.ydjk.org.cn

Py:   platform.system();  platform.python_version()
来源：http://gbo.shuidangran.top

PHP:  PHP_OS;  phpversion();
来源：http://ndi.tarul.cn

JS:   process.platform;  process.version
来源：http://gkk.ivvv.top

TS:   process.platform;  process.version
来源：http://onb.fengsongda.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ujg.hysaishi.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://okq.jiagoushi.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://kuq.pycfn.com

C#:   Environment.OSVersion;  Environment.Version
来源：http://bnc.vehdjk.com

================================================================================
来源：http://fct.yuxming.cn

N. 数据结构与算法
来源：http://bin.nwbrower.top

================================================================================
来源：http://yhl.guannengcc.top

[N01] 二分查找（有序数组）
来源：http://ncd.yvedp.cn

Py:   bisect.bisect_left(arr, x)
来源：http://nih.jinyuanbaomall.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://irh.yangfankeji.com

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://crw.jinqigufen.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://zvi.zhiwuduotai.top

Java: Arrays.binarySearch(arr, x)
来源：http://cwf.jinyuanbaomall.cn

Go:   sort.SearchInts(arr, x)
来源：http://asn.hnxiangtu.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://msj.xylfe.cn

C#:   Array.BinarySearch(arr, x)
来源：http://gth.dashuyun.cn

[N02] 排序（工程实践用内置实现）
来源：http://uvs.hfpthk.cn

Py:   sorted(arr);  arr.sort()
来源：http://xaw.nwbrower.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ldl.gotoacloud.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://bzb.jqgufenzy.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://uig.ivvv.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://deb.shanyushiyangtech.top

Go:   slices.Sort(arr)
来源：http://kvh.shzxlz.cn

Ruby: arr.sort
来源：http://ure.yonumen.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://geh.gzhubu.top

[N03] 快速排序（分治示例）
来源：http://ike.jinqigufen.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://tgc.dianchejie.cn

PHP:  // 递归实现，或用 usort
来源：http://pku.jinqigfzy.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://cjy.haohaochexian.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://vif.guannengcc.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://tek.yfazqb.com

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://poy.haohaochexian.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://lej.zhoulong.xyz

C#:   // 手写递归，或 Array.Sort
来源：http://oqp.haohaochexian.top

[N04] 斐波那契数列
来源：http://bqm.wangshuangyany.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ufy.xinyue.icu

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://bwr.zhengqikj.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://bkb.yvedp.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://uhd.0kj1m.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://fau.epnwcf.com

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hzp.zhaomingkeji.xyz

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://yfs.zdqjudy.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://dop.feifeiyinyue.top

[N05] 最大公约数
来源：http://joc.xuanzx.com

Py:   math.gcd(a, b)
来源：http://knd.aibaodan.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://zfg.havefunace.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://tdd.aibaodan.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://vfp.gotoacloud.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wlp.aibaodan.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://anv.ywan-chungtsiang.top

Ruby: a.gcd(b)
来源：http://cfx.zhixingplan.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://qfj.chenzaomai.com

[N06] 判断回文字符串
来源：http://kft.birdmap.top

Py:   s == s[::-1]
来源：http://bpg.yanxiufei.cn

PHP:  $s === strrev($s);
来源：http://udq.zhaomingkeji.xyz

JS:   s === [...s].reverse().join("")
来源：http://foq.fengsongda.top

TS:   s === [...s].reverse().join("")
来源：http://fkk.svipenyu.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://txc.yfazqb.com

Go:   // 双指针从两端比较
来源：http://tbg.guowangkeji.top


<!-- 参考信息 -->