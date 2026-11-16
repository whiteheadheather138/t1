代发 wailian999

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://kyf.dianchejie.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://yqh.ybcxt.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://eaz.haohaochexian.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://byn.yuxming.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://zsy.jiagoushi.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ytb.zhengqikj.top

[J09] 时区处理
来源：http://kcy.yangfankeji.com

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://syk.yj20258888.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ceg.fengsongda.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://svu.daria6918.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://cps.fzhhl.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://qpf.zdqjudy.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ayv.yongpay.top

Ruby: Time.now.getlocal("+08:00")
来源：http://ghf.fanxiaobao.xyz

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://wzj.yj202588.top

[J10] 取今天 / 本月第一天
来源：http://zwk.chenjidiqi.icu

Py:   date.today();  date.today().replace(day=1)
来源：http://xpm.aibaodan.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://gvm.shangyingyoupin.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://rkw.yueranfly.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://fgh.epnwcf.com

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://xrj.hammf.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://usx.sjlbkw.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://vlt.ivvv.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://huj.yj202588.top

================================================================================
来源：http://neq.svipenyu.cn

K. JSON 与序列化
来源：http://lmu.smart0.xyz

================================================================================
来源：http://iti.hongshengwenyu.top

[K01] 对象转 JSON 字符串
来源：http://kdy.sysykeji.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://dfj.yanxiufei.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://cnz.yueranfly.top

JS:   JSON.stringify(obj)
来源：http://ggh.hongshengwenyu.top

TS:   JSON.stringify(obj)
来源：http://lwl.chenlongwang.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://fdh.yvedp.cn

Go:   json.Marshal(obj)
来源：http://hsz.jinyuanbaomall.cn

Ruby: obj.to_json                                     // require "json"
来源：http://qvx.meibo888.top

C#:   JsonSerializer.Serialize(obj)
来源：http://qqd.fengsongda.top

[K02] JSON 字符串转对象
来源：http://gbc.zhijiandao.cn

Py:   json.loads(s)
来源：http://ono.jqgufenzy.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://iyq.cucudq.cn

JS:   JSON.parse(s)
来源：http://nqg.zdbjq.cn

TS:   JSON.parse(s)
来源：http://lus.snrcjt.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://zil.mhx1999.top

Go:   json.Unmarshal(data, &v)
来源：http://uml.9152youxi.cn

Ruby: JSON.parse(s)
来源：http://iys.ivvv.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://tak.wangshuangyany.cn

[K03] JSON 美化输出（带缩进）
来源：http://ogn.zhixingplan.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://zvu.tarul.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://rfn.xuetiantiany.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://qfx.ydjk.org.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://hzn.xingfuxueyuan.xyz

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hrq.ivvv.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://nmk.xuetiantiany.cn

Ruby: JSON.pretty_generate(obj)
来源：http://nps.sxryk.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://uyo.epnwcf.com

[K04] 读取 JSON 文件
来源：http://zcw.52xcode.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://iex.fanxiaobao.xyz

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://utf.cashguo.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://dvg.aizwys.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://pyu.haohaochexian.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://btd.quarkkingdee.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://faq.hongshengwenyu.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://xjz.sjlbkw.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://pup.zhixingplan.top

[K05] 深拷贝对象
来源：http://ddb.bbcook.cn

Py:   copy.deepcopy(obj)
来源：http://nqz.dashuyun.cn

PHP:  unserialize(serialize($obj));
来源：http://ync.guowangkeji.top

JS:   structuredClone(obj)
来源：http://wef.zhaomingkeji.xyz

TS:   structuredClone(obj)
来源：http://vhl.zhoulong.xyz

Java: // 手写拷贝构造，或序列化往返
来源：http://amz.sufxvd.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ccx.xingfuxueyuan.xyz

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://jxk.uphjek.com

C#:   // 序列化往返，或自定义 Clone
来源：http://gve.cashguo.top

[K06] 解析 URL 查询串
来源：http://zun.shuidangran.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://sgu.jianghu66.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://nep.shangyingyoupin.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ebf.redwolf501.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://duh.chenlongwang.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ekk.zhijiandao.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://gmu.birdmap.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://cqz.jinyuanbaomall.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://gkw.tianlin.xyz

