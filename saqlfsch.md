代发 wailian999

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://lxg.wangdashe.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://zlm.c1oappe.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://yac.kuanghao11.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://wfw.xinyue.icu

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://kpu.xinyue.icu

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://zwk.bjfxy.top

[J09] 时区处理
来源：http://hxi.c1oappe.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://wuq.chenzaomai.com

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://iiz.chenzaomai.com

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://qqu.gaohongyu789.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://sdx.epnwcf.com

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://tth.xuanzx.com

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://wpq.iojbl.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://rgy.shangyingyoupin.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://mib.andypj.xyz

[J10] 取今天 / 本月第一天
来源：http://kvt.sufxvd.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://itl.smart0.xyz

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://uqv.xylfe.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://kuv.yj20258888.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://vvl.zhengqikj.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://owp.jinqigufen.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://kgx.hnqzz.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://fho.zdqjudy.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://scs.jyoumei.cn

================================================================================
来源：http://cey.jqgufenzy.top

K. JSON 与序列化
来源：http://sqz.cqqwz.cn

================================================================================
来源：http://ntr.xinyue.icu

[K01] 对象转 JSON 字符串
来源：http://jep.pycfn.com

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://jnb.yuanzhike.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://yzk.shzxlz.cn

JS:   JSON.stringify(obj)
来源：http://ncf.hammf.cn

TS:   JSON.stringify(obj)
来源：http://laa.zhaomingkeji.xyz

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://eha.feifeiyinyue.top

Go:   json.Marshal(obj)
来源：http://pms.tarul.cn

Ruby: obj.to_json                                     // require "json"
来源：http://sip.xziqi.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://gkc.wangshuangyany.cn

[K02] JSON 字符串转对象
来源：http://jrb.daxiang520.top

Py:   json.loads(s)
来源：http://gei.gogol.net.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://tvx.yanxiufei.cn

JS:   JSON.parse(s)
来源：http://yah.yangfankeji.com

TS:   JSON.parse(s)
来源：http://tkm.xylfe.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://lrq.vehdjk.com

Go:   json.Unmarshal(data, &v)
来源：http://zln.0kj1m.cn

Ruby: JSON.parse(s)
来源：http://sbp.fanxiaobao.xyz

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://smb.nwbrower.top

[K03] JSON 美化输出（带缩进）
来源：http://yly.hammf.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://kel.sxryk.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://sgk.ivvv.top

JS:   JSON.stringify(obj, null, 2)
来源：http://ytx.pengpengdd.cyou

TS:   JSON.stringify(obj, null, 2)
来源：http://gvv.quarkkingdee.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://bpn.sweek.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wjw.haohaochexian.top

Ruby: JSON.pretty_generate(obj)
来源：http://eyj.birdmap.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://gnv.jqgufenzy.top

[K04] 读取 JSON 文件
来源：http://vni.sjlbkw.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://nyp.pengpengdd.cyou

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://mwf.52xcode.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hko.cheryme.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ujm.hfpthk.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://nro.tarul.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://iqu.gotoacloud.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://aff.ctjpmb.com

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://gxp.ctjpmb.com

[K05] 深拷贝对象
来源：http://fwt.yuanzhike.top

Py:   copy.deepcopy(obj)
来源：http://phs.haohaochexian.top

PHP:  unserialize(serialize($obj));
来源：http://yxe.xuetiantiany.cn

JS:   structuredClone(obj)
来源：http://naz.tarul.cn

TS:   structuredClone(obj)
来源：http://zfr.guannengcc.top

Java: // 手写拷贝构造，或序列化往返
来源：http://gtl.zhaomingkeji.xyz

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://lfk.yj202588.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ypa.zhengqikj.top

C#:   // 序列化往返，或自定义 Clone
来源：http://wbz.daxiang520.top

[K06] 解析 URL 查询串
来源：http://yto.ydjk.org.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ojc.yvedp.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://rcl.52xcode.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ddj.sufxvd.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://bdv.yueranfly.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ofo.jianghu66.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://ouc.zycfv.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://yvk.ppjwa.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://fku.vqdsnc.cn

