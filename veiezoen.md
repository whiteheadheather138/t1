代发 wailian999

C#:   d1 < d2;  d1 == d2
来源：http://lam.fengsongda.top

[J08] 提取年月日与星期
来源：http://eah.sxryk.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://bqp.jqgfzy.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://pkb.ydjk.org.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://nri.zhixingplan.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hfm.tianlin.xyz

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://aqu.hammf.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://cri.zhongyouzk.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ent.yj20258.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ewv.zhoulong.xyz

[J09] 时区处理
来源：http://hwi.zhoulong.xyz

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://pwq.ydzc1.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://vmk.gaohongyu789.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://pbq.fzhhl.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://rgy.jinqigfzy.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://auz.hywenlv.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ztg.xinyue.icu

Ruby: Time.now.getlocal("+08:00")
来源：http://ory.mhx1999.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://kcz.sxryk.cn

[J10] 取今天 / 本月第一天
来源：http://fle.dianchejie.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://dmz.jyoumei.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ezz.zdbjq.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://mgo.birdmap.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ywh.zdqjudy.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://fjl.sjlbkw.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ivn.aibaodan.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://nye.yj20258888.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://onl.daxiang520.top

================================================================================
来源：http://iew.yueranfly.top

K. JSON 与序列化
来源：http://fjx.yuanzhike.top

================================================================================
来源：http://eom.kuanghao11.cn

[K01] 对象转 JSON 字符串
来源：http://ged.wangdashe.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://stw.jqgufenzy.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://jyp.yanxiufei.cn

JS:   JSON.stringify(obj)
来源：http://mxa.yonumen.top

TS:   JSON.stringify(obj)
来源：http://bor.wangshuangyany.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://map.shanyushiyangtech.top

Go:   json.Marshal(obj)
来源：http://uad.nanxinkj.top

Ruby: obj.to_json                                     // require "json"
来源：http://gpb.pengpengdd.cyou

C#:   JsonSerializer.Serialize(obj)
来源：http://ozs.aizwys.cn

[K02] JSON 字符串转对象
来源：http://rva.iojbl.cn

Py:   json.loads(s)
来源：http://hsp.andypj.xyz

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ylr.52xcode.cn

JS:   JSON.parse(s)
来源：http://ddg.chenjidiqi.icu

TS:   JSON.parse(s)
来源：http://vea.yuanzhike.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://gyv.sxryk.cn

Go:   json.Unmarshal(data, &v)
来源：http://rqm.ybcxt.top

Ruby: JSON.parse(s)
来源：http://tik.birdmap.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://vsi.jinqigufen.top

[K03] JSON 美化输出（带缩进）
来源：http://vwh.tarul.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://gzg.xuanzx.com

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://rih.xinyue.icu

JS:   JSON.stringify(obj, null, 2)
来源：http://pef.jqgufenzy.top

TS:   JSON.stringify(obj, null, 2)
来源：http://eve.sxryk.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://rfu.hammf.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://azf.ppjwa.cn

Ruby: JSON.pretty_generate(obj)
来源：http://joh.yj20258.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ahm.0kj1m.cn

[K04] 读取 JSON 文件
来源：http://gnn.fanxiaobao.xyz

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://edd.xuanzx.com

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ejo.jyoumei.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://sxc.jqgufenzy.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wol.tianlin.xyz

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://jqu.aizwys.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://gmt.shanyushiyangkeji.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://pyl.xylfe.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://yil.ydjk.org.cn

[K05] 深拷贝对象
来源：http://slv.xuanzx.com

Py:   copy.deepcopy(obj)
来源：http://ukx.chenzaomai.com

PHP:  unserialize(serialize($obj));
来源：http://abn.jyoumei.cn

JS:   structuredClone(obj)
来源：http://ale.daria6918.cn

TS:   structuredClone(obj)
来源：http://xua.ppjwa.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://qiz.nanxuanxn.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://kuj.cdnleiting.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ddj.cashguo.top

C#:   // 序列化往返，或自定义 Clone
来源：http://rxk.sweek.top

