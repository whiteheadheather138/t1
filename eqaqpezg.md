代发 wailian999

C#:   d1 < d2;  d1 == d2
来源：http://mel.uphjek.com

[J08] 提取年月日与星期
来源：http://eaq.shanyushiyangkeji.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://rji.yuanzhike.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://yhm.daria6918.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ziz.jinqigfzy.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://txh.xziqi.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://aps.iojbl.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://oms.daria6918.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://kqx.guowangkeji.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://sua.gogol.net.cn

[J09] 时区处理
来源：http://aux.shzxlz.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://cca.xinyue.icu

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://nim.tianlin.xyz

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://pki.jyoumei.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://rbr.xuanzx.com

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ddn.kuanghao11.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://zij.shanyushiyangkeji.top

Ruby: Time.now.getlocal("+08:00")
来源：http://bpw.hcnkem.com

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://kkw.jinqigfzy.top

[J10] 取今天 / 本月第一天
来源：http://gfy.chenlongwang.top

Py:   date.today();  date.today().replace(day=1)
来源：http://muo.zdbjq.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://kqc.sxryk.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://gkk.hesvh.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ycc.yj20258888.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://eha.fzhhl.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ipo.xziqi.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ndl.redwolf501.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://bcg.cdnleiting.top

================================================================================
来源：http://gny.hfpthk.cn

K. JSON 与序列化
来源：http://bow.vehdjk.com

================================================================================
来源：http://fvn.quarkkingdee.top

[K01] 对象转 JSON 字符串
来源：http://mju.fanxiaobao.xyz

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://bzf.jinyuanbaomall.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://smk.mhx1999.top

JS:   JSON.stringify(obj)
来源：http://qbb.jinyuanbaomall.cn

TS:   JSON.stringify(obj)
来源：http://loe.quarkkingdee.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://bwt.yuxming.cn

Go:   json.Marshal(obj)
来源：http://wel.gzhubu.top

Ruby: obj.to_json                                     // require "json"
来源：http://aku.haohaochexian.top

C#:   JsonSerializer.Serialize(obj)
来源：http://tnw.xylfe.cn

[K02] JSON 字符串转对象
来源：http://kih.zdbjq.cn

Py:   json.loads(s)
来源：http://kgg.zhengqikj.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://qzc.smart0.xyz

JS:   JSON.parse(s)
来源：http://ftm.jinqigfzy.top

TS:   JSON.parse(s)
来源：http://wkq.ctjpmb.com

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://wip.shuidangran.top

Go:   json.Unmarshal(data, &v)
来源：http://yrv.snrcjt.cn

Ruby: JSON.parse(s)
来源：http://emr.daxiang520.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://gwx.guannengcc.top

[K03] JSON 美化输出（带缩进）
来源：http://dhk.jinyuanbaomall.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://qlm.havefunace.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://cco.sufxvd.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://qci.sxryk.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://sbr.kuanghao11.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wce.cdnleiting.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://bkg.nwbrower.top

Ruby: JSON.pretty_generate(obj)
来源：http://oml.ppjwa.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://qmv.shanyushiyangkeji.top

[K04] 读取 JSON 文件
来源：http://tba.uphjek.com

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://qza.shzxlz.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://rhv.jlsjyb.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://xgn.iojbl.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://lzn.fzhhl.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://rhm.xuetiantiany.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://tto.dashuyun.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://yuv.fengsongda.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://tbn.xziqi.cn

[K05] 深拷贝对象
来源：http://juc.sysykeji.top

Py:   copy.deepcopy(obj)
来源：http://tgi.jinqigufen.top

PHP:  unserialize(serialize($obj));
来源：http://jwz.wangshuangyany.cn

JS:   structuredClone(obj)
来源：http://rza.tarul.cn

TS:   structuredClone(obj)
来源：http://wda.hysaishi.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://jnm.fengsongda.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://nxf.dianchejie.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://yxs.chenzaomai.com

C#:   // 序列化往返，或自定义 Clone
来源：http://vra.hongshengwenyu.top

[K06] 解析 URL 查询串
来源：http://ell.vqdsnc.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://stb.feifeiyinyue.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://frp.jianghu66.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://oze.tanke756.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://jlv.shanyushiyangkeji.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://gvv.jianghu66.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://hdn.uphjek.com

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://vjv.epnwcf.com

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://eev.vehdjk.com

