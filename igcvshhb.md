代发 wailian999

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://dcn.vehdjk.com

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://abp.ehwqpu.com

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://gfc.hammf.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://eln.ppjwa.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://fkq.hywenlv.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://fqn.iojbl.cn

[J09] 时区处理
来源：http://xhk.yj202588.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ncb.snrcjt.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://mvv.dashuyun.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://skk.zhengqikj.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://umi.zhoulong.xyz

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://nyi.jqgfzy.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://lbu.sweek.top

Ruby: Time.now.getlocal("+08:00")
来源：http://ffk.jinyuanbaomall.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://mty.jinyuanbaomall.cn

[J10] 取今天 / 本月第一天
来源：http://xcm.cucudq.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://reu.nanxinkj.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://nnt.yj20258888.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://uvt.bbcook.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://pmf.xziqi.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://xfs.gotoacloud.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://avq.jinqigufen.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://xvn.zhoulong.xyz

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://eeb.hcnkem.com

================================================================================
来源：http://jfs.wangdashe.top

K. JSON 与序列化
来源：http://bdm.haohaochexian.top

================================================================================
来源：http://uoo.yueranfly.top

[K01] 对象转 JSON 字符串
来源：http://khl.ybcxt.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ddr.hammf.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://kwx.zhixingplan.top

JS:   JSON.stringify(obj)
来源：http://fha.hywenlv.cn

TS:   JSON.stringify(obj)
来源：http://ftd.epnwcf.com

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://iho.52xcode.cn

Go:   json.Marshal(obj)
来源：http://xdu.hesvh.cn

Ruby: obj.to_json                                     // require "json"
来源：http://thj.xingfuxueyuan.xyz

C#:   JsonSerializer.Serialize(obj)
来源：http://xxl.xylfe.cn

[K02] JSON 字符串转对象
来源：http://cwu.guowangkeji.top

Py:   json.loads(s)
来源：http://upo.havefunace.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://jbb.nanxuanxn.top

JS:   JSON.parse(s)
来源：http://nlf.feifeiyinyue.top

TS:   JSON.parse(s)
来源：http://cpp.zhoulong.xyz

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://uwd.sxryk.cn

Go:   json.Unmarshal(data, &v)
来源：http://htw.guowangkeji.top

Ruby: JSON.parse(s)
来源：http://ebx.52xcode.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://vmi.xylfe.cn

[K03] JSON 美化输出（带缩进）
来源：http://tcz.xziqi.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://uut.yvedp.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://msj.hammf.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://dcm.yonumen.top

TS:   JSON.stringify(obj, null, 2)
来源：http://pvo.yvedp.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://sip.bjfxy.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://gzn.cucudq.cn

Ruby: JSON.pretty_generate(obj)
来源：http://ipc.yj20258.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://eeg.fanxiaobao.xyz

[K04] 读取 JSON 文件
来源：http://zie.ehwqpu.com

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ghs.jinyuanbaomall.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://tpa.zdbjq.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://fae.hcnkem.com

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://idy.jianghu66.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://lbb.jianghu66.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://pmt.jinqigufen.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://fov.snrcjt.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://txq.xylfe.cn

[K05] 深拷贝对象
来源：http://wxi.ybcxt.top

Py:   copy.deepcopy(obj)
来源：http://cxq.wangshuangyany.cn

PHP:  unserialize(serialize($obj));
来源：http://mhw.yj20258.top

JS:   structuredClone(obj)
来源：http://lag.ydzc1.top

TS:   structuredClone(obj)
来源：http://iig.andypj.xyz

Java: // 手写拷贝构造，或序列化往返
来源：http://udd.jiagoushi.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://pwt.bbcook.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ozf.vehdjk.com

C#:   // 序列化往返，或自定义 Clone
来源：http://jvu.ctjpmb.com

[K06] 解析 URL 查询串
来源：http://bea.quarkkingdee.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://gby.sweek.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hnm.bjfxy.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://oih.havefunace.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://uuq.epnwcf.com

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://cfo.guannengcc.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://pfc.jinyuanbaomall.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://cmi.gzhubu.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://lhs.316326.xyz

