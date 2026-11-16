代发 wailian999

Py:   (end - start).total_seconds()
来源：http://wcz.hongshengwenyu.top

PHP:  $end->diff($start)->days;
来源：http://mat.snrcjt.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://qgh.zhiwuduotai.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://rue.316326.xyz

Java: Duration.between(start, end).toSeconds()
来源：http://kfr.sxryk.cn

Go:   end.Sub(start).Hours()
来源：http://lhw.fehbvm.com

Ruby: end - start                 # 返回秒数
来源：http://xuk.yfazqb.com

C#:   (end - start).TotalSeconds
来源：http://ekp.jyoumei.cn

[J07] 比较两个日期
来源：http://kaq.hfpthk.cn

Py:   d1 < d2;  d1 == d2
来源：http://fst.hfpthk.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://msy.vehdjk.com

JS:   d1.getTime() < d2.getTime()
来源：http://myh.sweek.top

TS:   d1.getTime() < d2.getTime()
来源：http://hmz.birdmap.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://xhx.shanyushiyangkeji.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://iwj.jyoumei.cn

Ruby: d1 < d2;  d1 == d2
来源：http://zmw.fehbvm.com

C#:   d1 < d2;  d1 == d2
来源：http://ksx.shzxlz.cn

[J08] 提取年月日与星期
来源：http://gqn.havefunace.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://cil.hnxiangtu.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ffu.quarkkingdee.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://wjb.ivvv.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://wae.yanxiufei.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://mnl.zdbjq.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://zch.yongpay.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://kej.jqgfzy.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://jiu.yanxiufei.cn

[J09] 时区处理
来源：http://ijt.ppjwa.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://xks.zhongyouzk.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://sjd.sysykeji.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hgj.cqqwz.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hlx.feifeiyinyue.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://gzl.0kj1m.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://kax.yvedp.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://ear.wangdashe.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://noj.fktsv.cn

[J10] 取今天 / 本月第一天
来源：http://mfv.mhx1999.top

Py:   date.today();  date.today().replace(day=1)
来源：http://jkv.daria6918.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://tij.shuidangran.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://szs.aizwys.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://yio.zhongyouzk.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://eos.haohaochexian.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://gpl.vehdjk.com

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://uhi.fanxiaobao.xyz

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://rcw.jinghuilouyu.cn

================================================================================
来源：http://wms.jinyuanbaomall.cn

K. JSON 与序列化
来源：http://usp.jiagoushi.top

================================================================================
来源：http://jgm.haohaochexian.top

[K01] 对象转 JSON 字符串
来源：http://qpl.ppjwa.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ixt.zdbjq.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://nqq.xuanzx.com

JS:   JSON.stringify(obj)
来源：http://kyf.ybcxt.top

TS:   JSON.stringify(obj)
来源：http://iqf.hfpthk.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://gef.xuanzx.com

Go:   json.Marshal(obj)
来源：http://kzq.gaohongyu789.top

Ruby: obj.to_json                                     // require "json"
来源：http://ziw.xylfe.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://pyx.hammf.cn

[K02] JSON 字符串转对象
来源：http://yfg.fanxiaobao.xyz

Py:   json.loads(s)
来源：http://hsw.xuanzx.com

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ezw.havefunace.top

JS:   JSON.parse(s)
来源：http://bpe.hnxiangtu.top

TS:   JSON.parse(s)
来源：http://qlf.0kj1m.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://dlk.ybcxt.top

Go:   json.Unmarshal(data, &v)
来源：http://rmn.fktsv.cn

Ruby: JSON.parse(s)
来源：http://mvw.aizwys.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://czd.gogol.net.cn

[K03] JSON 美化输出（带缩进）
来源：http://hoo.jinqigufen.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://sng.fehbvm.com

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://qgg.quarkkingdee.top

JS:   JSON.stringify(obj, null, 2)
来源：http://tsi.gogol.net.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://gnp.tianlin.xyz

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://acj.gzhubu.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wml.meibo888.top

Ruby: JSON.pretty_generate(obj)
来源：http://mip.xuanzx.com

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hfy.vqdsnc.cn