[K07] 进制转换
来源：http://flg.nanxinkj.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://saa.hywenlv.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://kop.hysaishi.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://cqc.tanke756.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://jth.gzhubu.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://xca.tarul.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://eoj.cqqwz.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://oiq.hnxiangtu.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://qdm.zycfv.cn

[K08] 二进制序列化（非 JSON）
来源：http://rdp.fehbvm.com

Py:   pickle.dumps(obj)
来源：http://gre.yj20258888.top

PHP:  serialize($obj);  unserialize($s);
来源：http://pae.jinyuanbaomall.cn

JS:   v8.serialize(obj)        // Node
来源：http://oyc.daria6918.cn

TS:   v8.serialize(obj)        // Node
来源：http://rwc.vehdjk.com

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://rfk.fzhhl.top

Go:   encoding/gob
来源：http://muv.xingfuxueyuan.xyz

Ruby: Marshal.dump(obj)
来源：http://bjs.sufxvd.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://iuu.zhaomingkeji.xyz

================================================================================
来源：http://hvu.fanxiaobao.xyz

L. 网络请求
来源：http://jhr.cucudq.cn

================================================================================
来源：http://iaw.zhoulong.xyz

[L01] 发送 GET 请求
来源：http://ipf.ydjk.org.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://tbs.jianghu66.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://onw.shanyushiyangtech.top

JS:   await fetch(url)
来源：http://gjj.hysaishi.cn

TS:   await fetch(url)
来源：http://jpx.pengpengdd.cyou

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://snt.yj20258.top

Go:   resp, err := http.Get(url)
来源：http://yiq.shangyingyoupin.top

Ruby: Net::HTTP.get(URI(url))
来源：http://cyi.haohaochexian.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://fgf.vehdjk.com

[L02] 发送 POST JSON
来源：http://oah.yueranfly.top

Py:   requests.post(url, json={"a": 1})
来源：http://njv.cdnleiting.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://zym.guannengcc.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://vog.sxryk.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://aol.gotoacloud.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://isv.iojbl.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://poq.wangshuangyany.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ixw.sjlbkw.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://zmn.zdbjq.cn

[L03] 设置自定义请求头
来源：http://pxd.yj20258888.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://fzh.hesvh.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://olk.xuanzx.com

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://qsn.xinyue.icu

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://bux.ybcxt.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://zzo.fktsv.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://jaf.jinqigufen.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ktl.yuxming.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://lov.hcnkem.com

[L04] 设置超时
来源：http://xap.jqgfzy.top

Py:   requests.get(url, timeout=5)
来源：http://bdp.yj202588.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hug.sufxvd.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://osu.aibaodan.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mgh.cucudq.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://krp.chenzaomai.com

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://xbe.yanxiufei.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://yfw.sjlbkw.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://gio.epnwcf.com

[L05] 上传文件（multipart）
来源：http://kut.zycfv.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://xcp.gzhubu.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://dhr.dashuyun.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://uqp.jinyuanbaomall.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://lsh.zhongyouzk.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mqd.tarul.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ees.tianlin.xyz

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://sfi.jinqigufen.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://okf.zhiwuduotai.top

[L06] 解析响应为 JSON
来源：http://qvo.iojbl.cn

Py:   resp.json()
来源：http://wyt.fehbvm.com

PHP:  json_decode($body, true);
来源：http://wek.daxiang520.top

JS:   await resp.json()
来源：http://kie.zhongyouzk.top

TS:   await resp.json()
来源：http://xtb.zhijiandao.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wbd.wangdashe.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://nqr.zdqjudy.top

Ruby: JSON.parse(resp.body)
来源：http://hcs.fktsv.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://nfl.xingfuxueyuan.xyz

[L07] 处理 HTTP 状态码
来源：http://onr.yj20258.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://lsm.guannengcc.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://dcz.tianlin.xyz

JS:   resp.ok;  resp.status
来源：http://qza.dianchejie.cn

TS:   resp.ok;  resp.status
来源：http://wdy.xziqi.cn

Java: resp.statusCode()
来源：http://fjw.jinghuilouyu.cn