[K07] 进制转换
来源：http://mya.hysaishi.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ytq.hongshengwenyu.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://xoz.feifeiyinyue.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://cdo.xziqi.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hbv.ydzc1.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://rle.shanyushiyangtech.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://loo.jyoumei.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://xfx.xingfuxueyuan.xyz

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://vuo.andypj.xyz

[K08] 二进制序列化（非 JSON）
来源：http://agq.jinqigufen.top

Py:   pickle.dumps(obj)
来源：http://mlg.birdmap.top

PHP:  serialize($obj);  unserialize($s);
来源：http://iiv.epnwcf.com

JS:   v8.serialize(obj)        // Node
来源：http://thi.dianchejie.cn

TS:   v8.serialize(obj)        // Node
来源：http://mbz.zdqjudy.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://cjj.epnwcf.com

Go:   encoding/gob
来源：http://lyu.fehbvm.com

Ruby: Marshal.dump(obj)
来源：http://guo.52xcode.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://iyd.chenzaomai.com

================================================================================
来源：http://ayz.jinqigufen.top

L. 网络请求
来源：http://gcx.shuidangran.top

================================================================================
来源：http://asn.yfazqb.com

[L01] 发送 GET 请求
来源：http://qnh.gotoacloud.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ipo.52xcode.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://uji.tian-w.cn

JS:   await fetch(url)
来源：http://mwx.dianchejie.cn

TS:   await fetch(url)
来源：http://adz.kuanghao11.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ice.chenjidiqi.icu

Go:   resp, err := http.Get(url)
来源：http://jja.jinqigufen.top

Ruby: Net::HTTP.get(URI(url))
来源：http://vbz.ybcxt.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://yqu.cucudq.cn

[L02] 发送 POST JSON
来源：http://lnn.jinyuanbaomall.cn

Py:   requests.post(url, json={"a": 1})
来源：http://wae.guannengcc.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://pln.yfazqb.com

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://opi.xziqi.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://sfm.pengpengdd.cyou

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ebl.meibo888.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://sfi.chenjidiqi.icu

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://oxm.c1oappe.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mfv.vqdsnc.cn

[L03] 设置自定义请求头
来源：http://dzu.aizwys.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://rqc.9152youxi.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ebb.yj20258888.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://nfc.hesvh.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://alh.guannengcc.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ruw.fengsongda.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://rox.xuetiantiany.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://fmw.ywan-chungtsiang.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://gad.shzxlz.cn

[L04] 设置超时
来源：http://fqr.ivvv.top

Py:   requests.get(url, timeout=5)
来源：http://kln.ywan-chungtsiang.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://gyb.hfpthk.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://zmf.gaohongyu789.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://bou.aizwys.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://kkh.cucudq.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ble.hesvh.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://dar.yuanzhike.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://fal.xingfuxueyuan.xyz

[L05] 上传文件（multipart）
来源：http://ogn.guannengcc.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://xtg.0kj1m.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://qej.bjfxy.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://nme.yanxiufei.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://qkp.bbcook.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://awi.shzxlz.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://roi.c1oappe.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://tjm.fzhhl.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://lri.c1oappe.top

[L06] 解析响应为 JSON
来源：http://qbj.yfazqb.com

Py:   resp.json()
来源：http://fbz.sufxvd.cn

PHP:  json_decode($body, true);
来源：http://jlh.9152youxi.cn

JS:   await resp.json()
来源：http://afv.ppjwa.cn

TS:   await resp.json()
来源：http://wlb.dianchejie.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://zyw.hfpthk.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://zvh.svipenyu.cn

Ruby: JSON.parse(resp.body)
来源：http://chs.aibaodan.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://vni.xziqi.cn

[L07] 处理 HTTP 状态码
来源：http://zxl.sweek.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://rak.guowangkeji.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://yif.vehdjk.com

JS:   resp.ok;  resp.status
来源：http://otc.ywan-chungtsiang.top

TS:   resp.ok;  resp.status
来源：http://foh.yj202588.top

Java: resp.statusCode()
来源：http://pkq.aibaodan.cn

Go:   resp.StatusCode
来源：http://ltq.zycfv.cn

Ruby: resp.code.to_i
来源：http://ath.yvedp.cn

C#:   (int)resp.StatusCode
来源：http://plt.wangdashe.top