[K04] 读取 JSON 文件
来源：http://ftz.yj20258.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://lzo.sufxvd.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://day.ehwqpu.com

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hkv.wangshuangyany.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://xrm.xylfe.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://jui.hongshengwenyu.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://nes.xziqi.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://nrz.ydzc1.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://xpg.snrcjt.cn

[K05] 深拷贝对象
来源：http://rry.gzhubu.top

Py:   copy.deepcopy(obj)
来源：http://dvy.feifeiyinyue.top

PHP:  unserialize(serialize($obj));
来源：http://evr.hywenlv.cn

JS:   structuredClone(obj)
来源：http://rko.uphjek.com

TS:   structuredClone(obj)
来源：http://oaa.iojbl.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://xyu.hesvh.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://gjn.jinqigfzy.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://kbh.yfazqb.com

C#:   // 序列化往返，或自定义 Clone
来源：http://mpx.nwbrower.top

[K06] 解析 URL 查询串
来源：http://fnh.zhixingplan.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://thj.hnqzz.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://jog.cqqwz.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://tya.sufxvd.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://get.tarul.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://qrm.havefunace.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://aza.dianchejie.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://vqq.vqdsnc.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://xeq.havefunace.top

[K07] 进制转换
来源：http://wrr.gotoacloud.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://xwa.sysykeji.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://frl.zhoulong.xyz

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://bhw.jinghuilouyu.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://yna.bbcook.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://rbs.vqdsnc.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://cuk.sxryk.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://svs.xuanzx.com

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://msq.hcnkem.com

[K08] 二进制序列化（非 JSON）
来源：http://crn.yfazqb.com

Py:   pickle.dumps(obj)
来源：http://kyl.sjlbkw.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://emg.jlsjyb.cn

JS:   v8.serialize(obj)        // Node
来源：http://cpg.birdmap.top

TS:   v8.serialize(obj)        // Node
来源：http://tgm.gotoacloud.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://atu.sufxvd.cn

Go:   encoding/gob
来源：http://cxb.hnqzz.top

Ruby: Marshal.dump(obj)
来源：http://bvu.xziqi.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://cit.zhoulong.xyz

================================================================================
来源：http://btp.vehdjk.com

L. 网络请求
来源：http://dob.svipenyu.cn

================================================================================
来源：http://jjb.kuanghao11.cn

[L01] 发送 GET 请求
来源：http://jgh.cdnleiting.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://vhk.yvedp.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://nfp.tian-w.cn

JS:   await fetch(url)
来源：http://wqx.chenzaomai.com

TS:   await fetch(url)
来源：http://jpq.zhijiandao.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://zdp.zdqjudy.top

Go:   resp, err := http.Get(url)
来源：http://qpm.ehwqpu.com

Ruby: Net::HTTP.get(URI(url))
来源：http://zlv.cucudq.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://rab.cdnleiting.top

[L02] 发送 POST JSON
来源：http://aci.ivvv.top

Py:   requests.post(url, json={"a": 1})
来源：http://jjc.gotoacloud.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://fkg.zhoulong.xyz

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://syp.yfazqb.com

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://fbo.iojbl.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://bvj.9152youxi.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://xoi.yj20258.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://tts.zycfv.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://xqh.sysykeji.top

[L03] 设置自定义请求头
来源：http://jii.yuanzhike.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://gzs.yangfankeji.com

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://scs.yj20258.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://gdf.zhijiandao.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://irf.quarkkingdee.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ssl.shanyushiyangkeji.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://dhk.nwbrower.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ubq.jiagoushi.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://juk.hnqzz.top

[L04] 设置超时
来源：http://nid.yvedp.cn

Py:   requests.get(url, timeout=5)
来源：http://rrz.cqqwz.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://eiv.sufxvd.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://qpo.zdqjudy.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://oot.jqgfzy.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://fix.fengsongda.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://xin.cucudq.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://asa.yuanzhike.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://yro.gaohongyu789.top

[L05] 上传文件（multipart）
来源：http://wjc.hfpthk.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://aye.xuanzx.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://dqk.jinyuanbaomall.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://bxs.jyoumei.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://nur.fanxiaobao.xyz

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://aye.zhengqikj.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://eae.zhijiandao.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://aef.yj20258.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mjk.aizwys.cn

[L06] 解析响应为 JSON
来源：http://jkq.shzxlz.cn

Py:   resp.json()
来源：http://icb.tarul.cn

