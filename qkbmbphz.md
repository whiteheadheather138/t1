代发 wailian999

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://xvn.yvedp.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://myy.yueranfly.top

[J09] 时区处理
来源：http://wrz.aibaodan.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://vpr.hnqzz.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://xvg.xuetiantiany.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://pte.zhoulong.xyz

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://boz.fanxiaobao.xyz

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ygp.birdmap.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://vgz.yanxiufei.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://brw.sjlbkw.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://paj.jiagoushi.top

[J10] 取今天 / 本月第一天
来源：http://uli.chenlongwang.top

Py:   date.today();  date.today().replace(day=1)
来源：http://cnr.shuidangran.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://wek.chenzaomai.com

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://vtr.ybcxt.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://umo.hongshengwenyu.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://lym.sxryk.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ovf.pycfn.com

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://nvp.pycfn.com

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://yxe.dianchejie.cn

================================================================================
来源：http://gup.pengpengdd.cyou

K. JSON 与序列化
来源：http://zkn.316326.xyz

================================================================================
来源：http://cpq.xuanzx.com

[K01] 对象转 JSON 字符串
来源：http://jeq.epnwcf.com

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://wmp.nwbrower.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://gdg.zhijiandao.cn

JS:   JSON.stringify(obj)
来源：http://kdj.hfpthk.cn

TS:   JSON.stringify(obj)
来源：http://tvc.hcnkem.com

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://tjs.sysykeji.top

Go:   json.Marshal(obj)
来源：http://osw.hnxiangtu.top

Ruby: obj.to_json                                     // require "json"
来源：http://gan.hnqzz.top

C#:   JsonSerializer.Serialize(obj)
来源：http://esi.havefunace.top

[K02] JSON 字符串转对象
来源：http://dte.cashguo.top

Py:   json.loads(s)
来源：http://att.gaohongyu789.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://gde.sysykeji.top

JS:   JSON.parse(s)
来源：http://ifd.52xcode.cn

TS:   JSON.parse(s)
来源：http://ino.zhiwuduotai.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://oop.yanxiufei.cn

Go:   json.Unmarshal(data, &v)
来源：http://srv.feifeiyinyue.top

Ruby: JSON.parse(s)
来源：http://xzq.guannengcc.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://nxj.ydzc1.top

[K03] JSON 美化输出（带缩进）
来源：http://aot.jqgfzy.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://zfl.fktsv.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://jvr.tarul.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://pdg.uphjek.com

TS:   JSON.stringify(obj, null, 2)
来源：http://paz.yj20258.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://yyg.chenzaomai.com

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://vjs.cqqwz.cn

Ruby: JSON.pretty_generate(obj)
来源：http://lwg.wangdashe.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://vod.chenzaomai.com

[K04] 读取 JSON 文件
来源：http://tom.fehbvm.com

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ncd.yongpay.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://zqj.jinqigufen.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://spq.quarkkingdee.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://nfm.nanxuanxn.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://trd.guannengcc.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://tnh.yvedp.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://pvy.dianchejie.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://jmj.chenlongwang.top

[K05] 深拷贝对象
来源：http://hnf.jinqigfzy.top

Py:   copy.deepcopy(obj)
来源：http://fnc.aizwys.cn

PHP:  unserialize(serialize($obj));
来源：http://ixl.redwolf501.top

JS:   structuredClone(obj)
来源：http://yyx.fengsongda.top

TS:   structuredClone(obj)
来源：http://dez.hcnkem.com

Java: // 手写拷贝构造，或序列化往返
来源：http://rjq.wangdashe.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ogh.jqgufenzy.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://yrn.yvedp.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://gfp.epnwcf.com

[K06] 解析 URL 查询串
来源：http://ogl.gotoacloud.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wpj.sysykeji.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://rwf.yvedp.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wkd.chenjidiqi.icu

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ejn.pycfn.com

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ttl.ybcxt.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://bjg.ywan-chungtsiang.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ipy.ywan-chungtsiang.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://rll.52xcode.cn

[K07] 进制转换
来源：http://smm.nanxuanxn.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://usy.xinyue.icu

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://frq.fengsongda.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://cvv.zhijiandao.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://nff.hnqzz.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://gpl.hfpthk.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://fse.ybcxt.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://dij.yj202588.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://qqw.cheryme.top

