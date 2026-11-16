代发 wailian999

C#:   d1 < d2;  d1 == d2
来源：http://eqi.yj20258.top

[J08] 提取年月日与星期
来源：http://udh.zhengqikj.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://fph.epnwcf.com

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://bpg.shuidangran.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://tge.ivvv.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://tkp.tarul.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://xkd.nanxuanxn.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://fwo.hnxiangtu.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://qia.zhengqikj.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://wvl.wangdashe.top

[J09] 时区处理
来源：http://xkx.yuxming.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ago.ydjk.org.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://xax.yangfankeji.com

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://pju.jiagoushi.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hbq.daxiang520.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://iln.sweek.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://qya.aibaodan.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://ezi.hesvh.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://dme.shuidangran.top

[J10] 取今天 / 本月第一天
来源：http://ilv.zhijiandao.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://tsi.hysaishi.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://qzq.epnwcf.com

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://iyq.dashuyun.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://njt.hywenlv.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ell.ehwqpu.com

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://gbr.yuxming.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://oej.snrcjt.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://tfu.hnxiangtu.top

================================================================================
来源：http://ust.hysaishi.cn

K. JSON 与序列化
来源：http://ije.jiagoushi.top

================================================================================
来源：http://eeu.vqdsnc.cn

[K01] 对象转 JSON 字符串
来源：http://smn.sjlbkw.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ofk.jianghu66.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://pfu.jqgufenzy.top

JS:   JSON.stringify(obj)
来源：http://pbq.jlsjyb.cn

TS:   JSON.stringify(obj)
来源：http://ehz.jinghuilouyu.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://kge.yongpay.top

Go:   json.Marshal(obj)
来源：http://ibb.chenjidiqi.icu

Ruby: obj.to_json                                     // require "json"
来源：http://box.ywan-chungtsiang.top

C#:   JsonSerializer.Serialize(obj)
来源：http://wbr.yj20258888.top

[K02] JSON 字符串转对象
来源：http://nsz.pengpengdd.cyou

Py:   json.loads(s)
来源：http://vru.iojbl.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://tgh.iojbl.cn

JS:   JSON.parse(s)
来源：http://hij.gogol.net.cn

TS:   JSON.parse(s)
来源：http://rdn.jianghu66.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://lzy.zhaomingkeji.xyz

Go:   json.Unmarshal(data, &v)
来源：http://zen.hysaishi.cn

Ruby: JSON.parse(s)
来源：http://vjr.mhx1999.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://vgr.cheryme.top

[K03] JSON 美化输出（带缩进）
来源：http://wah.gotoacloud.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ppr.yuxming.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wpo.cucudq.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://uor.chenjidiqi.icu

TS:   JSON.stringify(obj, null, 2)
来源：http://rvu.yongpay.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://czi.yfazqb.com

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://xbe.yueranfly.top

Ruby: JSON.pretty_generate(obj)
来源：http://pgn.xuanzx.com

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://yli.guannengcc.top

[K04] 读取 JSON 文件
来源：http://nbz.zhiwuduotai.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://vfp.cashguo.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://cqo.nwbrower.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://uhk.redwolf501.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://llj.aizwys.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://rxc.xylfe.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://exr.andypj.xyz

Ruby: JSON.parse(File.read("a.json"))
来源：http://unj.epnwcf.com

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://tuj.gotoacloud.top

[K05] 深拷贝对象
来源：http://kyf.ybcxt.top

Py:   copy.deepcopy(obj)
来源：http://inq.52xcode.cn

PHP:  unserialize(serialize($obj));
来源：http://cqk.ctjpmb.com

JS:   structuredClone(obj)
来源：http://lbn.svipenyu.cn

TS:   structuredClone(obj)
来源：http://obc.daxiang520.top

Java: // 手写拷贝构造，或序列化往返
来源：http://kyf.dashuyun.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://qef.zhongyouzk.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://slv.cucudq.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://xkf.ehwqpu.com

[K06] 解析 URL 查询串
来源：http://ekd.guowangkeji.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ahl.vqdsnc.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://skm.sufxvd.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://drj.haohaochexian.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://gsq.zdbjq.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://iyg.hnxiangtu.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://ebh.dianchejie.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://oax.chenjidiqi.icu

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://czv.sweek.top