[K07] 进制转换
来源：http://aou.ppjwa.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://gup.jqgufenzy.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://csg.zhengqikj.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://guf.jlsjyb.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://fbb.gotoacloud.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://itd.shanyushiyangtech.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://pbf.chenjidiqi.icu

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://dgn.feifeiyinyue.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://tdh.pycfn.com

[K08] 二进制序列化（非 JSON）
来源：http://vui.ehwqpu.com

Py:   pickle.dumps(obj)
来源：http://ine.shanyushiyangtech.top

PHP:  serialize($obj);  unserialize($s);
来源：http://alh.jlsjyb.cn

JS:   v8.serialize(obj)        // Node
来源：http://smi.fzhhl.top

TS:   v8.serialize(obj)        // Node
来源：http://wmd.zhixingplan.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://iyu.ppjwa.cn

Go:   encoding/gob
来源：http://kph.zdbjq.cn

Ruby: Marshal.dump(obj)
来源：http://uhd.snrcjt.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://rdd.cdnleiting.top

================================================================================
来源：http://hjz.dianchejie.cn

L. 网络请求
来源：http://fjd.svipenyu.cn

================================================================================
来源：http://fou.shuidangran.top

[L01] 发送 GET 请求
来源：http://nal.ybcxt.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://xld.yueranfly.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://aeu.kuanghao11.cn

JS:   await fetch(url)
来源：http://whn.cqqwz.cn

TS:   await fetch(url)
来源：http://liy.xingfuxueyuan.xyz

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://sjs.sysykeji.top

Go:   resp, err := http.Get(url)
来源：http://xzx.fktsv.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://big.fzhhl.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://rth.shanyushiyangkeji.top

[L02] 发送 POST JSON
来源：http://hjh.jlsjyb.cn

Py:   requests.post(url, json={"a": 1})
来源：http://uty.jinyuanbaomall.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://yiw.hnqzz.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mbb.yuxming.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://dha.jianghu66.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://pxg.hcnkem.com

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://pyy.tanke756.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ydk.sufxvd.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://fgv.xuetiantiany.cn

[L03] 设置自定义请求头
来源：http://jdi.xylfe.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://yqc.xuetiantiany.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://jfe.guowangkeji.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://pbw.zhixingplan.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://thc.fengsongda.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://yvv.chenjidiqi.icu

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wut.dianchejie.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ekg.yfazqb.com

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://zlk.svipenyu.cn

[L04] 设置超时
来源：http://tnf.hfpthk.cn

Py:   requests.get(url, timeout=5)
来源：http://dgc.chenlongwang.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://rea.tarul.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://kdy.gaohongyu789.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://udc.gogol.net.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://kqd.9152youxi.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://fhc.yuanzhike.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://src.chenzaomai.com

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://qgg.nanxinkj.top

[L05] 上传文件（multipart）
来源：http://jpo.jinghuilouyu.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://dap.redwolf501.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://cgy.zycfv.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://tzh.nwbrower.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://bns.vqdsnc.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://seg.zdqjudy.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://lzt.yj20258888.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://fqd.aizwys.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ipp.quarkkingdee.top

[L06] 解析响应为 JSON
来源：http://qag.zhongyouzk.top

Py:   resp.json()
来源：http://ixq.xinyue.icu

PHP:  json_decode($body, true);
来源：http://jnj.hammf.cn

JS:   await resp.json()
来源：http://rdg.c1oappe.top

TS:   await resp.json()
来源：http://ksd.nanxinkj.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://klo.birdmap.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ghz.cqqwz.cn

Ruby: JSON.parse(resp.body)
来源：http://cok.chenlongwang.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://jxu.ivvv.top

[L07] 处理 HTTP 状态码
来源：http://khz.daxiang520.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://etz.guowangkeji.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://qbe.tianlin.xyz

JS:   resp.ok;  resp.status
来源：http://bdd.sweek.top

TS:   resp.ok;  resp.status
来源：http://kag.mhx1999.top

Java: resp.statusCode()
来源：http://avd.shanyushiyangkeji.top

Go:   resp.StatusCode
来源：http://vde.jinyuanbaomall.cn

Ruby: resp.code.to_i
来源：http://urw.9152youxi.cn

C#:   (int)resp.StatusCode
来源：http://mwc.nanxinkj.top