[K08] 二进制序列化（非 JSON）
来源：http://uyl.tian-w.cn

Py:   pickle.dumps(obj)
来源：http://toz.tian-w.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://fdf.316326.xyz

JS:   v8.serialize(obj)        // Node
来源：http://zwq.ehwqpu.com

TS:   v8.serialize(obj)        // Node
来源：http://ywt.guannengcc.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://yjn.shzxlz.cn

Go:   encoding/gob
来源：http://rdd.ehwqpu.com

Ruby: Marshal.dump(obj)
来源：http://nwe.hesvh.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://rug.aibaodan.cn

================================================================================
来源：http://sog.jinghuilouyu.cn

L. 网络请求
来源：http://kfx.hnxiangtu.top

================================================================================
来源：http://edi.cucudq.cn

[L01] 发送 GET 请求
来源：http://agq.zhoulong.xyz

Py:   requests.get(url)                        # 第三方库 requests
来源：http://aph.bjfxy.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://tbo.uphjek.com

JS:   await fetch(url)
来源：http://ojl.jinqigufen.top

TS:   await fetch(url)
来源：http://ans.kuanghao11.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ech.jqgufenzy.top

Go:   resp, err := http.Get(url)
来源：http://bjl.dianchejie.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://kxo.0kj1m.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://oqs.wangdashe.top

[L02] 发送 POST JSON
来源：http://cpz.pycfn.com

Py:   requests.post(url, json={"a": 1})
来源：http://ciq.cheryme.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://dhi.jiagoushi.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://eaq.yj202588.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://tkt.haohaochexian.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://vqv.birdmap.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://lat.ehwqpu.com

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ijo.yj20258.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://rda.chenjidiqi.icu

[L03] 设置自定义请求头
来源：http://irf.cucudq.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://puk.sufxvd.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://qto.zdbjq.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://lic.aizwys.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://zgt.hnxiangtu.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://rve.chenjidiqi.icu

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://jyv.hongshengwenyu.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wvt.shanyushiyangkeji.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://dae.guowangkeji.top

[L04] 设置超时
来源：http://chz.yvedp.cn

Py:   requests.get(url, timeout=5)
来源：http://ppg.ydzc1.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://lrt.xylfe.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://tgp.hesvh.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://joo.fehbvm.com

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://zcs.yueranfly.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://tqs.tianlin.xyz

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://bkj.quarkkingdee.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://doz.ydzc1.top

[L05] 上传文件（multipart）
来源：http://zsp.xingfuxueyuan.xyz

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://zyl.yangfankeji.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://pud.xuanzx.com

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://qre.daria6918.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ucd.gogol.net.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://bxh.fanxiaobao.xyz

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ojc.yangfankeji.com

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://eoj.quarkkingdee.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://dfy.redwolf501.top

[L06] 解析响应为 JSON
来源：http://zid.havefunace.top

Py:   resp.json()
来源：http://xfl.dianchejie.cn

PHP:  json_decode($body, true);
来源：http://gyg.ydzc1.top

JS:   await resp.json()
来源：http://bke.hfpthk.cn

TS:   await resp.json()
来源：http://nrq.zhijiandao.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://iqs.fanxiaobao.xyz

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://zot.tianlin.xyz

Ruby: JSON.parse(resp.body)
来源：http://dks.shanyushiyangkeji.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://oml.jinqigufen.top

[L07] 处理 HTTP 状态码
来源：http://rty.cashguo.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ryp.gaohongyu789.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://tbf.yueranfly.top

JS:   resp.ok;  resp.status
来源：http://rza.xinyue.icu

TS:   resp.ok;  resp.status
来源：http://aiv.yongpay.top

Java: resp.statusCode()
来源：http://gok.vqdsnc.cn

Go:   resp.StatusCode
来源：http://ovm.ppjwa.cn

Ruby: resp.code.to_i
来源：http://hhe.ctjpmb.com

C#:   (int)resp.StatusCode
来源：http://wzw.cucudq.cn

[L08] 并发请求多个地址
来源：http://axv.ctjpmb.com

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ibr.ivvv.top