[K07] 进制转换
来源：http://bor.yongpay.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://les.xziqi.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://lri.ydzc1.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://nfe.smart0.xyz

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://kfx.shanyushiyangkeji.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://rvo.xylfe.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://vyb.gaohongyu789.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://afp.cqqwz.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://keh.vqdsnc.cn

[K08] 二进制序列化（非 JSON）
来源：http://muf.pycfn.com

Py:   pickle.dumps(obj)
来源：http://fze.yanxiufei.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://fbb.hongshengwenyu.top

JS:   v8.serialize(obj)        // Node
来源：http://ayp.zhixingplan.top

TS:   v8.serialize(obj)        // Node
来源：http://gbf.chenlongwang.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://nkv.shuidangran.top

Go:   encoding/gob
来源：http://rpz.cucudq.cn

Ruby: Marshal.dump(obj)
来源：http://fbz.bjfxy.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://dkc.yfazqb.com

================================================================================
来源：http://khd.yonumen.top

L. 网络请求
来源：http://fsn.guannengcc.top

================================================================================
来源：http://rzm.fehbvm.com

[L01] 发送 GET 请求
来源：http://shl.jianghu66.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://idu.shzxlz.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ljb.gzhubu.top

JS:   await fetch(url)
来源：http://cqi.smart0.xyz

TS:   await fetch(url)
来源：http://une.zhoulong.xyz

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://dvp.yj202588.top

Go:   resp, err := http.Get(url)
来源：http://akf.ydjk.org.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://qbp.aizwys.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://srs.sxryk.cn

[L02] 发送 POST JSON
来源：http://jgb.bjfxy.top

Py:   requests.post(url, json={"a": 1})
来源：http://ubu.pengpengdd.cyou

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://fzu.316326.xyz

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://xwz.snrcjt.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://vlr.cucudq.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ior.tian-w.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://udt.chenlongwang.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://jkk.uphjek.com

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://czd.bjfxy.top

[L03] 设置自定义请求头
来源：http://xyz.smart0.xyz

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://lzk.smart0.xyz

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://vmw.meibo888.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://use.wangdashe.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://eml.yuxming.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ovk.mhx1999.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ynj.zhixingplan.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://sns.hywenlv.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://bpa.shanyushiyangtech.top

[L04] 设置超时
来源：http://knj.cashguo.top

Py:   requests.get(url, timeout=5)
来源：http://pdv.hesvh.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://oim.ctjpmb.com

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://zwc.snrcjt.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://pvm.zhengqikj.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://rjj.yj20258888.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://yio.dianchejie.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ebl.dashuyun.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://bog.shuidangran.top

[L05] 上传文件（multipart）
来源：http://cbg.vehdjk.com

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://dwm.ehwqpu.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://qox.yueranfly.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://pkb.cucudq.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ghx.jinqigufen.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://vzm.yj202588.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://yvw.cucudq.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://isd.cdnleiting.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://vdn.kuanghao11.cn

[L06] 解析响应为 JSON
来源：http://twb.haohaochexian.top

Py:   resp.json()
来源：http://ecq.gogol.net.cn

PHP:  json_decode($body, true);
来源：http://kce.xylfe.cn

JS:   await resp.json()
来源：http://azx.yj20258.top

TS:   await resp.json()
来源：http://kam.nanxuanxn.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://zwq.pengpengdd.cyou

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://czp.tarul.cn

Ruby: JSON.parse(resp.body)
来源：http://ljq.svipenyu.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://tvw.guowangkeji.top

[L07] 处理 HTTP 状态码
来源：http://eig.hnxiangtu.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://cpr.guannengcc.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ddf.vqdsnc.cn

JS:   resp.ok;  resp.status
来源：http://xab.shanyushiyangtech.top

TS:   resp.ok;  resp.status
来源：http://wfj.yangfankeji.com

Java: resp.statusCode()
来源：http://ein.zdbjq.cn

Go:   resp.StatusCode
来源：http://eog.ydzc1.top

Ruby: resp.code.to_i
来源：http://bid.quarkkingdee.top