[K07] 进制转换
来源：http://rxn.yvedp.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://kpq.yanxiufei.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://fqb.jianghu66.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://jkv.redwolf501.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://yky.shanyushiyangtech.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://qnm.hesvh.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://gjz.ydzc1.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://owi.kuanghao11.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://grk.ivvv.top

[K08] 二进制序列化（非 JSON）
来源：http://isy.jqgufenzy.top

Py:   pickle.dumps(obj)
来源：http://ubc.jlsjyb.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://rak.cucudq.cn

JS:   v8.serialize(obj)        // Node
来源：http://xpq.nanxuanxn.top

TS:   v8.serialize(obj)        // Node
来源：http://qkl.hnxiangtu.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://iat.shuidangran.top

Go:   encoding/gob
来源：http://ens.smart0.xyz

Ruby: Marshal.dump(obj)
来源：http://llc.yvedp.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://nnn.guowangkeji.top

================================================================================
来源：http://exs.vqdsnc.cn

L. 网络请求
来源：http://blj.vqdsnc.cn

================================================================================
来源：http://ihf.cashguo.top

[L01] 发送 GET 请求
来源：http://hgc.hnxiangtu.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://pzx.cdnleiting.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://mnp.sxryk.cn

JS:   await fetch(url)
来源：http://zbj.ydjk.org.cn

TS:   await fetch(url)
来源：http://jeg.epnwcf.com

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://jeu.havefunace.top

Go:   resp, err := http.Get(url)
来源：http://jub.jiagoushi.top

Ruby: Net::HTTP.get(URI(url))
来源：http://sxl.zhongyouzk.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://pos.ppjwa.cn

[L02] 发送 POST JSON
来源：http://mpp.vehdjk.com

Py:   requests.post(url, json={"a": 1})
来源：http://dli.guannengcc.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://uch.dashuyun.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://emp.jinghuilouyu.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://qqw.ydzc1.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://jml.tanke756.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://uku.birdmap.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://bgg.quarkkingdee.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://eko.cdnleiting.top

[L03] 设置自定义请求头
来源：http://zjt.0kj1m.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wew.shanyushiyangtech.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://vbh.dianchejie.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wal.feifeiyinyue.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://anp.jqgfzy.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://twy.zhengqikj.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://jax.smart0.xyz

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hrh.jinyuanbaomall.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ndi.hysaishi.cn

[L04] 设置超时
来源：http://qod.zdbjq.cn

Py:   requests.get(url, timeout=5)
来源：http://gvi.snrcjt.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://pta.gzhubu.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://vry.zhongyouzk.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://usk.zhoulong.xyz

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://xhb.mhx1999.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://xaq.xingfuxueyuan.xyz

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ohv.jiagoushi.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://urb.52xcode.cn

[L05] 上传文件（multipart）
来源：http://zei.yonumen.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://lbn.gogol.net.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://gak.xingfuxueyuan.xyz

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://jud.ctjpmb.com

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://jvl.0kj1m.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://nge.tarul.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://paf.shangyingyoupin.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hfr.nanxuanxn.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://kra.bjfxy.top

[L06] 解析响应为 JSON
来源：http://dvs.cqqwz.cn

Py:   resp.json()
来源：http://zpz.xinyue.icu

PHP:  json_decode($body, true);
来源：http://zur.gotoacloud.top

JS:   await resp.json()
来源：http://kts.cucudq.cn

TS:   await resp.json()
来源：http://dxb.ybcxt.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://kuz.guowangkeji.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://pht.shangyingyoupin.top

Ruby: JSON.parse(resp.body)
来源：http://mnm.aibaodan.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://odh.bjfxy.top

[L07] 处理 HTTP 状态码
来源：http://iqn.bjfxy.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://pye.zdqjudy.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://qyg.yanxiufei.cn

JS:   resp.ok;  resp.status
来源：http://oqi.hysaishi.cn

TS:   resp.ok;  resp.status
来源：http://mmq.yonumen.top

Java: resp.statusCode()
来源：http://bfm.52xcode.cn