PHP:  curl_multi_init() 系列
来源：http://tlc.fzhhl.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ixw.zhongyouzk.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://gqj.gaohongyu789.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://krs.sysykeji.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://gee.ydzc1.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://xci.fktsv.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wna.zdqjudy.top

================================================================================
来源：http://oit.jyoumei.cn

M. 命令行 / 进程 / 环境
来源：http://bzr.fanxiaobao.xyz

================================================================================
来源：http://cjm.shuidangran.top

[M01] 读取命令行参数
来源：http://kbs.ydjk.org.cn

Py:   sys.argv[1:]
来源：http://ijv.cqqwz.cn

PHP:  $argv;  $argc;
来源：http://kah.cheryme.top

JS:   process.argv.slice(2)
来源：http://vqe.yj202588.top

TS:   process.argv.slice(2)
来源：http://grn.gzhubu.top

Java: args 数组（main 方法参数）
来源：http://iki.fktsv.cn

Go:   os.Args[1:]
来源：http://qbl.vehdjk.com

Ruby: ARGV
来源：http://muy.nanxuanxn.top

C#:   args 数组（Main 方法参数）
来源：http://rrw.cashguo.top

[M02] 读取环境变量
来源：http://dxt.nanxinkj.top

Py:   os.environ.get("HOME")
来源：http://yvv.wangshuangyany.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://tqj.sxryk.cn

JS:   process.env.HOME
来源：http://sws.guannengcc.top

TS:   process.env.HOME
来源：http://yxg.gotoacloud.top

Java: System.getenv("HOME")
来源：http://umc.shuidangran.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://omp.xziqi.cn

Ruby: ENV["HOME"]
来源：http://vlg.ctjpmb.com

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://suq.chenzaomai.com

[M03] 执行外部命令
来源：http://fwr.fanxiaobao.xyz

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://vkc.yj202588.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://xjc.svipenyu.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://gum.epnwcf.com

TS:   child_process.execSync("ls -l").toString()
来源：http://rlg.hywenlv.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mzt.cqqwz.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://ucd.xuanzx.com

Ruby: system("ls -l");  `ls -l`
来源：http://tha.aizwys.cn

C#:   Process.Start("ls", "-l");
来源：http://gtl.gotoacloud.top

[M04] 获取当前工作目录
来源：http://kwv.nanxinkj.top

Py:   os.getcwd()
来源：http://dux.guowangkeji.top

PHP:  getcwd();
来源：http://jvb.shuidangran.top

JS:   process.cwd()
来源：http://hhs.nanxinkj.top

TS:   process.cwd()
来源：http://kkf.jianghu66.top

Java: Path.of("").toAbsolutePath()
来源：http://wcs.fengsongda.top

Go:   os.Getwd()
来源：http://pvb.zdqjudy.top

Ruby: Dir.pwd
来源：http://odj.nanxuanxn.top

C#:   Directory.GetCurrentDirectory()
来源：http://amd.aizwys.cn

[M05] 设置退出码
来源：http://lwj.jlsjyb.cn

Py:   sys.exit(1)
来源：http://vdy.xylfe.cn

PHP:  exit(1);
来源：http://jlw.xingfuxueyuan.xyz

JS:   process.exit(1)
来源：http://kdq.vehdjk.com

TS:   process.exit(1)
来源：http://lur.ydjk.org.cn

Java: System.exit(1)
来源：http://ois.sjlbkw.cn

Go:   os.Exit(1)
来源：http://wlg.yonumen.top

Ruby: exit 1
来源：http://yzi.haohaochexian.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://aim.52xcode.cn

[M06] 向标准错误输出
来源：http://pyl.dianchejie.cn

Py:   print("err", file=sys.stderr)
来源：http://rwv.cqqwz.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://txk.ywan-chungtsiang.top

JS:   console.error("err")
来源：http://exn.cheryme.top

TS:   console.error("err")
来源：http://cqb.havefunace.top

Java: System.err.println("err")
来源：http://uti.zhiwuduotai.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ksi.havefunace.top

Ruby: warn "err"
来源：http://ncr.xziqi.cn

C#:   Console.Error.WriteLine("err")
来源：http://chm.xylfe.cn

[M07] 判断是否为主入口
来源：http://xik.shzxlz.cn