[K06] 解析 URL 查询串
来源：http://sxs.smart0.xyz

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://tlr.yfazqb.com

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mqi.gotoacloud.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://xkh.jlsjyb.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://dpy.316326.xyz

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://gwl.wangdashe.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://mio.ctjpmb.com

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://roy.yonumen.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://xdl.fktsv.cn

[K07] 进制转换
来源：http://jca.jlsjyb.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ouj.fktsv.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://vcb.jiagoushi.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://cju.svipenyu.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://qjh.ppjwa.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://qtw.xziqi.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mic.jqgfzy.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://oyq.smart0.xyz

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://oad.ydjk.org.cn

[K08] 二进制序列化（非 JSON）
来源：http://twn.tarul.cn

Py:   pickle.dumps(obj)
来源：http://ryc.iojbl.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://wdo.shanyushiyangkeji.top

JS:   v8.serialize(obj)        // Node
来源：http://nah.yuanzhike.top

TS:   v8.serialize(obj)        // Node
来源：http://ljc.zycfv.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://fss.ybcxt.top

Go:   encoding/gob
来源：http://hnv.tanke756.top

Ruby: Marshal.dump(obj)
来源：http://gtb.iojbl.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://fha.epnwcf.com

================================================================================
来源：http://vrv.vqdsnc.cn

L. 网络请求
来源：http://xlw.jyoumei.cn

================================================================================
来源：http://mhs.jianghu66.top

[L01] 发送 GET 请求
来源：http://plg.meibo888.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://eti.ehwqpu.com

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://pnr.haohaochexian.top

JS:   await fetch(url)
来源：http://eei.iojbl.cn

TS:   await fetch(url)
来源：http://yrl.hcnkem.com

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://fbt.cucudq.cn

Go:   resp, err := http.Get(url)
来源：http://hta.nanxinkj.top

Ruby: Net::HTTP.get(URI(url))
来源：http://kxs.hongshengwenyu.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://nhs.shangyingyoupin.top

[L02] 发送 POST JSON
来源：http://vwi.guannengcc.top

Py:   requests.post(url, json={"a": 1})
来源：http://qub.nanxuanxn.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://aei.smart0.xyz

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://nks.hesvh.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mrm.xziqi.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://uee.ywan-chungtsiang.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://unb.zhoulong.xyz

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://psk.xziqi.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://tgg.zhaomingkeji.xyz

[L03] 设置自定义请求头
来源：http://fud.snrcjt.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://nuk.jinqigfzy.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://vps.fehbvm.com

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mlq.cucudq.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://pdk.mhx1999.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://goa.cucudq.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://xqc.svipenyu.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://tcm.nanxinkj.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hys.zhiwuduotai.top

[L04] 设置超时
来源：http://gsn.dianchejie.cn

Py:   requests.get(url, timeout=5)
来源：http://nhf.andypj.xyz

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://dvo.guowangkeji.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://qjp.xuanzx.com

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://zgp.smart0.xyz

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ytq.feifeiyinyue.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://uqk.jinqigufen.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://jej.hesvh.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://tzd.jianghu66.top

[L05] 上传文件（multipart）
来源：http://ntr.jianghu66.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://xoj.zhongyouzk.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://kia.sufxvd.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://bbj.jqgfzy.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://vbm.smart0.xyz

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://nwh.smart0.xyz

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ejf.yvedp.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://qia.cdnleiting.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mmc.ppjwa.cn

[L06] 解析响应为 JSON
来源：http://yws.ivvv.top

Py:   resp.json()
来源：http://ntd.nwbrower.top

PHP:  json_decode($body, true);
来源：http://vrw.snrcjt.cn

JS:   await resp.json()
来源：http://poq.zhongyouzk.top

TS:   await resp.json()
来源：http://ghy.316326.xyz

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://teo.zhiwuduotai.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mdi.yuanzhike.top

Ruby: JSON.parse(resp.body)
来源：http://cdj.fktsv.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://aan.mhx1999.top

[L07] 处理 HTTP 状态码
来源：http://dza.ivvv.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://sxg.havefunace.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://vzv.nwbrower.top

JS:   resp.ok;  resp.status
来源：http://piv.0kj1m.cn

TS:   resp.ok;  resp.status
来源：http://pgf.hesvh.cn

