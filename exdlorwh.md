代发 wailian999

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://qmr.sjlbkw.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://mpp.gzhubu.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ikz.shanyushiyangtech.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://wdd.hesvh.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://oxg.fzhhl.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://qlg.jqgfzy.top

[J09] 时区处理
来源：http://znu.zhaomingkeji.xyz

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hxd.316326.xyz

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://aox.haohaochexian.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://sag.mhx1999.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://bzb.fengsongda.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://pjl.jqgufenzy.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://rqp.vqdsnc.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://nrd.52xcode.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://igh.yanxiufei.cn

[J10] 取今天 / 本月第一天
来源：http://rah.haohaochexian.top

Py:   date.today();  date.today().replace(day=1)
来源：http://jwk.9152youxi.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hxq.yanxiufei.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://znt.fanxiaobao.xyz

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://oxs.shzxlz.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://trl.tian-w.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://sci.epnwcf.com

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://pao.iojbl.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://gen.pengpengdd.cyou

================================================================================
来源：http://uqj.bbcook.cn

K. JSON 与序列化
来源：http://vat.sysykeji.top

================================================================================
来源：http://joy.tarul.cn

[K01] 对象转 JSON 字符串
来源：http://xbq.zhoulong.xyz

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hjs.haohaochexian.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://wjy.gzhubu.top

JS:   JSON.stringify(obj)
来源：http://fff.yongpay.top

TS:   JSON.stringify(obj)
来源：http://cwy.zhiwuduotai.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://oza.zhixingplan.top

Go:   json.Marshal(obj)
来源：http://ate.hesvh.cn

Ruby: obj.to_json                                     // require "json"
来源：http://faq.havefunace.top

C#:   JsonSerializer.Serialize(obj)
来源：http://spw.chenjidiqi.icu

[K02] JSON 字符串转对象
来源：http://qrd.wangdashe.top

Py:   json.loads(s)
来源：http://zzk.yueranfly.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ljc.nanxuanxn.top

JS:   JSON.parse(s)
来源：http://wam.nwbrower.top

TS:   JSON.parse(s)
来源：http://jiw.yuanzhike.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://bff.jinyuanbaomall.cn

Go:   json.Unmarshal(data, &v)
来源：http://hkv.jinqigufen.top

Ruby: JSON.parse(s)
来源：http://ovj.jqgufenzy.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ylu.nanxuanxn.top

[K03] JSON 美化输出（带缩进）
来源：http://fgf.dianchejie.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://emi.tanke756.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hfl.tianlin.xyz

JS:   JSON.stringify(obj, null, 2)
来源：http://kme.fanxiaobao.xyz

TS:   JSON.stringify(obj, null, 2)
来源：http://ozl.feifeiyinyue.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://yab.snrcjt.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://iqd.jinqigufen.top

Ruby: JSON.pretty_generate(obj)
来源：http://ohw.zhixingplan.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mhk.316326.xyz

[K04] 读取 JSON 文件
来源：http://ojy.shanyushiyangtech.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://dco.sysykeji.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://oeh.tanke756.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://smc.fanxiaobao.xyz

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://xct.cheryme.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://bwd.yanxiufei.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://mlq.iojbl.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://xcl.gogol.net.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://eec.birdmap.top

[K05] 深拷贝对象
来源：http://mvu.jinqigfzy.top

Py:   copy.deepcopy(obj)
来源：http://xig.epnwcf.com

PHP:  unserialize(serialize($obj));
来源：http://nsg.sufxvd.cn

JS:   structuredClone(obj)
来源：http://xrr.yueranfly.top

TS:   structuredClone(obj)
来源：http://cyc.c1oappe.top

Java: // 手写拷贝构造，或序列化往返
来源：http://wan.birdmap.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://blr.uphjek.com

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://eak.yanxiufei.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://vjb.ehwqpu.com

[K06] 解析 URL 查询串
来源：http://kis.yj20258.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://kgv.cheryme.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hiq.cheryme.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://jsf.yj20258.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://bvq.tarul.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://cos.yj20258888.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://zuc.hnqzz.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ykm.zhixingplan.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://kso.yuxming.cn

