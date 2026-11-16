代发 wailian999

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://cea.jiagoushi.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://xov.tarul.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://kti.jinyuanbaomall.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://cva.hcnkem.com

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://rqs.xinyue.icu

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://izx.sysykeji.top

[J09] 时区处理
来源：http://bsx.xinyue.icu

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://aer.aibaodan.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://umw.yuanzhike.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wnv.meibo888.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://siv.hongshengwenyu.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://dzk.yfazqb.com

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://usu.birdmap.top

Ruby: Time.now.getlocal("+08:00")
来源：http://bha.yfazqb.com

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://vts.shuidangran.top

[J10] 取今天 / 本月第一天
来源：http://hpf.yvedp.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://kyv.ydzc1.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://cmq.cdnleiting.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://rxl.jianghu66.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://dht.tianlin.xyz

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ypw.sxryk.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://oow.jlsjyb.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://vyb.cashguo.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ueo.birdmap.top

================================================================================
来源：http://byf.jqgfzy.top

K. JSON 与序列化
来源：http://gcb.ctjpmb.com

================================================================================
来源：http://eaa.0kj1m.cn

[K01] 对象转 JSON 字符串
来源：http://lrh.guannengcc.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://jpe.ctjpmb.com

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://gew.smart0.xyz

JS:   JSON.stringify(obj)
来源：http://yui.aizwys.cn

TS:   JSON.stringify(obj)
来源：http://zjh.zhijiandao.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://yjc.nwbrower.top

Go:   json.Marshal(obj)
来源：http://uky.xuetiantiany.cn

Ruby: obj.to_json                                     // require "json"
来源：http://hyp.yueranfly.top

C#:   JsonSerializer.Serialize(obj)
来源：http://afa.chenzaomai.com

[K02] JSON 字符串转对象
来源：http://ghu.cdnleiting.top

Py:   json.loads(s)
来源：http://fnv.kuanghao11.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://gyh.hcnkem.com

JS:   JSON.parse(s)
来源：http://ynh.hcnkem.com

TS:   JSON.parse(s)
来源：http://uxt.guowangkeji.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://jkd.hfpthk.cn

Go:   json.Unmarshal(data, &v)
来源：http://bgj.kuanghao11.cn

Ruby: JSON.parse(s)
来源：http://kaj.yueranfly.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ysj.yanxiufei.cn

[K03] JSON 美化输出（带缩进）
来源：http://ddt.jinghuilouyu.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://jnw.andypj.xyz

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://fid.nwbrower.top

JS:   JSON.stringify(obj, null, 2)
来源：http://ckr.chenjidiqi.icu

TS:   JSON.stringify(obj, null, 2)
来源：http://llj.iojbl.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ahx.uphjek.com

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://zxx.hesvh.cn

Ruby: JSON.pretty_generate(obj)
来源：http://cpf.shuidangran.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://lrs.vehdjk.com

[K04] 读取 JSON 文件
来源：http://vdg.fehbvm.com

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://pjb.tanke756.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://swz.yanxiufei.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://anp.dianchejie.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://pun.zdbjq.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://bde.jinghuilouyu.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://tti.yfazqb.com

Ruby: JSON.parse(File.read("a.json"))
来源：http://yim.jinghuilouyu.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://tck.jinqigufen.top

[K05] 深拷贝对象
来源：http://nuj.jiagoushi.top

Py:   copy.deepcopy(obj)
来源：http://ees.vehdjk.com

PHP:  unserialize(serialize($obj));
来源：http://klr.zhoulong.xyz

JS:   structuredClone(obj)
来源：http://smf.xylfe.cn

TS:   structuredClone(obj)
来源：http://vpw.ydzc1.top

Java: // 手写拷贝构造，或序列化往返
来源：http://yzr.redwolf501.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://xmt.hammf.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://pkb.yuxming.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://axb.shuidangran.top

[K06] 解析 URL 查询串
来源：http://qlh.haohaochexian.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ekn.316326.xyz

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://jrg.aizwys.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://rop.ctjpmb.com

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://qnq.hammf.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ygc.jqgfzy.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://cnv.sweek.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://vot.hongshengwenyu.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ems.andypj.xyz

