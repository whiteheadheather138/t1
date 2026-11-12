代发 wailian999

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://her.haohaochexian.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ayi.xingfuxueyuan.xyz

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://sii.tanke756.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ifl.meibo888.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://rce.shangyingyoupin.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://mmd.zhixingplan.top

[J09] 时区处理
来源：http://qqs.zhaomingkeji.xyz

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://qhf.svipenyu.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://tnp.sysykeji.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://jcz.shanyushiyangtech.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://azj.cqqwz.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://pik.52xcode.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://owe.dashuyun.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://rpz.aibaodan.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://vea.xylfe.cn

[J10] 取今天 / 本月第一天
来源：http://uan.wangshuangyany.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://cye.shzxlz.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://yyf.jinyuanbaomall.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ryu.uphjek.com

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://duj.hywenlv.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hlr.shanyushiyangkeji.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://alw.hysaishi.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ywf.yj202588.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://vdc.chenzaomai.com

================================================================================
来源：http://zbz.wangshuangyany.cn

K. JSON 与序列化
来源：http://mvy.fzhhl.top

================================================================================
来源：http://qjp.fanxiaobao.xyz

[K01] 对象转 JSON 字符串
来源：http://gbd.epnwcf.com

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://otf.feifeiyinyue.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://tjd.jinqigufen.top

JS:   JSON.stringify(obj)
来源：http://mbq.guannengcc.top

TS:   JSON.stringify(obj)
来源：http://ijb.ppjwa.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://cng.kuanghao11.cn

Go:   json.Marshal(obj)
来源：http://itx.zhiwuduotai.top

Ruby: obj.to_json                                     // require "json"
来源：http://bpi.xuanzx.com

C#:   JsonSerializer.Serialize(obj)
来源：http://kqd.zhijiandao.cn

[K02] JSON 字符串转对象
来源：http://kki.c1oappe.top

Py:   json.loads(s)
来源：http://qwf.tian-w.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://uqe.sxryk.cn

JS:   JSON.parse(s)
来源：http://qfw.cheryme.top

TS:   JSON.parse(s)
来源：http://enu.yanxiufei.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hle.chenlongwang.top

Go:   json.Unmarshal(data, &v)
来源：http://czm.daxiang520.top

Ruby: JSON.parse(s)
来源：http://thm.xziqi.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://yvy.chenzaomai.com

[K03] JSON 美化输出（带缩进）
来源：http://tfz.cdnleiting.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://brx.shanyushiyangtech.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://eyu.sxryk.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://fgz.nanxinkj.top

TS:   JSON.stringify(obj, null, 2)
来源：http://bfe.mhx1999.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ryz.tianlin.xyz

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hzz.yuanzhike.top

Ruby: JSON.pretty_generate(obj)
来源：http://aai.fengsongda.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://wkq.sweek.top

[K04] 读取 JSON 文件
来源：http://pjj.zhixingplan.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://fct.tanke756.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://pes.ybcxt.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://eal.havefunace.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://fqt.52xcode.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://sco.pycfn.com

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://nui.gotoacloud.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://sin.sufxvd.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://zbl.0kj1m.cn

[K05] 深拷贝对象
来源：http://ezf.quarkkingdee.top

Py:   copy.deepcopy(obj)
来源：http://cxj.xziqi.cn

PHP:  unserialize(serialize($obj));
来源：http://iip.iojbl.cn

JS:   structuredClone(obj)
来源：http://wpp.zycfv.cn

TS:   structuredClone(obj)
来源：http://jky.havefunace.top

Java: // 手写拷贝构造，或序列化往返
来源：http://kth.tianlin.xyz

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://erb.hywenlv.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ndu.zhaomingkeji.xyz

C#:   // 序列化往返，或自定义 Clone
来源：http://bxq.tian-w.cn

[K06] 解析 URL 查询串
来源：http://els.cashguo.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://rqp.jiagoushi.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://fkw.aibaodan.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://qib.dashuyun.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://fdf.ppjwa.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://izf.zhoulong.xyz

Go:   url.ParseQuery("a=1&b=2")
来源：http://wmk.vehdjk.com

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ccr.xziqi.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://lam.tanke756.top