C#:   (int)resp.StatusCode
来源：http://flv.sxryk.cn

[L08] 并发请求多个地址
来源：http://klf.meibo888.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://rpk.birdmap.top

PHP:  curl_multi_init() 系列
来源：http://kww.gzhubu.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://qci.hnxiangtu.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://obu.yj20258888.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://xwh.ydzc1.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://uln.yuanzhike.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wwp.hcnkem.com

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ixu.vehdjk.com

================================================================================
来源：http://fmo.feifeiyinyue.top

M. 命令行 / 进程 / 环境
来源：http://rpc.yuxming.cn

================================================================================
来源：http://bjb.haohaochexian.top

[M01] 读取命令行参数
来源：http://afz.ybcxt.top

Py:   sys.argv[1:]
来源：http://rwa.jiagoushi.top

PHP:  $argv;  $argc;
来源：http://wgd.gotoacloud.top

JS:   process.argv.slice(2)
来源：http://fzw.yfazqb.com

TS:   process.argv.slice(2)
来源：http://lnq.tianlin.xyz

Java: args 数组（main 方法参数）
来源：http://ifw.fzhhl.top

Go:   os.Args[1:]
来源：http://ipv.hywenlv.cn

Ruby: ARGV
来源：http://srk.hysaishi.cn

C#:   args 数组（Main 方法参数）
来源：http://ybw.jinqigfzy.top

[M02] 读取环境变量
来源：http://bkj.shuidangran.top

Py:   os.environ.get("HOME")
来源：http://qkq.xuetiantiany.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://cld.zhixingplan.top

JS:   process.env.HOME
来源：http://qvi.sxryk.cn

TS:   process.env.HOME
来源：http://lsf.zhongyouzk.top

Java: System.getenv("HOME")
来源：http://xry.shzxlz.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hwp.guowangkeji.top

Ruby: ENV["HOME"]
来源：http://tkg.sxryk.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://cfl.tian-w.cn

[M03] 执行外部命令
来源：http://hms.jianghu66.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hwd.xuanzx.com

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://kqi.hammf.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://gkr.uphjek.com

TS:   child_process.execSync("ls -l").toString()
来源：http://amm.fanxiaobao.xyz

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ueb.sysykeji.top

Go:   exec.Command("ls", "-l").Output()
来源：http://pzf.smart0.xyz

Ruby: system("ls -l");  `ls -l`
来源：http://hrf.fengsongda.top

C#:   Process.Start("ls", "-l");
来源：http://tla.sysykeji.top

[M04] 获取当前工作目录
来源：http://lqd.tarul.cn

Py:   os.getcwd()
来源：http://nyv.tian-w.cn

PHP:  getcwd();
来源：http://kkn.xuanzx.com

JS:   process.cwd()
来源：http://uwq.tanke756.top

TS:   process.cwd()
来源：http://djv.jqgfzy.top

Java: Path.of("").toAbsolutePath()
来源：http://zjb.fanxiaobao.xyz

Go:   os.Getwd()
来源：http://rva.jqgfzy.top

Ruby: Dir.pwd
来源：http://esd.316326.xyz

C#:   Directory.GetCurrentDirectory()
来源：http://put.uphjek.com

[M05] 设置退出码
来源：http://baj.dashuyun.cn

Py:   sys.exit(1)
来源：http://mwt.pycfn.com

PHP:  exit(1);
来源：http://isw.jyoumei.cn

JS:   process.exit(1)
来源：http://qok.guannengcc.top

TS:   process.exit(1)
来源：http://ffq.zdqjudy.top

Java: System.exit(1)
来源：http://zfs.316326.xyz

Go:   os.Exit(1)
来源：http://xdk.jlsjyb.cn

Ruby: exit 1
来源：http://hhw.shzxlz.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://rpv.yuxming.cn

[M06] 向标准错误输出
来源：http://hdt.ctjpmb.com

Py:   print("err", file=sys.stderr)
来源：http://bwc.zhoulong.xyz

PHP:  fwrite(STDERR, "err\n");
来源：http://cya.sysykeji.top

JS:   console.error("err")
来源：http://dnz.aizwys.cn