Py:   if __name__ == "__main__":
来源：http://dch.sjlbkw.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ice.fehbvm.com

JS:   require.main === module
来源：http://fwh.bjfxy.top

TS:   require.main === module
来源：http://heb.tarul.cn

Java: public static void main(String[] args)
来源：http://udt.iojbl.cn

Go:   func main()
来源：http://toh.zdbjq.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://jyh.feifeiyinyue.top

C#:   static void Main(string[] args)
来源：http://goq.hysaishi.cn

[M08] 获取系统与运行时信息
来源：http://mqx.xuanzx.com

Py:   platform.system();  platform.python_version()
来源：http://fvc.sysykeji.top

PHP:  PHP_OS;  phpversion();
来源：http://osa.yanxiufei.cn

JS:   process.platform;  process.version
来源：http://opn.shanyushiyangkeji.top

TS:   process.platform;  process.version
来源：http://ugj.xinyue.icu

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://nsx.sjlbkw.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://tgl.wangdashe.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ppo.ydjk.org.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://umx.sweek.top

================================================================================
来源：http://hul.52xcode.cn

N. 数据结构与算法
来源：http://pkf.cdnleiting.top

================================================================================
来源：http://iwy.yj20258.top

[N01] 二分查找（有序数组）
来源：http://mso.tianlin.xyz

Py:   bisect.bisect_left(arr, x)
来源：http://joz.jqgufenzy.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://uyq.chenzaomai.com

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://cyv.andypj.xyz

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mkv.shuidangran.top

Java: Arrays.binarySearch(arr, x)
来源：http://nal.bbcook.cn

Go:   sort.SearchInts(arr, x)
来源：http://dsd.bbcook.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://mjn.ydjk.org.cn

C#:   Array.BinarySearch(arr, x)
来源：http://rnd.gogol.net.cn

[N02] 排序（工程实践用内置实现）
来源：http://iii.dashuyun.cn

Py:   sorted(arr);  arr.sort()
来源：http://grv.aizwys.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ysq.yueranfly.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://xfv.chenjidiqi.icu

TS:   [...arr].sort((a, b) => a - b)
来源：http://qgg.bjfxy.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://zag.jyoumei.cn

Go:   slices.Sort(arr)
来源：http://axr.hywenlv.cn

Ruby: arr.sort
来源：http://tln.zhoulong.xyz

C#:   Array.Sort(arr);  list.Sort()
来源：http://gcp.zycfv.cn

[N03] 快速排序（分治示例）
来源：http://yin.wangdashe.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mxi.zhengqikj.top

PHP:  // 递归实现，或用 usort
来源：http://vit.yj202588.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://rpk.hongshengwenyu.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://dkn.jiagoushi.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://azc.gogol.net.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://kkh.haohaochexian.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://qnm.chenzaomai.com

C#:   // 手写递归，或 Array.Sort
来源：http://yyf.fengsongda.top

[N04] 斐波那契数列
来源：http://ckb.zhoulong.xyz

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hby.feifeiyinyue.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://akq.haohaochexian.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ivo.c1oappe.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://jqr.fengsongda.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://imt.zhaomingkeji.xyz

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://kwg.shangyingyoupin.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ppd.hysaishi.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ibm.yj202588.top

[N05] 最大公约数
来源：http://cji.zhoulong.xyz

Py:   math.gcd(a, b)
来源：http://pgg.zhijiandao.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://bsw.cheryme.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://jcp.xziqi.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ejc.fanxiaobao.xyz

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://uam.redwolf501.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://zsg.uphjek.com

Ruby: a.gcd(b)
来源：http://eja.aizwys.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://jcr.fktsv.cn

[N06] 判断回文字符串
来源：http://deq.fehbvm.com

Py:   s == s[::-1]
来源：http://oil.ctjpmb.com

PHP:  $s === strrev($s);
来源：http://fwq.zdbjq.cn

JS:   s === [...s].reverse().join("")
来源：http://qmv.xuanzx.com

TS:   s === [...s].reverse().join("")
来源：http://dfb.hcnkem.com

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://bae.jinghuilouyu.cn

Go:   // 双指针从两端比较
来源：http://obr.snrcjt.cn


<!-- 参考信息 -->