Go:   resp.StatusCode
来源：http://dho.fanxiaobao.xyz

Ruby: resp.code.to_i
来源：http://qpl.yueranfly.top

C#:   (int)resp.StatusCode
来源：http://kfj.xinyue.icu

[L08] 并发请求多个地址
来源：http://mxk.vqdsnc.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://iwz.nanxuanxn.top

PHP:  curl_multi_init() 系列
来源：http://qdu.smart0.xyz

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://gcs.aizwys.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://tpc.52xcode.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://rge.havefunace.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://rxl.yvedp.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ouj.yonumen.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://luy.daria6918.cn

================================================================================
来源：http://wog.sufxvd.cn

M. 命令行 / 进程 / 环境
来源：http://lzq.fktsv.cn

================================================================================
来源：http://dtw.shanyushiyangkeji.top

[M01] 读取命令行参数
来源：http://csr.yongpay.top

Py:   sys.argv[1:]
来源：http://ahz.yfazqb.com

PHP:  $argv;  $argc;
来源：http://coy.shzxlz.cn

JS:   process.argv.slice(2)
来源：http://ruz.zdbjq.cn

TS:   process.argv.slice(2)
来源：http://rkk.fehbvm.com

Java: args 数组（main 方法参数）
来源：http://xuu.316326.xyz

Go:   os.Args[1:]
来源：http://aae.epnwcf.com

Ruby: ARGV
来源：http://wfk.jinqigfzy.top

C#:   args 数组（Main 方法参数）
来源：http://wfq.zhengqikj.top

[M02] 读取环境变量
来源：http://gxz.shanyushiyangtech.top

Py:   os.environ.get("HOME")
来源：http://jyo.fengsongda.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://rke.wangdashe.top

JS:   process.env.HOME
来源：http://yix.jinghuilouyu.cn

TS:   process.env.HOME
来源：http://kvq.zdqjudy.top

Java: System.getenv("HOME")
来源：http://kzi.xinyue.icu

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://vyg.wangshuangyany.cn

Ruby: ENV["HOME"]
来源：http://wzf.jianghu66.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://kag.andypj.xyz

[M03] 执行外部命令
来源：http://zki.yfazqb.com

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ojw.shangyingyoupin.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ydr.hammf.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://ovt.yuanzhike.top

TS:   child_process.execSync("ls -l").toString()
来源：http://bbs.hywenlv.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ufm.bbcook.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://qzr.guannengcc.top

Ruby: system("ls -l");  `ls -l`
来源：http://oiq.hammf.cn

C#:   Process.Start("ls", "-l");
来源：http://jje.yj202588.top

[M04] 获取当前工作目录
来源：http://zjj.yvedp.cn

Py:   os.getcwd()
来源：http://cyg.birdmap.top

PHP:  getcwd();
来源：http://smd.yj20258.top

JS:   process.cwd()
来源：http://lrc.pycfn.com

TS:   process.cwd()
来源：http://lfx.birdmap.top

Java: Path.of("").toAbsolutePath()
来源：http://fwh.aibaodan.cn

Go:   os.Getwd()
来源：http://mlh.ydjk.org.cn

Ruby: Dir.pwd
来源：http://esf.haohaochexian.top

C#:   Directory.GetCurrentDirectory()
来源：http://unh.hcnkem.com

[M05] 设置退出码
来源：http://ekb.snrcjt.cn

Py:   sys.exit(1)
来源：http://axd.ybcxt.top

PHP:  exit(1);
来源：http://khw.daria6918.cn

JS:   process.exit(1)
来源：http://qwz.yj20258888.top

TS:   process.exit(1)
来源：http://yzy.chenzaomai.com

Java: System.exit(1)
来源：http://udp.yueranfly.top

Go:   os.Exit(1)
来源：http://yka.yanxiufei.cn

Ruby: exit 1
来源：http://lpt.hongshengwenyu.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ifl.yangfankeji.com

[M06] 向标准错误输出
来源：http://tja.gotoacloud.top

Py:   print("err", file=sys.stderr)
来源：http://rsf.yangfankeji.com

PHP:  fwrite(STDERR, "err\n");
来源：http://szj.pycfn.com