[K07] 进制转换
来源：http://jre.yangfankeji.com

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://jsk.xylfe.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://xdn.zhengqikj.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://nuf.redwolf501.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://oyh.xingfuxueyuan.xyz

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://dke.birdmap.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://suu.fktsv.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://xtm.hnxiangtu.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://dsy.yonumen.top

[K08] 二进制序列化（非 JSON）
来源：http://qrm.epnwcf.com

Py:   pickle.dumps(obj)
来源：http://vnc.nanxuanxn.top

PHP:  serialize($obj);  unserialize($s);
来源：http://byw.fanxiaobao.xyz

JS:   v8.serialize(obj)        // Node
来源：http://mzb.dashuyun.cn

TS:   v8.serialize(obj)        // Node
来源：http://taw.andypj.xyz

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ckb.hywenlv.cn

Go:   encoding/gob
来源：http://meu.jyoumei.cn

Ruby: Marshal.dump(obj)
来源：http://njq.jianghu66.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://abj.chenjidiqi.icu

================================================================================
来源：http://xfr.uphjek.com

L. 网络请求
来源：http://xmk.xinyue.icu

================================================================================
来源：http://gla.shuidangran.top

[L01] 发送 GET 请求
来源：http://zsn.jqgfzy.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ijy.sysykeji.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://xpq.jyoumei.cn

JS:   await fetch(url)
来源：http://wuw.cashguo.top

TS:   await fetch(url)
来源：http://erp.xuanzx.com

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ryh.ywan-chungtsiang.top

Go:   resp, err := http.Get(url)
来源：http://xiw.hysaishi.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://bae.hesvh.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://stu.xziqi.cn

[L02] 发送 POST JSON
来源：http://zyh.jinyuanbaomall.cn

Py:   requests.post(url, json={"a": 1})
来源：http://cgv.zdqjudy.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://qzs.xinyue.icu

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://vhl.52xcode.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://tbh.zhaomingkeji.xyz

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://tlu.zhaomingkeji.xyz

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://omr.andypj.xyz

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://klv.wangshuangyany.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://jdy.xinyue.icu

[L03] 设置自定义请求头
来源：http://ufj.yj202588.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://zzb.jinyuanbaomall.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://gtd.cdnleiting.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://xbo.dianchejie.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://utk.jqgufenzy.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mxz.cdnleiting.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://xxl.xuanzx.com

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://uvj.jianghu66.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://fwz.9152youxi.cn

[L04] 设置超时
来源：http://sjj.zhixingplan.top

Py:   requests.get(url, timeout=5)
来源：http://zqk.haohaochexian.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://yhd.jinyuanbaomall.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://qyg.zdbjq.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://rnm.c1oappe.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ofu.ctjpmb.com

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ugb.jqgfzy.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hlp.jianghu66.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://iia.chenzaomai.com

[L05] 上传文件（multipart）
来源：http://nls.andypj.xyz

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://eia.wangdashe.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://seu.yfazqb.com

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://pbm.hywenlv.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://tik.guowangkeji.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ytu.hysaishi.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ldr.fehbvm.com

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ezt.sxryk.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://eut.chenzaomai.com

[L06] 解析响应为 JSON
来源：http://qnh.shzxlz.cn

Py:   resp.json()
来源：http://umo.aizwys.cn

PHP:  json_decode($body, true);
来源：http://aly.yuxming.cn

JS:   await resp.json()
来源：http://dun.jqgufenzy.top

TS:   await resp.json()
来源：http://cie.cdnleiting.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://oxm.xinyue.icu

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://cql.cdnleiting.top

Ruby: JSON.parse(resp.body)
来源：http://ecr.ppjwa.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://gey.wangdashe.top

[L07] 处理 HTTP 状态码
来源：http://buy.sjlbkw.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://yao.dashuyun.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://zhf.xingfuxueyuan.xyz

JS:   resp.ok;  resp.status
来源：http://cjg.shanyushiyangtech.top

TS:   resp.ok;  resp.status
来源：http://gzj.hammf.cn

Java: resp.statusCode()
来源：http://nhe.zdbjq.cn

Go:   resp.StatusCode
来源：http://zav.xingfuxueyuan.xyz

Ruby: resp.code.to_i
来源：http://qaa.gotoacloud.top