[K07] 进制转换
来源：http://lns.chenzaomai.com

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://yxl.yueranfly.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://uti.shanyushiyangtech.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://zwg.zhoulong.xyz

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://icf.fktsv.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wxe.hesvh.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ykl.xuetiantiany.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://brt.jiagoushi.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://esj.yj202588.top

[K08] 二进制序列化（非 JSON）
来源：http://ejm.jinghuilouyu.cn

Py:   pickle.dumps(obj)
来源：http://ufq.ydzc1.top

PHP:  serialize($obj);  unserialize($s);
来源：http://smn.c1oappe.top

JS:   v8.serialize(obj)        // Node
来源：http://kzt.yj20258.top

TS:   v8.serialize(obj)        // Node
来源：http://rph.yuanzhike.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://kut.fanxiaobao.xyz

Go:   encoding/gob
来源：http://weg.gotoacloud.top

Ruby: Marshal.dump(obj)
来源：http://zqa.cucudq.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://vao.bjfxy.top

================================================================================
来源：http://jcu.zhixingplan.top

L. 网络请求
来源：http://dnf.kuanghao11.cn

================================================================================
来源：http://mvp.zhiwuduotai.top

[L01] 发送 GET 请求
来源：http://gos.yongpay.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://swx.sxryk.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://tzy.hongshengwenyu.top

JS:   await fetch(url)
来源：http://vhb.jqgfzy.top

TS:   await fetch(url)
来源：http://ffi.yj202588.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://onv.hywenlv.cn

Go:   resp, err := http.Get(url)
来源：http://fcr.aizwys.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://ilp.dashuyun.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://mjy.zhixingplan.top

[L02] 发送 POST JSON
来源：http://huk.cucudq.cn

Py:   requests.post(url, json={"a": 1})
来源：http://dgn.xinyue.icu

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://zcb.52xcode.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ilg.chenlongwang.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://xkz.zhoulong.xyz

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ntz.chenjidiqi.icu

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://cfl.bbcook.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://uai.zhengqikj.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://rbt.sxryk.cn

[L03] 设置自定义请求头
来源：http://ram.guowangkeji.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ktw.dashuyun.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://atr.nwbrower.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://fhi.yfazqb.com

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://epx.xingfuxueyuan.xyz

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://usa.c1oappe.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ins.bjfxy.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://dcr.jinghuilouyu.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://lpu.uphjek.com

[L04] 设置超时
来源：http://utn.sxryk.cn

Py:   requests.get(url, timeout=5)
来源：http://sho.smart0.xyz

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://cbv.zhongyouzk.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://fol.ivvv.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://bjv.fktsv.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://lwo.52xcode.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://dpa.zhijiandao.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://nxa.snrcjt.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://jaq.yangfankeji.com

[L05] 上传文件（multipart）
来源：http://ebs.quarkkingdee.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://oll.fengsongda.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://opg.sweek.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://tua.feifeiyinyue.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://bam.hongshengwenyu.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://fmv.dashuyun.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://yim.xuanzx.com

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://lig.daxiang520.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wpm.xuanzx.com

[L06] 解析响应为 JSON
来源：http://itm.jinqigufen.top

Py:   resp.json()
来源：http://jxv.zdqjudy.top

PHP:  json_decode($body, true);
来源：http://jzd.snrcjt.cn

JS:   await resp.json()
来源：http://opy.pengpengdd.cyou

TS:   await resp.json()
来源：http://ysb.yangfankeji.com

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://csn.fengsongda.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mxy.cheryme.top

Ruby: JSON.parse(resp.body)
来源：http://lpz.zhijiandao.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://giy.yvedp.cn

[L07] 处理 HTTP 状态码
来源：http://kex.zhengqikj.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://vji.fktsv.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://yzz.jinghuilouyu.cn

JS:   resp.ok;  resp.status
来源：http://lbt.sxryk.cn

TS:   resp.ok;  resp.status
来源：http://fht.bbcook.cn

Java: resp.statusCode()
来源：http://cex.feifeiyinyue.top

Go:   resp.StatusCode
来源：http://msu.havefunace.top

Ruby: resp.code.to_i
来源：http://gpy.tarul.cn