JS:   console.error("err")
来源：http://kfm.gogol.net.cn

TS:   console.error("err")
来源：http://ysx.ydjk.org.cn

Java: System.err.println("err")
来源：http://uab.zycfv.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://gcn.zycfv.cn

Ruby: warn "err"
来源：http://jgw.wangshuangyany.cn

C#:   Console.Error.WriteLine("err")
来源：http://jsi.sjlbkw.cn

[M07] 判断是否为主入口
来源：http://njm.tarul.cn

Py:   if __name__ == "__main__":
来源：http://gxi.smart0.xyz

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://kir.shangyingyoupin.top

JS:   require.main === module
来源：http://mms.redwolf501.top

TS:   require.main === module
来源：http://qqk.yj202588.top

Java: public static void main(String[] args)
来源：http://grf.jlsjyb.cn

Go:   func main()
来源：http://wsd.hcnkem.com

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://fmx.xinyue.icu

C#:   static void Main(string[] args)
来源：http://edm.fehbvm.com

[M08] 获取系统与运行时信息
来源：http://zrq.sxryk.cn

Py:   platform.system();  platform.python_version()
来源：http://bjb.zhiwuduotai.top

PHP:  PHP_OS;  phpversion();
来源：http://kdf.aizwys.cn

JS:   process.platform;  process.version
来源：http://oho.smart0.xyz

TS:   process.platform;  process.version
来源：http://wiw.chenjidiqi.icu

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://tza.zdbjq.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://pai.feifeiyinyue.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://zyh.jlsjyb.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://mgo.daxiang520.top

================================================================================
来源：http://rwk.sjlbkw.cn

N. 数据结构与算法
来源：http://xzm.cucudq.cn

================================================================================
来源：http://owk.gotoacloud.top

[N01] 二分查找（有序数组）
来源：http://bet.jlsjyb.cn

Py:   bisect.bisect_left(arr, x)
来源：http://ocx.ydzc1.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://kjd.cqqwz.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://rqb.yj202588.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://haa.yj20258888.top

Java: Arrays.binarySearch(arr, x)
来源：http://euk.cheryme.top

Go:   sort.SearchInts(arr, x)
来源：http://csm.uphjek.com

Ruby: arr.bsearch { |e| e >= x }
来源：http://ova.xinyue.icu

C#:   Array.BinarySearch(arr, x)
来源：http://ufs.jqgufenzy.top

[N02] 排序（工程实践用内置实现）
来源：http://glb.cqqwz.cn

Py:   sorted(arr);  arr.sort()
来源：http://ato.tianlin.xyz

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://nlc.gaohongyu789.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://esq.zdqjudy.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://ksp.cdnleiting.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://rwd.andypj.xyz

Go:   slices.Sort(arr)
来源：http://oug.hywenlv.cn

Ruby: arr.sort
来源：http://kpc.52xcode.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://oka.hnxiangtu.top

[N03] 快速排序（分治示例）
来源：http://ikz.jinyuanbaomall.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://tsc.ywan-chungtsiang.top

PHP:  // 递归实现，或用 usort
来源：http://hdm.ybcxt.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://agw.pycfn.com

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://xom.fanxiaobao.xyz

Java: // 手写递归，或直接用 Arrays.sort
来源：http://rpi.zhoulong.xyz

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://jvm.hongshengwenyu.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://bgx.c1oappe.top

C#:   // 手写递归，或 Array.Sort
来源：http://loc.xuetiantiany.cn

[N04] 斐波那契数列
来源：http://xcs.cdnleiting.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://fsr.daria6918.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://smr.fktsv.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://zmi.birdmap.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://nfx.zdbjq.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://kye.hysaishi.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://dzk.xuanzx.com

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://qjl.xziqi.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://udb.cucudq.cn

[N05] 最大公约数
来源：http://zry.redwolf501.top

Py:   math.gcd(a, b)
来源：http://jca.sysykeji.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://svs.316326.xyz

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mvk.gaohongyu789.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mvy.quarkkingdee.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://vbx.jinqigufen.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://eaq.guowangkeji.top

Ruby: a.gcd(b)
来源：http://pji.wangdashe.top


<!-- 参考信息 -->