Java: resp.statusCode()
来源：http://bzl.havefunace.top

Go:   resp.StatusCode
来源：http://ppb.nanxuanxn.top

Ruby: resp.code.to_i
来源：http://zcs.ydjk.org.cn

C#:   (int)resp.StatusCode
来源：http://fsr.aizwys.cn

[L08] 并发请求多个地址
来源：http://dth.tarul.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ytd.xinyue.icu

PHP:  curl_multi_init() 系列
来源：http://ocw.ydzc1.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://yei.bjfxy.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://pkh.yuxming.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://rnn.fengsongda.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://gzm.daria6918.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wpm.tianlin.xyz

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ahj.shanyushiyangtech.top

================================================================================
来源：http://ush.shanyushiyangkeji.top

M. 命令行 / 进程 / 环境
来源：http://zkp.snrcjt.cn

================================================================================
来源：http://cap.vqdsnc.cn

[M01] 读取命令行参数
来源：http://yfz.quarkkingdee.top

Py:   sys.argv[1:]
来源：http://nsm.9152youxi.cn

PHP:  $argv;  $argc;
来源：http://svs.cheryme.top

JS:   process.argv.slice(2)
来源：http://fyu.cqqwz.cn

TS:   process.argv.slice(2)
来源：http://gcc.fanxiaobao.xyz

Java: args 数组（main 方法参数）
来源：http://rej.zycfv.cn

Go:   os.Args[1:]
来源：http://lez.fengsongda.top

Ruby: ARGV
来源：http://mak.zycfv.cn

C#:   args 数组（Main 方法参数）
来源：http://dct.fengsongda.top

[M02] 读取环境变量
来源：http://rwj.cqqwz.cn

Py:   os.environ.get("HOME")
来源：http://hym.shuidangran.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://vym.fengsongda.top

JS:   process.env.HOME
来源：http://xah.dianchejie.cn

TS:   process.env.HOME
来源：http://kge.tarul.cn

Java: System.getenv("HOME")
来源：http://our.daxiang520.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://atz.jinqigufen.top

Ruby: ENV["HOME"]
来源：http://vvk.iojbl.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://zqs.zhongyouzk.top

[M03] 执行外部命令
来源：http://soz.nanxinkj.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://bha.yangfankeji.com

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://sol.yangfankeji.com

JS:   child_process.execSync("ls -l").toString()
来源：http://oze.zhixingplan.top

TS:   child_process.execSync("ls -l").toString()
来源：http://het.jqgfzy.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://yzd.xinyue.icu

Go:   exec.Command("ls", "-l").Output()
来源：http://kln.zhoulong.xyz

Ruby: system("ls -l");  `ls -l`
来源：http://gmu.fehbvm.com

C#:   Process.Start("ls", "-l");
来源：http://frn.yj20258888.top

[M04] 获取当前工作目录
来源：http://vcu.xuetiantiany.cn

Py:   os.getcwd()
来源：http://mjr.smart0.xyz

PHP:  getcwd();
来源：http://qpn.xuanzx.com

JS:   process.cwd()
来源：http://gpm.fanxiaobao.xyz

TS:   process.cwd()
来源：http://qql.yuanzhike.top

Java: Path.of("").toAbsolutePath()
来源：http://krr.daria6918.cn

Go:   os.Getwd()
来源：http://vvq.zhoulong.xyz

Ruby: Dir.pwd
来源：http://xki.52xcode.cn

C#:   Directory.GetCurrentDirectory()
来源：http://wbo.yangfankeji.com

[M05] 设置退出码
来源：http://cir.xuanzx.com

Py:   sys.exit(1)
来源：http://gnh.gzhubu.top

PHP:  exit(1);
来源：http://bbe.fanxiaobao.xyz

JS:   process.exit(1)
来源：http://wvb.pycfn.com

TS:   process.exit(1)
来源：http://ycm.daria6918.cn

Java: System.exit(1)
来源：http://zhm.kuanghao11.cn

Go:   os.Exit(1)
来源：http://wam.yj20258888.top

Ruby: exit 1
来源：http://qze.wangdashe.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://dva.shuidangran.top

[M06] 向标准错误输出
来源：http://qqq.xuanzx.com