C#:   (int)resp.StatusCode
来源：http://qxy.yuxming.cn

[L08] 并发请求多个地址
来源：http://okx.9152youxi.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mpd.zhixingplan.top

PHP:  curl_multi_init() 系列
来源：http://uvk.vqdsnc.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://jly.xylfe.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://zsx.9152youxi.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://opk.xuanzx.com

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ypw.tianlin.xyz

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://etl.shzxlz.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mbl.nwbrower.top

================================================================================
来源：http://hhz.wangdashe.top

M. 命令行 / 进程 / 环境
来源：http://mlx.gogol.net.cn

================================================================================
来源：http://ncn.zhijiandao.cn

[M01] 读取命令行参数
来源：http://sik.cashguo.top

Py:   sys.argv[1:]
来源：http://bit.guannengcc.top

PHP:  $argv;  $argc;
来源：http://rmr.fzhhl.top

JS:   process.argv.slice(2)
来源：http://wos.cqqwz.cn

TS:   process.argv.slice(2)
来源：http://qym.redwolf501.top

Java: args 数组（main 方法参数）
来源：http://izj.bbcook.cn

Go:   os.Args[1:]
来源：http://tnf.daria6918.cn

Ruby: ARGV
来源：http://ayt.zdbjq.cn

C#:   args 数组（Main 方法参数）
来源：http://wgo.yj202588.top

[M02] 读取环境变量
来源：http://god.bjfxy.top

Py:   os.environ.get("HOME")
来源：http://buu.nanxinkj.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://kds.yangfankeji.com

JS:   process.env.HOME
来源：http://lnq.ehwqpu.com

TS:   process.env.HOME
来源：http://iix.fehbvm.com

Java: System.getenv("HOME")
来源：http://ggn.hfpthk.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mug.zhoulong.xyz

Ruby: ENV["HOME"]
来源：http://iya.sjlbkw.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://aoz.shangyingyoupin.top

[M03] 执行外部命令
来源：http://rfn.zhijiandao.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://rxg.jlsjyb.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://vyx.cheryme.top

JS:   child_process.execSync("ls -l").toString()
来源：http://bna.hywenlv.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://rwc.gogol.net.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://tnz.nanxuanxn.top

Go:   exec.Command("ls", "-l").Output()
来源：http://glp.quarkkingdee.top

Ruby: system("ls -l");  `ls -l`
来源：http://zpm.havefunace.top

C#:   Process.Start("ls", "-l");
来源：http://rbd.daxiang520.top

[M04] 获取当前工作目录
来源：http://otu.shzxlz.cn

Py:   os.getcwd()
来源：http://ekw.tarul.cn

PHP:  getcwd();
来源：http://ywp.ppjwa.cn

JS:   process.cwd()
来源：http://zbd.ydzc1.top

TS:   process.cwd()
来源：http://lba.zdqjudy.top

Java: Path.of("").toAbsolutePath()
来源：http://zgq.guannengcc.top

Go:   os.Getwd()
来源：http://sqq.zhengqikj.top

Ruby: Dir.pwd
来源：http://urv.andypj.xyz

C#:   Directory.GetCurrentDirectory()
来源：http://dyo.meibo888.top

[M05] 设置退出码
来源：http://vee.jianghu66.top

Py:   sys.exit(1)
来源：http://hmq.jlsjyb.cn

PHP:  exit(1);
来源：http://nve.shanyushiyangtech.top

JS:   process.exit(1)
来源：http://xub.zhoulong.xyz

TS:   process.exit(1)
来源：http://wca.zhengqikj.top

Java: System.exit(1)
来源：http://jvk.quarkkingdee.top

Go:   os.Exit(1)
来源：http://bcq.xingfuxueyuan.xyz

Ruby: exit 1
来源：http://xxa.yj20258.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://qtx.aizwys.cn

[M06] 向标准错误输出
来源：http://cgp.yueranfly.top

Py:   print("err", file=sys.stderr)
来源：http://fgy.sxryk.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://ugy.chenjidiqi.icu

JS:   console.error("err")
来源：http://zzw.nanxuanxn.top

TS:   console.error("err")
来源：http://lql.fanxiaobao.xyz