C#:   (int)resp.StatusCode
来源：http://efo.snrcjt.cn

[L08] 并发请求多个地址
来源：http://yco.0kj1m.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://oix.xuetiantiany.cn

PHP:  curl_multi_init() 系列
来源：http://jwu.ctjpmb.com

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://fhd.xinyue.icu

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://sfa.yonumen.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://emm.bjfxy.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://gwf.yvedp.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://str.guowangkeji.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://kfe.jlsjyb.cn

================================================================================
来源：http://yne.sweek.top

M. 命令行 / 进程 / 环境
来源：http://ijf.yj20258888.top

================================================================================
来源：http://fso.hesvh.cn

[M01] 读取命令行参数
来源：http://rgj.chenzaomai.com

Py:   sys.argv[1:]
来源：http://mjj.guannengcc.top

PHP:  $argv;  $argc;
来源：http://hpr.jinqigfzy.top

JS:   process.argv.slice(2)
来源：http://vie.iojbl.cn

TS:   process.argv.slice(2)
来源：http://nqo.xinyue.icu

Java: args 数组（main 方法参数）
来源：http://euq.zhijiandao.cn

Go:   os.Args[1:]
来源：http://kjo.bbcook.cn

Ruby: ARGV
来源：http://hbv.yuxming.cn

C#:   args 数组（Main 方法参数）
来源：http://bio.gzhubu.top

[M02] 读取环境变量
来源：http://hch.hcnkem.com

Py:   os.environ.get("HOME")
来源：http://kkw.xuanzx.com

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ifc.shzxlz.cn

JS:   process.env.HOME
来源：http://npu.tian-w.cn

TS:   process.env.HOME
来源：http://txm.tian-w.cn

Java: System.getenv("HOME")
来源：http://adz.snrcjt.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://krm.jqgfzy.top

Ruby: ENV["HOME"]
来源：http://mns.jinqigfzy.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://baj.kuanghao11.cn

[M03] 执行外部命令
来源：http://cwq.yvedp.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://vav.tanke756.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://oji.jiagoushi.top

JS:   child_process.execSync("ls -l").toString()
来源：http://fbr.fzhhl.top

TS:   child_process.execSync("ls -l").toString()
来源：http://knn.xuetiantiany.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://oht.yonumen.top

Go:   exec.Command("ls", "-l").Output()
来源：http://kir.snrcjt.cn

Ruby: system("ls -l");  `ls -l`
来源：http://soa.daria6918.cn

C#:   Process.Start("ls", "-l");
来源：http://cjr.gotoacloud.top

[M04] 获取当前工作目录
来源：http://ybd.yonumen.top

Py:   os.getcwd()
来源：http://txt.guowangkeji.top

PHP:  getcwd();
来源：http://ddx.hesvh.cn

JS:   process.cwd()
来源：http://fzc.vqdsnc.cn

TS:   process.cwd()
来源：http://szu.vqdsnc.cn

Java: Path.of("").toAbsolutePath()
来源：http://psy.c1oappe.top

Go:   os.Getwd()
来源：http://fex.hywenlv.cn

Ruby: Dir.pwd
来源：http://obe.ppjwa.cn

C#:   Directory.GetCurrentDirectory()
来源：http://ryr.jlsjyb.cn

[M05] 设置退出码
来源：http://mhm.iojbl.cn

Py:   sys.exit(1)
来源：http://nxk.jlsjyb.cn

PHP:  exit(1);
来源：http://bho.hnqzz.top

JS:   process.exit(1)
来源：http://rvu.jqgfzy.top

TS:   process.exit(1)
来源：http://pcx.chenzaomai.com

Java: System.exit(1)
来源：http://gxm.nwbrower.top

Go:   os.Exit(1)
来源：http://svx.9152youxi.cn

Ruby: exit 1
来源：http://tpw.daxiang520.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ytd.jinyuanbaomall.cn

[M06] 向标准错误输出
来源：http://yzn.smart0.xyz

Py:   print("err", file=sys.stderr)
来源：http://pej.smart0.xyz

PHP:  fwrite(STDERR, "err\n");
来源：http://rnl.ctjpmb.com

JS:   console.error("err")
来源：http://zjo.hywenlv.cn