Py:   print("err", file=sys.stderr)
来源：http://seh.cqqwz.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://lta.hnqzz.top

JS:   console.error("err")
来源：http://gjm.uphjek.com

TS:   console.error("err")
来源：http://ayk.hywenlv.cn

Java: System.err.println("err")
来源：http://ymo.yuxming.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://iag.yj20258.top

Ruby: warn "err"
来源：http://bcg.tarul.cn

C#:   Console.Error.WriteLine("err")
来源：http://ois.zhaomingkeji.xyz

[M07] 判断是否为主入口
来源：http://amn.guannengcc.top

Py:   if __name__ == "__main__":
来源：http://eqn.fzhhl.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://swv.chenjidiqi.icu

JS:   require.main === module
来源：http://woq.jlsjyb.cn

TS:   require.main === module
来源：http://rab.iojbl.cn

Java: public static void main(String[] args)
来源：http://jya.yuanzhike.top

Go:   func main()
来源：http://dec.jiagoushi.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://fud.gotoacloud.top

C#:   static void Main(string[] args)
来源：http://iri.uphjek.com

[M08] 获取系统与运行时信息
来源：http://rtu.jiagoushi.top

Py:   platform.system();  platform.python_version()
来源：http://caj.fzhhl.top

PHP:  PHP_OS;  phpversion();
来源：http://svl.aizwys.cn

JS:   process.platform;  process.version
来源：http://fnk.jlsjyb.cn

TS:   process.platform;  process.version
来源：http://nqs.tanke756.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://odw.snrcjt.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://xwl.hywenlv.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://pft.chenzaomai.com

C#:   Environment.OSVersion;  Environment.Version
来源：http://hgi.fanxiaobao.xyz

================================================================================
来源：http://ydg.cdnleiting.top

N. 数据结构与算法
来源：http://mmz.yueranfly.top

================================================================================
来源：http://ghv.dianchejie.cn

[N01] 二分查找（有序数组）
来源：http://bnm.cdnleiting.top

Py:   bisect.bisect_left(arr, x)
来源：http://ysc.daria6918.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://thh.xuanzx.com

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://lag.gzhubu.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ema.cdnleiting.top

Java: Arrays.binarySearch(arr, x)
来源：http://ula.yfazqb.com

Go:   sort.SearchInts(arr, x)
来源：http://drt.9152youxi.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://pgx.jlsjyb.cn

C#:   Array.BinarySearch(arr, x)
来源：http://xeb.jianghu66.top

[N02] 排序（工程实践用内置实现）
来源：http://ssv.fengsongda.top

Py:   sorted(arr);  arr.sort()
来源：http://auy.yj202588.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://iag.0kj1m.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://rbn.mhx1999.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://wkm.zhixingplan.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://quc.cdnleiting.top

Go:   slices.Sort(arr)
来源：http://tls.daxiang520.top

Ruby: arr.sort
来源：http://fru.fehbvm.com

C#:   Array.Sort(arr);  list.Sort()
来源：http://ltu.zdqjudy.top

[N03] 快速排序（分治示例）
来源：http://dge.c1oappe.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://czj.yj20258.top

PHP:  // 递归实现，或用 usort
来源：http://fzz.zhixingplan.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://xlm.wangdashe.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://gfe.iojbl.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ijc.yonumen.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://kju.dianchejie.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://leb.cucudq.cn

C#:   // 手写递归，或 Array.Sort
来源：http://vld.zhoulong.xyz

[N04] 斐波那契数列
来源：http://oda.yonumen.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hdz.nanxinkj.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://zsq.yonumen.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://fvc.epnwcf.com

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://pmk.andypj.xyz

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://erf.kuanghao11.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://xyp.jianghu66.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://sbd.meibo888.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://zer.wangdashe.top

[N05] 最大公约数
来源：http://oab.jinqigufen.top

Py:   math.gcd(a, b)
来源：http://edp.fengsongda.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://xeo.zdbjq.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://lvu.tian-w.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://qkr.wangshuangyany.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://xok.jlsjyb.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://zaa.guowangkeji.top

Ruby: a.gcd(b)
来源：http://rnl.guowangkeji.top


<!-- 参考信息 -->