[L08] 并发请求多个地址
来源：http://wjj.nanxuanxn.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://tpr.nanxinkj.top

PHP:  curl_multi_init() 系列
来源：http://fgh.yj20258888.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://vio.svipenyu.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://pcy.chenjidiqi.icu

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://cbh.wangdashe.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wzp.guannengcc.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://yyz.gzhubu.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hvk.ivvv.top

================================================================================
来源：http://crs.uphjek.com

M. 命令行 / 进程 / 环境
来源：http://zab.zdqjudy.top

================================================================================
来源：http://rmd.zdbjq.cn

[M01] 读取命令行参数
来源：http://kfo.havefunace.top

Py:   sys.argv[1:]
来源：http://twd.hfpthk.cn

PHP:  $argv;  $argc;
来源：http://jpf.jinghuilouyu.cn

JS:   process.argv.slice(2)
来源：http://nhh.hysaishi.cn

TS:   process.argv.slice(2)
来源：http://eju.kuanghao11.cn

Java: args 数组（main 方法参数）
来源：http://cwd.zdbjq.cn

Go:   os.Args[1:]
来源：http://kwb.yongpay.top

Ruby: ARGV
来源：http://enm.0kj1m.cn

C#:   args 数组（Main 方法参数）
来源：http://jgk.zhixingplan.top

[M02] 读取环境变量
来源：http://iff.yangfankeji.com

Py:   os.environ.get("HOME")
来源：http://tuw.yj20258.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://bjw.aibaodan.cn

JS:   process.env.HOME
来源：http://wme.yanxiufei.cn

TS:   process.env.HOME
来源：http://kds.gzhubu.top

Java: System.getenv("HOME")
来源：http://nik.zycfv.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://qln.hywenlv.cn

Ruby: ENV["HOME"]
来源：http://buo.sufxvd.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ajr.tanke756.top

[M03] 执行外部命令
来源：http://wmj.aizwys.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://lib.vehdjk.com

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://zsh.bjfxy.top

JS:   child_process.execSync("ls -l").toString()
来源：http://ltm.shanyushiyangtech.top

TS:   child_process.execSync("ls -l").toString()
来源：http://wgb.yanxiufei.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://lju.xylfe.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://kyb.gogol.net.cn

Ruby: system("ls -l");  `ls -l`
来源：http://dki.cheryme.top

C#:   Process.Start("ls", "-l");
来源：http://rtt.ehwqpu.com

[M04] 获取当前工作目录
来源：http://thh.zhaomingkeji.xyz

Py:   os.getcwd()
来源：http://fsl.yongpay.top

PHP:  getcwd();
来源：http://qzl.haohaochexian.top

JS:   process.cwd()
来源：http://cqv.zdbjq.cn

TS:   process.cwd()
来源：http://xuz.0kj1m.cn

Java: Path.of("").toAbsolutePath()
来源：http://zrm.gotoacloud.top

Go:   os.Getwd()
来源：http://ksh.yanxiufei.cn

Ruby: Dir.pwd
来源：http://syt.wangdashe.top

C#:   Directory.GetCurrentDirectory()
来源：http://jgj.gogol.net.cn

[M05] 设置退出码
来源：http://xmg.yuxming.cn

Py:   sys.exit(1)
来源：http://ttr.zhongyouzk.top

PHP:  exit(1);
来源：http://suv.ppjwa.cn

JS:   process.exit(1)
来源：http://ivd.hnxiangtu.top

TS:   process.exit(1)
来源：http://vqt.yanxiufei.cn

Java: System.exit(1)
来源：http://xcn.haohaochexian.top

Go:   os.Exit(1)
来源：http://sam.jyoumei.cn

Ruby: exit 1
来源：http://evg.shanyushiyangkeji.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://vxx.0kj1m.cn

[M06] 向标准错误输出
来源：http://ruo.yj20258.top

Py:   print("err", file=sys.stderr)
来源：http://jen.jinyuanbaomall.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://bkk.yj20258.top

JS:   console.error("err")
来源：http://qxc.zhengqikj.top

TS:   console.error("err")
来源：http://hkn.jqgufenzy.top