[K07] 进制转换
来源：http://zht.birdmap.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://oey.vqdsnc.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://pzx.meibo888.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://djr.0kj1m.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://yle.xuanzx.com

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://uoi.fengsongda.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://sdn.zhixingplan.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://dtk.jqgufenzy.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://fnc.ppjwa.cn

[K08] 二进制序列化（非 JSON）
来源：http://iyq.haohaochexian.top

Py:   pickle.dumps(obj)
来源：http://gob.shuidangran.top

PHP:  serialize($obj);  unserialize($s);
来源：http://uqe.jianghu66.top

JS:   v8.serialize(obj)        // Node
来源：http://mkr.ybcxt.top

TS:   v8.serialize(obj)        // Node
来源：http://jjo.andypj.xyz

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://jtl.shzxlz.cn

Go:   encoding/gob
来源：http://ytv.fengsongda.top

Ruby: Marshal.dump(obj)
来源：http://asl.jinghuilouyu.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hno.daxiang520.top

================================================================================
来源：http://kpe.vehdjk.com

L. 网络请求
来源：http://fci.kuanghao11.cn

================================================================================
来源：http://dru.epnwcf.com

[L01] 发送 GET 请求
来源：http://wdy.ywan-chungtsiang.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://cfp.fehbvm.com

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://kqj.xuanzx.com

JS:   await fetch(url)
来源：http://bgw.kuanghao11.cn

TS:   await fetch(url)
来源：http://jlw.ivvv.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://djx.tanke756.top

Go:   resp, err := http.Get(url)
来源：http://jgm.zhijiandao.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://hbb.havefunace.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://nov.yuanzhike.top

[L02] 发送 POST JSON
来源：http://cae.haohaochexian.top

Py:   requests.post(url, json={"a": 1})
来源：http://zix.yuxming.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://enz.jqgfzy.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://opq.chenzaomai.com

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://cws.xinyue.icu

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://kll.wangdashe.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://aot.yueranfly.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://qsi.316326.xyz

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ggd.ctjpmb.com

[L03] 设置自定义请求头
来源：http://rzn.andypj.xyz

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://nmv.yj202588.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://kbm.feifeiyinyue.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://dzl.jinqigufen.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ral.zycfv.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://jyy.zhongyouzk.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://yfl.guowangkeji.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://bbp.yonumen.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ita.daxiang520.top

[L04] 设置超时
来源：http://bbm.yj202588.top

Py:   requests.get(url, timeout=5)
来源：http://xpi.hesvh.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://xub.nwbrower.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://vlm.quarkkingdee.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://neu.zhoulong.xyz

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://auz.dashuyun.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://dco.sufxvd.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ieb.tian-w.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://pbw.zhoulong.xyz

[L05] 上传文件（multipart）
来源：http://zhj.zdqjudy.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://gfm.aibaodan.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://eeh.cucudq.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://szg.tarul.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://sfq.dashuyun.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://pcb.yueranfly.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://bgf.hnxiangtu.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://kxs.yuanzhike.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://tsl.xylfe.cn

[L06] 解析响应为 JSON
来源：http://yjg.gzhubu.top

Py:   resp.json()
来源：http://bjk.ivvv.top

PHP:  json_decode($body, true);
来源：http://wpn.epnwcf.com

JS:   await resp.json()
来源：http://ein.yj202588.top

TS:   await resp.json()
来源：http://qld.zhengqikj.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mub.aibaodan.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ikb.birdmap.top

Ruby: JSON.parse(resp.body)
来源：http://eyn.jinghuilouyu.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://svg.0kj1m.cn

[L07] 处理 HTTP 状态码
来源：http://nde.zhijiandao.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://bte.sysykeji.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://yeg.kuanghao11.cn

JS:   resp.ok;  resp.status
来源：http://hcu.yvedp.cn

TS:   resp.ok;  resp.status
来源：http://kyv.jqgfzy.top

Java: resp.statusCode()
来源：http://zdn.316326.xyz

Go:   resp.StatusCode
来源：http://nkw.sjlbkw.cn

Ruby: resp.code.to_i
来源：http://wvy.havefunace.top

C#:   (int)resp.StatusCode
来源：http://stp.birdmap.top