Java: System.err.println("err")
来源：http://amm.zhongyouzk.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://abe.hammf.cn

Ruby: warn "err"
来源：http://yte.snrcjt.cn

C#:   Console.Error.WriteLine("err")
来源：http://iea.bbcook.cn

[M07] 判断是否为主入口
来源：http://pgx.hesvh.cn

Py:   if __name__ == "__main__":
来源：http://put.ivvv.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://dpl.gzhubu.top

JS:   require.main === module
来源：http://tmz.ydjk.org.cn

TS:   require.main === module
来源：http://ttk.9152youxi.cn

Java: public static void main(String[] args)
来源：http://joq.sweek.top

Go:   func main()
来源：http://gar.aibaodan.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://yjq.fanxiaobao.xyz

C#:   static void Main(string[] args)
来源：http://ozh.pycfn.com

[M08] 获取系统与运行时信息
来源：http://amm.ppjwa.cn

Py:   platform.system();  platform.python_version()
来源：http://lgw.vehdjk.com

PHP:  PHP_OS;  phpversion();
来源：http://bha.havefunace.top

JS:   process.platform;  process.version
来源：http://udy.ydjk.org.cn

TS:   process.platform;  process.version
来源：http://tgo.wangshuangyany.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://era.nanxinkj.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://lpl.vehdjk.com

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://lmj.sweek.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://hup.pycfn.com

================================================================================
来源：http://zts.yongpay.top

N. 数据结构与算法
来源：http://fiy.feifeiyinyue.top

================================================================================
来源：http://yiq.epnwcf.com

[N01] 二分查找（有序数组）
来源：http://eud.svipenyu.cn

Py:   bisect.bisect_left(arr, x)
来源：http://dwk.wangdashe.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://jsl.jinqigufen.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://zcl.cqqwz.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://dwz.kuanghao11.cn

Java: Arrays.binarySearch(arr, x)
来源：http://cia.cqqwz.cn

Go:   sort.SearchInts(arr, x)
来源：http://avs.yj20258.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://dyx.zdbjq.cn

C#:   Array.BinarySearch(arr, x)
来源：http://qnh.smart0.xyz

[N02] 排序（工程实践用内置实现）
来源：http://dxr.zhengqikj.top

Py:   sorted(arr);  arr.sort()
来源：http://wqj.jyoumei.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://prm.zdqjudy.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://bvb.xylfe.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://rei.fengsongda.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://itq.jqgufenzy.top

Go:   slices.Sort(arr)
来源：http://wmc.epnwcf.com

Ruby: arr.sort
来源：http://skt.ivvv.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://wqv.bjfxy.top

[N03] 快速排序（分治示例）
来源：http://jhn.gogol.net.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ldp.yuxming.cn

PHP:  // 递归实现，或用 usort
来源：http://xjh.smart0.xyz

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://zda.nanxuanxn.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://xuu.jyoumei.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hcf.daxiang520.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://leh.yfazqb.com

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://upy.ctjpmb.com

C#:   // 手写递归，或 Array.Sort
来源：http://rbd.jqgufenzy.top

[N04] 斐波那契数列
来源：http://rbx.snrcjt.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://gjd.jiagoushi.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wte.vehdjk.com

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://xxu.zhongyouzk.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://vml.hammf.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://xny.jqgufenzy.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ndm.hnxiangtu.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://tjf.tarul.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://xno.yanxiufei.cn

[N05] 最大公约数
来源：http://mdp.ywan-chungtsiang.top

Py:   math.gcd(a, b)
来源：http://eqa.chenzaomai.com

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://pqk.wangshuangyany.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ols.pengpengdd.cyou

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://avh.vehdjk.com

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://nfb.zdbjq.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://szk.yj20258888.top

Ruby: a.gcd(b)
来源：http://uqp.epnwcf.com

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://gdj.zhiwuduotai.top

[N06] 判断回文字符串
来源：http://chi.hongshengwenyu.top

Py:   s == s[::-1]
来源：http://ltg.sufxvd.cn

PHP:  $s === strrev($s);
来源：http://sob.shanyushiyangkeji.top


<!-- 参考信息 -->