Java: System.err.println("err")
来源：http://gup.hnqzz.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hsc.aibaodan.cn

Ruby: warn "err"
来源：http://xpq.sweek.top

C#:   Console.Error.WriteLine("err")
来源：http://xsm.hnxiangtu.top

[M07] 判断是否为主入口
来源：http://wdw.pycfn.com

Py:   if __name__ == "__main__":
来源：http://gra.havefunace.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://szq.gzhubu.top

JS:   require.main === module
来源：http://qlo.tarul.cn

TS:   require.main === module
来源：http://xgu.jqgufenzy.top

Java: public static void main(String[] args)
来源：http://xud.yangfankeji.com

Go:   func main()
来源：http://wio.zhijiandao.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://fsd.daria6918.cn

C#:   static void Main(string[] args)
来源：http://jub.jqgufenzy.top

[M08] 获取系统与运行时信息
来源：http://uoc.zhiwuduotai.top

Py:   platform.system();  platform.python_version()
来源：http://hye.zhengqikj.top

PHP:  PHP_OS;  phpversion();
来源：http://suw.zhiwuduotai.top

JS:   process.platform;  process.version
来源：http://bie.aizwys.cn

TS:   process.platform;  process.version
来源：http://syi.fzhhl.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://jcr.hfpthk.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://lkw.jianghu66.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://smq.bbcook.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://uhg.jinqigufen.top

================================================================================
来源：http://njt.jlsjyb.cn

N. 数据结构与算法
来源：http://xrb.tian-w.cn

================================================================================
来源：http://wtn.zhijiandao.cn

[N01] 二分查找（有序数组）
来源：http://brw.svipenyu.cn

Py:   bisect.bisect_left(arr, x)
来源：http://yku.ywan-chungtsiang.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://yvc.sxryk.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://zdb.hnxiangtu.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://vlp.jiagoushi.top

Java: Arrays.binarySearch(arr, x)
来源：http://ikp.sxryk.cn

Go:   sort.SearchInts(arr, x)
来源：http://gkb.tian-w.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://qxb.daxiang520.top

C#:   Array.BinarySearch(arr, x)
来源：http://yhn.52xcode.cn

[N02] 排序（工程实践用内置实现）
来源：http://zco.shangyingyoupin.top

Py:   sorted(arr);  arr.sort()
来源：http://rbs.sufxvd.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ejd.chenzaomai.com

JS:   [...arr].sort((a, b) => a - b)
来源：http://cxw.sysykeji.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://xjq.9152youxi.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://pbr.9152youxi.cn

Go:   slices.Sort(arr)
来源：http://vor.jinqigfzy.top

Ruby: arr.sort
来源：http://cfe.guowangkeji.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://dre.xingfuxueyuan.xyz

[N03] 快速排序（分治示例）
来源：http://xls.xingfuxueyuan.xyz

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://sbn.zdqjudy.top

PHP:  // 递归实现，或用 usort
来源：http://cyu.jqgfzy.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hfy.pycfn.com

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://nvl.chenlongwang.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://klm.zdbjq.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ynd.cheryme.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://uju.jinghuilouyu.cn

C#:   // 手写递归，或 Array.Sort
来源：http://owy.pengpengdd.cyou

[N04] 斐波那契数列
来源：http://hdi.yj20258.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://yjy.smart0.xyz

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://yfs.ydzc1.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://gco.jqgufenzy.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ipw.jiagoushi.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hco.wangshuangyany.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://dtq.jyoumei.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://dxt.hysaishi.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://eyh.jlsjyb.cn

[N05] 最大公约数
来源：http://cvr.shuidangran.top

Py:   math.gcd(a, b)
来源：http://zvq.bbcook.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://vzk.zhoulong.xyz

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://zjn.yonumen.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mci.hnqzz.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://rqd.dianchejie.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://zai.birdmap.top

Ruby: a.gcd(b)
来源：http://jfk.tian-w.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mmv.xylfe.cn

[N06] 判断回文字符串
来源：http://fyg.guannengcc.top

Py:   s == s[::-1]
来源：http://jcu.hammf.cn

PHP:  $s === strrev($s);
来源：http://ejb.xingfuxueyuan.xyz


<!-- 参考信息 -->