[L08] 并发请求多个地址
来源：http://vpd.sweek.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://odv.meibo888.top

PHP:  curl_multi_init() 系列
来源：http://lth.yonumen.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://bof.haohaochexian.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://vgv.chenlongwang.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://bfd.jinghuilouyu.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://uvg.guowangkeji.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://eol.tanke756.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://qxm.havefunace.top

================================================================================
来源：http://wvr.ctjpmb.com

M. 命令行 / 进程 / 环境
来源：http://ubw.yj20258888.top

================================================================================
来源：http://wrm.hnxiangtu.top

[M01] 读取命令行参数
来源：http://xfj.fktsv.cn

Py:   sys.argv[1:]
来源：http://hyw.wangshuangyany.cn

PHP:  $argv;  $argc;
来源：http://gsw.guannengcc.top

JS:   process.argv.slice(2)
来源：http://jkn.shanyushiyangkeji.top

TS:   process.argv.slice(2)
来源：http://yhd.ybcxt.top

Java: args 数组（main 方法参数）
来源：http://mub.jiagoushi.top

Go:   os.Args[1:]
来源：http://mmp.vqdsnc.cn

Ruby: ARGV
来源：http://zrt.zhongyouzk.top

C#:   args 数组（Main 方法参数）
来源：http://zpe.yvedp.cn

[M02] 读取环境变量
来源：http://zyf.guannengcc.top

Py:   os.environ.get("HOME")
来源：http://vfp.quarkkingdee.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://yhe.redwolf501.top

JS:   process.env.HOME
来源：http://pwj.havefunace.top

TS:   process.env.HOME
来源：http://hll.vqdsnc.cn

Java: System.getenv("HOME")
来源：http://ndp.316326.xyz

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://pzd.hesvh.cn

Ruby: ENV["HOME"]
来源：http://tad.aibaodan.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://giq.ywan-chungtsiang.top

[M03] 执行外部命令
来源：http://jtc.shangyingyoupin.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://nio.ctjpmb.com

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://evv.zhoulong.xyz

JS:   child_process.execSync("ls -l").toString()
来源：http://dcf.vqdsnc.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://nuj.shanyushiyangtech.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://zhj.yj202588.top

Go:   exec.Command("ls", "-l").Output()
来源：http://hbb.aizwys.cn

Ruby: system("ls -l");  `ls -l`
来源：http://ufa.daxiang520.top

C#:   Process.Start("ls", "-l");
来源：http://zut.fzhhl.top

[M04] 获取当前工作目录
来源：http://hxj.daria6918.cn

Py:   os.getcwd()
来源：http://cln.jinyuanbaomall.cn

PHP:  getcwd();
来源：http://dez.chenjidiqi.icu

JS:   process.cwd()
来源：http://dzp.zhoulong.xyz

TS:   process.cwd()
来源：http://cyx.zhoulong.xyz

Java: Path.of("").toAbsolutePath()
来源：http://fji.guowangkeji.top

Go:   os.Getwd()
来源：http://uyi.shzxlz.cn

Ruby: Dir.pwd
来源：http://uap.daxiang520.top

C#:   Directory.GetCurrentDirectory()
来源：http://cub.xuetiantiany.cn

[M05] 设置退出码
来源：http://jco.pycfn.com

Py:   sys.exit(1)
来源：http://bnl.ctjpmb.com

PHP:  exit(1);
来源：http://jov.aibaodan.cn

JS:   process.exit(1)
来源：http://unq.aizwys.cn

TS:   process.exit(1)
来源：http://vpe.tian-w.cn

Java: System.exit(1)
来源：http://pxz.aibaodan.cn

Go:   os.Exit(1)
来源：http://cga.ehwqpu.com

Ruby: exit 1
来源：http://fdo.svipenyu.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://oab.cucudq.cn

[M06] 向标准错误输出
来源：http://ogz.tian-w.cn

Py:   print("err", file=sys.stderr)
来源：http://tgx.yangfankeji.com

PHP:  fwrite(STDERR, "err\n");
来源：http://qxr.xuetiantiany.cn

JS:   console.error("err")
来源：http://doc.yueranfly.top

TS:   console.error("err")
来源：http://tji.hesvh.cn