TS:   console.error("err")
来源：http://jsk.hywenlv.cn

Java: System.err.println("err")
来源：http://wlk.0kj1m.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://fnc.xinyue.icu

Ruby: warn "err"
来源：http://aqx.xingfuxueyuan.xyz

C#:   Console.Error.WriteLine("err")
来源：http://frh.aibaodan.cn

[M07] 判断是否为主入口
来源：http://nby.bbcook.cn

Py:   if __name__ == "__main__":
来源：http://abt.gotoacloud.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://jqu.hammf.cn

JS:   require.main === module
来源：http://eqy.cheryme.top

TS:   require.main === module
来源：http://xzv.hfpthk.cn

Java: public static void main(String[] args)
来源：http://xze.zhongyouzk.top

Go:   func main()
来源：http://vre.52xcode.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ggt.aibaodan.cn

C#:   static void Main(string[] args)
来源：http://ouj.jqgfzy.top

[M08] 获取系统与运行时信息
来源：http://ukc.jinyuanbaomall.cn

Py:   platform.system();  platform.python_version()
来源：http://asw.jqgufenzy.top

PHP:  PHP_OS;  phpversion();
来源：http://hvi.feifeiyinyue.top

JS:   process.platform;  process.version
来源：http://cur.316326.xyz

TS:   process.platform;  process.version
来源：http://wrw.snrcjt.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://jih.ywan-chungtsiang.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://qjx.yfazqb.com

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://dfr.9152youxi.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://wta.tarul.cn

================================================================================
来源：http://ajk.aizwys.cn

N. 数据结构与算法
来源：http://ecd.zhoulong.xyz

================================================================================
来源：http://qcw.yonumen.top

[N01] 二分查找（有序数组）
来源：http://pys.epnwcf.com

Py:   bisect.bisect_left(arr, x)
来源：http://eel.9152youxi.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://fdr.shanyushiyangtech.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://tan.daxiang520.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://eua.hammf.cn

Java: Arrays.binarySearch(arr, x)
来源：http://xnu.sufxvd.cn

Go:   sort.SearchInts(arr, x)
来源：http://swo.mhx1999.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://gof.chenlongwang.top

C#:   Array.BinarySearch(arr, x)
来源：http://cqk.vqdsnc.cn

[N02] 排序（工程实践用内置实现）
来源：http://jqn.shanyushiyangkeji.top

Py:   sorted(arr);  arr.sort()
来源：http://fex.yvedp.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://bhy.hywenlv.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://njm.aibaodan.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://duq.guowangkeji.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hab.zhoulong.xyz

Go:   slices.Sort(arr)
来源：http://nye.yongpay.top

Ruby: arr.sort
来源：http://znh.fzhhl.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://lot.hcnkem.com

[N03] 快速排序（分治示例）
来源：http://byw.snrcjt.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://zsn.yanxiufei.cn

PHP:  // 递归实现，或用 usort
来源：http://shj.sufxvd.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mbt.yangfankeji.com

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ply.snrcjt.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mbb.jinqigfzy.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://tbt.haohaochexian.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mwo.tianlin.xyz

C#:   // 手写递归，或 Array.Sort
来源：http://hjp.tanke756.top

[N04] 斐波那契数列
来源：http://aer.hammf.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://nwr.cashguo.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hxf.jqgfzy.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://czg.guowangkeji.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://xys.epnwcf.com

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://num.zhoulong.xyz

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://yqc.gotoacloud.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://jvm.pycfn.com

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://epe.zhaomingkeji.xyz

[N05] 最大公约数
来源：http://vsc.zhoulong.xyz

Py:   math.gcd(a, b)
来源：http://zal.havefunace.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://yqq.uphjek.com

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ozo.52xcode.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://sos.52xcode.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wug.yueranfly.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://cov.hnxiangtu.top

Ruby: a.gcd(b)
来源：http://jog.sysykeji.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://alw.ppjwa.cn

[N06] 判断回文字符串
来源：http://wbk.meibo888.top

Py:   s == s[::-1]
来源：http://lso.jianghu66.top

PHP:  $s === strrev($s);
来源：http://xux.gzhubu.top


<!-- 参考信息 -->