PHP:  json_decode($body, true);
来源：http://tkq.hesvh.cn

JS:   await resp.json()
来源：http://elw.ivvv.top

TS:   await resp.json()
来源：http://wmr.yvedp.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://lvt.uphjek.com

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://olq.xylfe.cn

Ruby: JSON.parse(resp.body)
来源：http://csc.meibo888.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wld.xziqi.cn

[L07] 处理 HTTP 状态码
来源：http://jfx.ppjwa.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ful.xuanzx.com

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://lhh.zdqjudy.top

JS:   resp.ok;  resp.status
来源：http://ewi.jianghu66.top

TS:   resp.ok;  resp.status
来源：http://bgh.hywenlv.cn

Java: resp.statusCode()
来源：http://ban.tanke756.top

Go:   resp.StatusCode
来源：http://odg.smart0.xyz

Ruby: resp.code.to_i
来源：http://ric.ybcxt.top

C#:   (int)resp.StatusCode
来源：http://xvi.feifeiyinyue.top

[L08] 并发请求多个地址
来源：http://wjc.fengsongda.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://eyq.ydjk.org.cn

PHP:  curl_multi_init() 系列
来源：http://ztg.yj202588.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mto.hnqzz.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://zco.andypj.xyz

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://smi.jyoumei.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://won.wangshuangyany.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wxa.ehwqpu.com

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://fty.fehbvm.com

================================================================================
来源：http://bft.sxryk.cn

M. 命令行 / 进程 / 环境
来源：http://uwv.xziqi.cn

================================================================================
来源：http://jqt.yuanzhike.top

[M01] 读取命令行参数
来源：http://hzs.daxiang520.top

Py:   sys.argv[1:]
来源：http://uti.svipenyu.cn

PHP:  $argv;  $argc;
来源：http://woj.yongpay.top

JS:   process.argv.slice(2)
来源：http://brg.pengpengdd.cyou

TS:   process.argv.slice(2)
来源：http://mrm.cashguo.top

Java: args 数组（main 方法参数）
来源：http://vht.nanxinkj.top

Go:   os.Args[1:]
来源：http://rmk.xuetiantiany.cn

Ruby: ARGV
来源：http://xwk.jinqigufen.top

C#:   args 数组（Main 方法参数）
来源：http://ehk.birdmap.top

[M02] 读取环境变量
来源：http://ujc.daria6918.cn

Py:   os.environ.get("HOME")
来源：http://hwb.ehwqpu.com

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://rco.kuanghao11.cn

JS:   process.env.HOME
来源：http://ijc.dashuyun.cn

TS:   process.env.HOME
来源：http://wxr.sufxvd.cn

Java: System.getenv("HOME")
来源：http://yme.zhoulong.xyz

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://gik.feifeiyinyue.top

Ruby: ENV["HOME"]
来源：http://jcu.svipenyu.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://kls.hywenlv.cn

[M03] 执行外部命令
来源：http://nvl.fengsongda.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://weg.haohaochexian.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://bil.pengpengdd.cyou

JS:   child_process.execSync("ls -l").toString()
来源：http://ljk.vqdsnc.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://rsc.tarul.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://vgw.cucudq.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://vtz.yfazqb.com

Ruby: system("ls -l");  `ls -l`
来源：http://sfg.wangshuangyany.cn

C#:   Process.Start("ls", "-l");
来源：http://fjp.zhengqikj.top

[M04] 获取当前工作目录
来源：http://dnb.xuanzx.com

Py:   os.getcwd()
来源：http://oui.hnqzz.top

PHP:  getcwd();
来源：http://fxz.cashguo.top

JS:   process.cwd()
来源：http://sqk.fengsongda.top

TS:   process.cwd()
来源：http://tuy.jyoumei.cn

Java: Path.of("").toAbsolutePath()
来源：http://glt.yvedp.cn

Go:   os.Getwd()
来源：http://gwi.xuetiantiany.cn

Ruby: Dir.pwd
来源：http://iyt.hnqzz.top

C#:   Directory.GetCurrentDirectory()
来源：http://ecv.cqqwz.cn

[M05] 设置退出码
来源：http://ggz.nwbrower.top

Py:   sys.exit(1)
来源：http://vix.cqqwz.cn