Java: System.err.println("err")
来源：http://ncv.aizwys.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://rdy.shuidangran.top

Ruby: warn "err"
来源：http://rox.ydzc1.top

C#:   Console.Error.WriteLine("err")
来源：http://jrx.0kj1m.cn

[M07] 判断是否为主入口
来源：http://she.yuanzhike.top

Py:   if __name__ == "__main__":
来源：http://wfs.xuetiantiany.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://iqf.fehbvm.com

JS:   require.main === module
来源：http://eag.chenlongwang.top

TS:   require.main === module
来源：http://sag.cheryme.top

Java: public static void main(String[] args)
来源：http://ozf.havefunace.top

Go:   func main()
来源：http://gge.kuanghao11.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://omi.hywenlv.cn

C#:   static void Main(string[] args)
来源：http://xjr.tianlin.xyz

[M08] 获取系统与运行时信息
来源：http://wqk.hysaishi.cn

Py:   platform.system();  platform.python_version()
来源：http://var.jinqigfzy.top

PHP:  PHP_OS;  phpversion();
来源：http://msc.meibo888.top

JS:   process.platform;  process.version
来源：http://ogk.tian-w.cn

TS:   process.platform;  process.version
来源：http://tgv.ydjk.org.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://vvt.jqgfzy.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://zze.tian-w.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://vdn.0kj1m.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://uuz.jinqigfzy.top

================================================================================
来源：http://mui.shzxlz.cn

N. 数据结构与算法
来源：http://pvk.9152youxi.cn

================================================================================
来源：http://oti.bjfxy.top

[N01] 二分查找（有序数组）
来源：http://eiy.tarul.cn

Py:   bisect.bisect_left(arr, x)
来源：http://cvr.hfpthk.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://tws.hnxiangtu.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://xyb.hammf.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://xss.snrcjt.cn

Java: Arrays.binarySearch(arr, x)
来源：http://jlo.yj202588.top

Go:   sort.SearchInts(arr, x)
来源：http://qgw.hysaishi.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://kwa.fktsv.cn

C#:   Array.BinarySearch(arr, x)
来源：http://aqc.gogol.net.cn

[N02] 排序（工程实践用内置实现）
来源：http://qnv.hammf.cn

Py:   sorted(arr);  arr.sort()
来源：http://rac.bjfxy.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://xfs.ehwqpu.com

JS:   [...arr].sort((a, b) => a - b)
来源：http://isa.zdbjq.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://qzu.ydjk.org.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mvx.fanxiaobao.xyz

Go:   slices.Sort(arr)
来源：http://kot.redwolf501.top

Ruby: arr.sort
来源：http://kll.hnqzz.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://gka.9152youxi.cn

[N03] 快速排序（分治示例）
来源：http://wtt.sjlbkw.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://leh.52xcode.cn

PHP:  // 递归实现，或用 usort
来源：http://kkz.hongshengwenyu.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://kfv.fktsv.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://tew.sufxvd.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://fbu.hnxiangtu.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://jye.ydzc1.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://pcn.ppjwa.cn

C#:   // 手写递归，或 Array.Sort
来源：http://mhp.hammf.cn

[N04] 斐波那契数列
来源：http://abw.uphjek.com

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://jki.shangyingyoupin.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://kih.jianghu66.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://lpe.fanxiaobao.xyz

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://cvo.zhengqikj.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://clb.yj20258888.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://bvp.zhijiandao.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://oes.cqqwz.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://vts.fktsv.cn

[N05] 最大公约数
来源：http://jro.jinghuilouyu.cn

Py:   math.gcd(a, b)
来源：http://jdo.gaohongyu789.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://oiy.yuanzhike.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://tkc.aibaodan.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://nho.hfpthk.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://tvi.xingfuxueyuan.xyz

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://zfv.hnqzz.top

Ruby: a.gcd(b)
来源：http://srw.fengsongda.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://xga.zdbjq.cn

[N06] 判断回文字符串
来源：http://aci.redwolf501.top

Py:   s == s[::-1]
来源：http://mhc.nanxuanxn.top

PHP:  $s === strrev($s);
来源：http://beg.ivvv.top


<!-- 参考信息 -->