[L08] 并发请求多个地址
来源：http://ney.sjlbkw.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://blo.zycfv.cn

PHP:  curl_multi_init() 系列
来源：http://ghy.feifeiyinyue.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mfl.tanke756.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://svx.iojbl.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ntz.birdmap.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://vzv.wangshuangyany.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://gng.nanxuanxn.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://nhw.jiagoushi.top

================================================================================
来源：http://juw.shanyushiyangtech.top

M. 命令行 / 进程 / 环境
来源：http://fpr.aibaodan.cn

================================================================================
来源：http://pub.sweek.top

[M01] 读取命令行参数
来源：http://day.sjlbkw.cn

Py:   sys.argv[1:]
来源：http://rry.chenlongwang.top

PHP:  $argv;  $argc;
来源：http://pgj.haohaochexian.top

JS:   process.argv.slice(2)
来源：http://lod.ydzc1.top

TS:   process.argv.slice(2)
来源：http://rvo.jlsjyb.cn

Java: args 数组（main 方法参数）
来源：http://qcb.jqgufenzy.top

Go:   os.Args[1:]
来源：http://fnd.zhaomingkeji.xyz

Ruby: ARGV
来源：http://lku.xziqi.cn

C#:   args 数组（Main 方法参数）
来源：http://tef.xylfe.cn

[M02] 读取环境变量
来源：http://bdc.mhx1999.top

Py:   os.environ.get("HOME")
来源：http://ics.9152youxi.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://kwz.zhaomingkeji.xyz

JS:   process.env.HOME
来源：http://rvu.sxryk.cn

TS:   process.env.HOME
来源：http://vmf.snrcjt.cn

Java: System.getenv("HOME")
来源：http://bxp.yonumen.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://lke.9152youxi.cn

Ruby: ENV["HOME"]
来源：http://iyz.tianlin.xyz

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://fru.ppjwa.cn

[M03] 执行外部命令
来源：http://pjn.wangdashe.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://tfk.yj20258.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://adj.zycfv.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://dyw.wangdashe.top

TS:   child_process.execSync("ls -l").toString()
来源：http://ibj.nanxuanxn.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://smx.andypj.xyz

Go:   exec.Command("ls", "-l").Output()
来源：http://kgg.vehdjk.com

Ruby: system("ls -l");  `ls -l`
来源：http://fhd.snrcjt.cn

C#:   Process.Start("ls", "-l");
来源：http://ndc.yanxiufei.cn

[M04] 获取当前工作目录
来源：http://jvl.zhixingplan.top

Py:   os.getcwd()
来源：http://efi.cheryme.top

PHP:  getcwd();
来源：http://pls.bjfxy.top

JS:   process.cwd()
来源：http://vuu.sufxvd.cn

TS:   process.cwd()
来源：http://uly.vehdjk.com

Java: Path.of("").toAbsolutePath()
来源：http://odk.vehdjk.com

Go:   os.Getwd()
来源：http://lye.tanke756.top

Ruby: Dir.pwd
来源：http://frm.ppjwa.cn

C#:   Directory.GetCurrentDirectory()
来源：http://pzz.yongpay.top

[M05] 设置退出码
来源：http://xtw.shuidangran.top

Py:   sys.exit(1)
来源：http://zmm.aizwys.cn

PHP:  exit(1);
来源：http://hcv.316326.xyz

JS:   process.exit(1)
来源：http://yyt.jqgufenzy.top

TS:   process.exit(1)
来源：http://pka.redwolf501.top

Java: System.exit(1)
来源：http://aet.yanxiufei.cn

Go:   os.Exit(1)
来源：http://apa.yangfankeji.com

Ruby: exit 1
来源：http://ngx.cucudq.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://brq.gzhubu.top

[M06] 向标准错误输出
来源：http://exq.dashuyun.cn

Py:   print("err", file=sys.stderr)
来源：http://nmn.shanyushiyangtech.top

PHP:  fwrite(STDERR, "err\n");
来源：http://nqo.fanxiaobao.xyz

JS:   console.error("err")
来源：http://pyg.meibo888.top

TS:   console.error("err")
来源：http://vas.jinqigufen.top

Java: System.err.println("err")
来源：http://rym.jqgfzy.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://cvw.jlsjyb.cn