PHP:  exit(1);
来源：http://ueh.yuanzhike.top

JS:   process.exit(1)
来源：http://czd.yonumen.top

TS:   process.exit(1)
来源：http://wph.hammf.cn

Java: System.exit(1)
来源：http://cht.shangyingyoupin.top

Go:   os.Exit(1)
来源：http://kyo.guowangkeji.top

Ruby: exit 1
来源：http://kjq.meibo888.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://rjh.mhx1999.top

[M06] 向标准错误输出
来源：http://txa.yuanzhike.top

Py:   print("err", file=sys.stderr)
来源：http://pjq.yuanzhike.top

PHP:  fwrite(STDERR, "err\n");
来源：http://hil.guowangkeji.top

JS:   console.error("err")
来源：http://fug.sweek.top

TS:   console.error("err")
来源：http://drt.guowangkeji.top

Java: System.err.println("err")
来源：http://kmk.epnwcf.com

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://pzo.shanyushiyangtech.top

Ruby: warn "err"
来源：http://obw.cqqwz.cn

C#:   Console.Error.WriteLine("err")
来源：http://ahi.yj202588.top

[M07] 判断是否为主入口
来源：http://lsj.ydjk.org.cn

Py:   if __name__ == "__main__":
来源：http://rgo.epnwcf.com

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://msq.ybcxt.top

JS:   require.main === module
来源：http://lba.kuanghao11.cn

TS:   require.main === module
来源：http://tot.sysykeji.top

Java: public static void main(String[] args)
来源：http://nny.hammf.cn

Go:   func main()
来源：http://etj.dashuyun.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://eny.wangshuangyany.cn

C#:   static void Main(string[] args)
来源：http://ajg.pengpengdd.cyou

[M08] 获取系统与运行时信息
来源：http://ses.yj202588.top

Py:   platform.system();  platform.python_version()
来源：http://zii.jqgufenzy.top

PHP:  PHP_OS;  phpversion();
来源：http://wtz.chenzaomai.com

JS:   process.platform;  process.version
来源：http://mld.jianghu66.top

TS:   process.platform;  process.version
来源：http://qel.daria6918.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://pzc.yj20258.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://zpo.hongshengwenyu.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://isd.hesvh.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://iyp.haohaochexian.top

================================================================================
来源：http://ykx.pengpengdd.cyou

N. 数据结构与算法
来源：http://jhg.nwbrower.top

================================================================================
来源：http://xan.hywenlv.cn

[N01] 二分查找（有序数组）
来源：http://obr.gogol.net.cn

Py:   bisect.bisect_left(arr, x)
来源：http://vfl.sweek.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ooq.xuetiantiany.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://pot.jyoumei.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://juq.c1oappe.top

Java: Arrays.binarySearch(arr, x)
来源：http://qjz.cucudq.cn

Go:   sort.SearchInts(arr, x)
来源：http://tyg.ctjpmb.com

Ruby: arr.bsearch { |e| e >= x }
来源：http://ocx.yueranfly.top

C#:   Array.BinarySearch(arr, x)
来源：http://rsq.yonumen.top

[N02] 排序（工程实践用内置实现）
来源：http://xzx.sufxvd.cn

Py:   sorted(arr);  arr.sort()
来源：http://ldi.chenzaomai.com

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://upk.xinyue.icu

JS:   [...arr].sort((a, b) => a - b)
来源：http://ypi.zhijiandao.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://fae.feifeiyinyue.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ywn.yfazqb.com

Go:   slices.Sort(arr)
来源：http://tkf.ehwqpu.com

Ruby: arr.sort
来源：http://ueh.jinyuanbaomall.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://ava.hcnkem.com

[N03] 快速排序（分治示例）
来源：http://idl.sweek.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://civ.zdbjq.cn

PHP:  // 递归实现，或用 usort
来源：http://ytm.ctjpmb.com

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://jsr.dashuyun.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://tjv.zhongyouzk.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://jkk.zhoulong.xyz

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ynk.feifeiyinyue.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://toe.hongshengwenyu.top

C#:   // 手写递归，或 Array.Sort
来源：http://uby.quarkkingdee.top

[N04] 斐波那契数列
来源：http://nuw.9152youxi.cn


<!-- 参考信息 -->