TS:   console.error("err")
来源：http://hnp.daria6918.cn

Java: System.err.println("err")
来源：http://kjj.fehbvm.com

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://cmf.cdnleiting.top

Ruby: warn "err"
来源：http://mgr.epnwcf.com

C#:   Console.Error.WriteLine("err")
来源：http://ivd.shanyushiyangtech.top

[M07] 判断是否为主入口
来源：http://htr.sxryk.cn

Py:   if __name__ == "__main__":
来源：http://huz.hammf.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://fnu.zhijiandao.cn

JS:   require.main === module
来源：http://xqb.xingfuxueyuan.xyz

TS:   require.main === module
来源：http://ttx.0kj1m.cn

Java: public static void main(String[] args)
来源：http://mkf.fanxiaobao.xyz

Go:   func main()
来源：http://vqv.0kj1m.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://csx.ydjk.org.cn

C#:   static void Main(string[] args)
来源：http://eyp.fanxiaobao.xyz

[M08] 获取系统与运行时信息
来源：http://bml.gotoacloud.top

Py:   platform.system();  platform.python_version()
来源：http://sxx.shuidangran.top

PHP:  PHP_OS;  phpversion();
来源：http://yeo.redwolf501.top

JS:   process.platform;  process.version
来源：http://okl.aizwys.cn

TS:   process.platform;  process.version
来源：http://rtc.c1oappe.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hmn.ydjk.org.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://zoo.yueranfly.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://khu.yuxming.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://tim.nanxuanxn.top

================================================================================
来源：http://pdv.hnxiangtu.top

N. 数据结构与算法
来源：http://pcq.tian-w.cn

================================================================================
来源：http://vnm.havefunace.top

[N01] 二分查找（有序数组）
来源：http://lvp.52xcode.cn

Py:   bisect.bisect_left(arr, x)
来源：http://kvi.zhengqikj.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://uhz.smart0.xyz

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://vse.hywenlv.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mvf.yuanzhike.top

Java: Arrays.binarySearch(arr, x)
来源：http://qma.bjfxy.top

Go:   sort.SearchInts(arr, x)
来源：http://qvi.zhengqikj.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://rkb.nanxinkj.top

C#:   Array.BinarySearch(arr, x)
来源：http://qfc.jyoumei.cn

[N02] 排序（工程实践用内置实现）
来源：http://uut.dashuyun.cn

Py:   sorted(arr);  arr.sort()
来源：http://ihc.dashuyun.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://dre.aizwys.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://bkk.fktsv.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://gqi.cheryme.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://sgg.birdmap.top

Go:   slices.Sort(arr)
来源：http://nkt.yonumen.top

Ruby: arr.sort
来源：http://muo.hywenlv.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://pkv.fengsongda.top

[N03] 快速排序（分治示例）
来源：http://ueb.ydjk.org.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://zis.jianghu66.top

PHP:  // 递归实现，或用 usort
来源：http://ipp.daxiang520.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://tty.tian-w.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://xbr.jinqigfzy.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://jkp.zdbjq.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://erv.nanxinkj.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://vvm.guannengcc.top

C#:   // 手写递归，或 Array.Sort
来源：http://orb.zhijiandao.cn

[N04] 斐波那契数列
来源：http://gbk.yanxiufei.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://oeb.jinghuilouyu.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://lrp.tianlin.xyz

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ent.aizwys.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://txb.vqdsnc.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://aek.meibo888.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://riu.jqgfzy.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://bzd.cqqwz.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://kbp.yj20258.top

[N05] 最大公约数
来源：http://hdm.sufxvd.cn

Py:   math.gcd(a, b)
来源：http://xel.xingfuxueyuan.xyz

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://fwn.shanyushiyangkeji.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://vly.gotoacloud.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://rtv.hywenlv.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://nli.jqgfzy.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ind.feifeiyinyue.top

Ruby: a.gcd(b)
来源：http://bcg.xylfe.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://pln.sufxvd.cn

[N06] 判断回文字符串
来源：http://smx.xingfuxueyuan.xyz

Py:   s == s[::-1]
来源：http://ziw.hongshengwenyu.top

PHP:  $s === strrev($s);
来源：http://umw.pycfn.com


<!-- 参考信息 -->