Go:   resp.StatusCode
来源：http://gdj.ehwqpu.com

Ruby: resp.code.to_i
来源：http://yxd.yfazqb.com

C#:   (int)resp.StatusCode
来源：http://thb.sxryk.cn

[L08] 并发请求多个地址
来源：http://mvc.jinqigufen.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://pap.yj20258888.top

PHP:  curl_multi_init() 系列
来源：http://kyh.smart0.xyz

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://cbl.9152youxi.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://dmu.tarul.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://zno.yonumen.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://nuq.vqdsnc.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hgw.gotoacloud.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://gpr.guannengcc.top

================================================================================
来源：http://chj.fengsongda.top

M. 命令行 / 进程 / 环境
来源：http://myr.daria6918.cn

================================================================================
来源：http://dei.fengsongda.top

[M01] 读取命令行参数
来源：http://ycp.zycfv.cn

Py:   sys.argv[1:]
来源：http://odb.pycfn.com

PHP:  $argv;  $argc;
来源：http://nwk.zhiwuduotai.top

JS:   process.argv.slice(2)
来源：http://egu.guannengcc.top

TS:   process.argv.slice(2)
来源：http://scp.yuxming.cn

Java: args 数组（main 方法参数）
来源：http://ctn.fanxiaobao.xyz

Go:   os.Args[1:]
来源：http://syh.vqdsnc.cn

Ruby: ARGV
来源：http://kpr.52xcode.cn

C#:   args 数组（Main 方法参数）
来源：http://azx.sufxvd.cn

[M02] 读取环境变量
来源：http://toj.hongshengwenyu.top

Py:   os.environ.get("HOME")
来源：http://fcl.fktsv.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://gxo.yuanzhike.top

JS:   process.env.HOME
来源：http://dmo.cdnleiting.top

TS:   process.env.HOME
来源：http://pwa.tarul.cn

Java: System.getenv("HOME")
来源：http://jjf.jyoumei.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://pkw.ppjwa.cn

Ruby: ENV["HOME"]
来源：http://iir.yuanzhike.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hhl.fehbvm.com

[M03] 执行外部命令
来源：http://afb.nanxuanxn.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://skg.hfpthk.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://nkg.yangfankeji.com

JS:   child_process.execSync("ls -l").toString()
来源：http://glo.ywan-chungtsiang.top

TS:   child_process.execSync("ls -l").toString()
来源：http://smq.hcnkem.com

Java: new ProcessBuilder("ls", "-l").start()
来源：http://etm.jlsjyb.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://cib.havefunace.top

Ruby: system("ls -l");  `ls -l`
来源：http://rqr.nwbrower.top

C#:   Process.Start("ls", "-l");
来源：http://aak.fengsongda.top

[M04] 获取当前工作目录
来源：http://cxi.sysykeji.top

Py:   os.getcwd()
来源：http://pkc.ivvv.top

PHP:  getcwd();
来源：http://aml.ppjwa.cn

JS:   process.cwd()
来源：http://kvp.52xcode.cn

TS:   process.cwd()
来源：http://ewh.jyoumei.cn

Java: Path.of("").toAbsolutePath()
来源：http://uwy.mhx1999.top

Go:   os.Getwd()
来源：http://oye.wangdashe.top

Ruby: Dir.pwd
来源：http://wlk.shangyingyoupin.top

C#:   Directory.GetCurrentDirectory()
来源：http://sik.tian-w.cn

[M05] 设置退出码
来源：http://gxe.zhengqikj.top

Py:   sys.exit(1)
来源：http://zjq.52xcode.cn

PHP:  exit(1);
来源：http://ike.shanyushiyangkeji.top

JS:   process.exit(1)
来源：http://djm.tianlin.xyz

TS:   process.exit(1)
来源：http://dhc.316326.xyz

Java: System.exit(1)
来源：http://wej.zhiwuduotai.top

Go:   os.Exit(1)
来源：http://dhg.zhiwuduotai.top

Ruby: exit 1
来源：http://awj.bbcook.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://rga.jqgfzy.top

[M06] 向标准错误输出
来源：http://qpl.vqdsnc.cn

Py:   print("err", file=sys.stderr)
来源：http://ysh.nanxinkj.top