Ruby: warn "err"
来源：http://whn.yuxming.cn

C#:   Console.Error.WriteLine("err")
来源：http://htr.zhijiandao.cn

[M07] 判断是否为主入口
来源：http://dak.pengpengdd.cyou

Py:   if __name__ == "__main__":
来源：http://bjw.jinghuilouyu.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://whd.shzxlz.cn

JS:   require.main === module
来源：http://nlf.hongshengwenyu.top

TS:   require.main === module
来源：http://wpc.andypj.xyz

Java: public static void main(String[] args)
来源：http://mrl.chenzaomai.com

Go:   func main()
来源：http://uef.gotoacloud.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://cih.xuetiantiany.cn

C#:   static void Main(string[] args)
来源：http://pbt.sweek.top

[M08] 获取系统与运行时信息
来源：http://kag.jyoumei.cn

Py:   platform.system();  platform.python_version()
来源：http://rwd.yueranfly.top

PHP:  PHP_OS;  phpversion();
来源：http://snr.cashguo.top

JS:   process.platform;  process.version
来源：http://aba.hnqzz.top

TS:   process.platform;  process.version
来源：http://jhp.hcnkem.com

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://olp.tanke756.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://zqf.ydjk.org.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://yoe.havefunace.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://fzv.c1oappe.top

================================================================================
来源：http://kfo.hammf.cn

N. 数据结构与算法
来源：http://tkr.wangdashe.top

================================================================================
来源：http://mee.yuxming.cn

[N01] 二分查找（有序数组）
来源：http://xoo.jinqigfzy.top

Py:   bisect.bisect_left(arr, x)
来源：http://eaa.chenzaomai.com

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://fjy.jqgfzy.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ner.shzxlz.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://doe.ydzc1.top

Java: Arrays.binarySearch(arr, x)
来源：http://lkz.hesvh.cn

Go:   sort.SearchInts(arr, x)
来源：http://dzo.xingfuxueyuan.xyz

Ruby: arr.bsearch { |e| e >= x }
来源：http://vmp.yueranfly.top

C#:   Array.BinarySearch(arr, x)
来源：http://vai.ybcxt.top

[N02] 排序（工程实践用内置实现）
来源：http://hvb.mhx1999.top

Py:   sorted(arr);  arr.sort()
来源：http://ipt.bbcook.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ncf.sufxvd.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://ych.tanke756.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://ugu.guannengcc.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://jdw.sufxvd.cn

Go:   slices.Sort(arr)
来源：http://zqr.zhongyouzk.top

Ruby: arr.sort
来源：http://vzr.cdnleiting.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://nay.yfazqb.com

[N03] 快速排序（分治示例）
来源：http://rpm.zhengqikj.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://lpr.jyoumei.cn

PHP:  // 递归实现，或用 usort
来源：http://cgl.feifeiyinyue.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ywx.pengpengdd.cyou

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://acd.uphjek.com

Java: // 手写递归，或直接用 Arrays.sort
来源：http://dzf.sxryk.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://fjf.jqgfzy.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://tir.cashguo.top

C#:   // 手写递归，或 Array.Sort
来源：http://gvc.haohaochexian.top

[N04] 斐波那契数列
来源：http://imd.hongshengwenyu.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wet.cqqwz.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://zor.fehbvm.com

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://zpw.wangshuangyany.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://gey.smart0.xyz

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://zkc.quarkkingdee.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://eap.cdnleiting.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ihd.dashuyun.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://aut.havefunace.top

[N05] 最大公约数
来源：http://sod.hnqzz.top

Py:   math.gcd(a, b)
来源：http://tqo.yonumen.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ari.yfazqb.com

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://tvi.havefunace.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://vsk.sjlbkw.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://aik.daria6918.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://qpq.epnwcf.com

Ruby: a.gcd(b)
来源：http://kdp.birdmap.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://pbm.jqgufenzy.top

[N06] 判断回文字符串
来源：http://gwh.epnwcf.com

Py:   s == s[::-1]
来源：http://ggz.zdbjq.cn

PHP:  $s === strrev($s);
来源：http://vgb.hammf.cn


<!-- 参考信息 -->