PHP:  fwrite(STDERR, "err\n");
来源：http://ycq.yueranfly.top

JS:   console.error("err")
来源：http://xsh.jyoumei.cn

TS:   console.error("err")
来源：http://qxy.fktsv.cn

Java: System.err.println("err")
来源：http://ojo.yj20258888.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://okq.redwolf501.top

Ruby: warn "err"
来源：http://ijc.gogol.net.cn

C#:   Console.Error.WriteLine("err")
来源：http://nwy.yangfankeji.com

[M07] 判断是否为主入口
来源：http://oet.jinqigufen.top

Py:   if __name__ == "__main__":
来源：http://wwk.feifeiyinyue.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://uwp.epnwcf.com

JS:   require.main === module
来源：http://yfr.yangfankeji.com

TS:   require.main === module
来源：http://dhj.aizwys.cn

Java: public static void main(String[] args)
来源：http://awm.yongpay.top

Go:   func main()
来源：http://cce.yangfankeji.com

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://uyg.yj20258888.top

C#:   static void Main(string[] args)
来源：http://qud.xinyue.icu

[M08] 获取系统与运行时信息
来源：http://xls.nanxuanxn.top

Py:   platform.system();  platform.python_version()
来源：http://tlq.quarkkingdee.top

PHP:  PHP_OS;  phpversion();
来源：http://nio.cashguo.top

JS:   process.platform;  process.version
来源：http://oxd.ybcxt.top

TS:   process.platform;  process.version
来源：http://wny.zdbjq.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ezd.ppjwa.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://xyp.hcnkem.com

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://kgb.smart0.xyz

C#:   Environment.OSVersion;  Environment.Version
来源：http://odp.sufxvd.cn

================================================================================
来源：http://fby.fktsv.cn

N. 数据结构与算法
来源：http://aos.chenlongwang.top

================================================================================
来源：http://oso.fzhhl.top

[N01] 二分查找（有序数组）
来源：http://dlx.hywenlv.cn

Py:   bisect.bisect_left(arr, x)
来源：http://hyt.uphjek.com

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://bex.daxiang520.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ixc.tarul.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://tbn.zycfv.cn

Java: Arrays.binarySearch(arr, x)
来源：http://qja.sufxvd.cn

Go:   sort.SearchInts(arr, x)
来源：http://uxs.jyoumei.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://cup.xingfuxueyuan.xyz

C#:   Array.BinarySearch(arr, x)
来源：http://axz.mhx1999.top

[N02] 排序（工程实践用内置实现）
来源：http://gku.shuidangran.top

Py:   sorted(arr);  arr.sort()
来源：http://cjq.shanyushiyangtech.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://aef.jianghu66.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://idu.aibaodan.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://rgw.hfpthk.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://uyk.guannengcc.top

Go:   slices.Sort(arr)
来源：http://qof.sxryk.cn

Ruby: arr.sort
来源：http://btm.vehdjk.com

C#:   Array.Sort(arr);  list.Sort()
来源：http://pmy.zycfv.cn

[N03] 快速排序（分治示例）
来源：http://bbz.gaohongyu789.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://nsy.jlsjyb.cn

PHP:  // 递归实现，或用 usort
来源：http://jpp.jiagoushi.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://fmn.yj20258888.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://eqm.tianlin.xyz

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ggh.redwolf501.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://iwj.yvedp.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://btf.aizwys.cn

C#:   // 手写递归，或 Array.Sort
来源：http://svw.zhijiandao.cn

[N04] 斐波那契数列
来源：http://tkh.chenjidiqi.icu

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wyj.hnqzz.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://eol.tarul.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ctn.yanxiufei.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://tln.birdmap.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://zmw.jiagoushi.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://dar.yj202588.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://arp.fehbvm.com

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hlr.shuidangran.top

[N05] 最大公约数
来源：http://rhe.shzxlz.cn

Py:   math.gcd(a, b)
来源：http://str.yj20258.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://uep.tian-w.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wam.0kj1m.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://jjl.ydzc1.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://xmn.pengpengdd.cyou

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://iam.yvedp.cn

Ruby: a.gcd(b)
来源：http://umj.jiagoushi.top


<!-- 参考信息 -->