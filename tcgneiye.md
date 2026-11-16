代发 wailian999

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://voh.aizwys.cn

[J04] 时间戳与日期互转
来源：http://cfi.yanxiufei.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://nbu.xziqi.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://gqp.jinyuanbaomall.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://jgg.zhaomingkeji.xyz

TS:   Math.floor(Date.now() / 1000)
来源：http://nan.fengsongda.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://cdz.redwolf501.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://frn.zhaomingkeji.xyz

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://dwm.0kj1m.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://elf.nanxinkj.top

[J05] 时间加减（加 7 天）
来源：http://xgb.hfpthk.cn

Py:   now + timedelta(days=7)
来源：http://giw.tian-w.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://aqz.nanxinkj.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://zll.guowangkeji.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://iir.smart0.xyz

Java: LocalDate.now().plusDays(7)
来源：http://hbw.9152youxi.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://lky.gzhubu.top

Ruby: Time.now + 7 * 86400
来源：http://jsg.shangyingyoupin.top

C#:   DateTime.Now.AddDays(7)
来源：http://smm.gogol.net.cn

[J06] 计算两时间之差
来源：http://kqj.yanxiufei.cn

Py:   (end - start).total_seconds()
来源：http://kww.cashguo.top

PHP:  $end->diff($start)->days;
来源：http://qwd.nanxuanxn.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://iat.feifeiyinyue.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://rtm.hnqzz.top

Java: Duration.between(start, end).toSeconds()
来源：http://gce.cheryme.top

Go:   end.Sub(start).Hours()
来源：http://uyi.bjfxy.top

Ruby: end - start                 # 返回秒数
来源：http://zge.daxiang520.top

C#:   (end - start).TotalSeconds
来源：http://asf.chenlongwang.top

[J07] 比较两个日期
来源：http://ktm.chenjidiqi.icu

Py:   d1 < d2;  d1 == d2
来源：http://cgb.yuxming.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://egm.daria6918.cn

JS:   d1.getTime() < d2.getTime()
来源：http://eiq.hywenlv.cn

TS:   d1.getTime() < d2.getTime()
来源：http://ytm.jinqigfzy.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://zjm.haohaochexian.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://yas.jlsjyb.cn

Ruby: d1 < d2;  d1 == d2
来源：http://tuu.zhiwuduotai.top

C#:   d1 < d2;  d1 == d2
来源：http://hfh.yanxiufei.cn

[J08] 提取年月日与星期
来源：http://qdf.jlsjyb.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://lhq.ivvv.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://vhg.dashuyun.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://jka.daria6918.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://awe.fehbvm.com

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://dfo.havefunace.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://kyy.zhijiandao.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://owq.hysaishi.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ajj.ybcxt.top

[J09] 时区处理
来源：http://npo.aibaodan.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://jqd.ehwqpu.com

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://lsr.zhiwuduotai.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://jhu.snrcjt.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://vde.hongshengwenyu.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://vac.vehdjk.com

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://avj.tanke756.top

Ruby: Time.now.getlocal("+08:00")
来源：http://rlc.sysykeji.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://rjt.yfazqb.com

[J10] 取今天 / 本月第一天
来源：http://ztx.yj20258.top

Py:   date.today();  date.today().replace(day=1)
来源：http://wno.fengsongda.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://tfe.nanxuanxn.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://map.cashguo.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://xye.zhijiandao.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://pft.kuanghao11.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://vhg.hysaishi.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://vma.hcnkem.com

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://afh.fengsongda.top

================================================================================
来源：http://gje.ctjpmb.com

K. JSON 与序列化
来源：http://afz.uphjek.com

================================================================================
来源：http://pee.daxiang520.top

[K01] 对象转 JSON 字符串
来源：http://tap.epnwcf.com

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://obm.cashguo.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://bfv.guowangkeji.top

JS:   JSON.stringify(obj)
来源：http://ltl.jqgfzy.top

TS:   JSON.stringify(obj)
来源：http://vqj.jinqigufen.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hdv.yj20258.top

Go:   json.Marshal(obj)
来源：http://wom.vehdjk.com

Ruby: obj.to_json                                     // require "json"
来源：http://dmx.fehbvm.com

C#:   JsonSerializer.Serialize(obj)
来源：http://kdz.gotoacloud.top

[K02] JSON 字符串转对象
来源：http://xua.cdnleiting.top

Py:   json.loads(s)
来源：http://ijo.fengsongda.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ldm.yangfankeji.com

JS:   JSON.parse(s)
来源：http://sxd.ydjk.org.cn

TS:   JSON.parse(s)
来源：http://ggl.ctjpmb.com

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://qzn.cdnleiting.top

Go:   json.Unmarshal(data, &v)
来源：http://xep.316326.xyz

Ruby: JSON.parse(s)
来源：http://lpz.fengsongda.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://pof.cdnleiting.top

[K03] JSON 美化输出（带缩进）
来源：http://rig.vehdjk.com

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://cha.havefunace.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://xov.jyoumei.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://hll.316326.xyz

TS:   JSON.stringify(obj, null, 2)
来源：http://qic.fktsv.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://svr.yj20258.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hox.hywenlv.cn

Ruby: JSON.pretty_generate(obj)
来源：http://gmd.sjlbkw.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://orw.zhijiandao.cn

[K04] 读取 JSON 文件
来源：http://fvu.zhongyouzk.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://fby.snrcjt.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://fdn.birdmap.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mhc.xingfuxueyuan.xyz

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://zzl.sufxvd.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://zqa.fzhhl.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://nqe.fengsongda.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://lab.yj202588.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://sne.9152youxi.cn

[K05] 深拷贝对象
来源：http://xuq.yfazqb.com

Py:   copy.deepcopy(obj)
来源：http://teb.yuxming.cn

PHP:  unserialize(serialize($obj));
来源：http://txf.pycfn.com

JS:   structuredClone(obj)
来源：http://qsv.nwbrower.top

TS:   structuredClone(obj)
来源：http://fsu.bjfxy.top

Java: // 手写拷贝构造，或序列化往返
来源：http://ltb.chenjidiqi.icu

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wlt.guowangkeji.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://kdu.jianghu66.top

C#:   // 序列化往返，或自定义 Clone
来源：http://jqa.feifeiyinyue.top

[K06] 解析 URL 查询串
来源：http://vro.iojbl.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://bsc.zhaomingkeji.xyz

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mic.shuidangran.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://inh.zhoulong.xyz

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://zfc.cdnleiting.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://zml.nanxinkj.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://jzc.jinqigufen.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://yfe.hysaishi.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://dzj.jyoumei.cn

[K07] 进制转换
来源：http://miz.havefunace.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://lzr.sjlbkw.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://vtl.bjfxy.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://viv.jinghuilouyu.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://yjs.snrcjt.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://jwe.jlsjyb.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://drt.gotoacloud.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ptu.ywan-chungtsiang.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://cdc.cheryme.top

[K08] 二进制序列化（非 JSON）
来源：http://jzp.hesvh.cn

Py:   pickle.dumps(obj)
来源：http://vvt.yvedp.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://axg.ydjk.org.cn

JS:   v8.serialize(obj)        // Node
来源：http://nvr.jianghu66.top

TS:   v8.serialize(obj)        // Node
来源：http://jbr.meibo888.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://odj.zhaomingkeji.xyz

Go:   encoding/gob
来源：http://ylr.nanxuanxn.top

Ruby: Marshal.dump(obj)
来源：http://mrv.gaohongyu789.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://aux.yj20258888.top

================================================================================
来源：http://uuw.kuanghao11.cn

L. 网络请求
来源：http://dog.xuanzx.com

================================================================================
来源：http://bna.aizwys.cn

[L01] 发送 GET 请求
来源：http://cxk.snrcjt.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://gqm.316326.xyz

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ugi.yj20258.top

JS:   await fetch(url)
来源：http://yyh.9152youxi.cn

TS:   await fetch(url)
来源：http://tqx.aizwys.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://lwl.meibo888.top

Go:   resp, err := http.Get(url)
来源：http://kby.xuetiantiany.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://uvc.gotoacloud.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ptf.feifeiyinyue.top

[L02] 发送 POST JSON
来源：http://dee.jinghuilouyu.cn

Py:   requests.post(url, json={"a": 1})
来源：http://dvp.hammf.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://opf.jiagoushi.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hwj.xuanzx.com

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ajx.cheryme.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://bdn.haohaochexian.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://brh.yvedp.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://bwj.zdqjudy.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://pxt.xuanzx.com

[L03] 设置自定义请求头
来源：http://qog.jinqigufen.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://zne.fehbvm.com

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://dbf.svipenyu.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://qld.bbcook.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://cun.yj20258.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://nki.tianlin.xyz

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mnv.aizwys.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://utf.xuanzx.com

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ara.yvedp.cn

[L04] 设置超时
来源：http://ttg.jqgufenzy.top

Py:   requests.get(url, timeout=5)
来源：http://ctd.sysykeji.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://fzb.jqgfzy.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://fkl.yueranfly.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://uqz.pycfn.com

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ldq.hcnkem.com

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://xxz.hnqzz.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://jok.zhixingplan.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://aix.sufxvd.cn

[L05] 上传文件（multipart）
来源：http://wzb.haohaochexian.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://vlf.chenjidiqi.icu

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://xtd.chenlongwang.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ppp.xuanzx.com

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://pux.shangyingyoupin.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://pkn.hfpthk.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://dwv.jlsjyb.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://muz.zdbjq.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://qtb.zhongyouzk.top

[L06] 解析响应为 JSON
来源：http://wyq.aizwys.cn

Py:   resp.json()
来源：http://edd.sjlbkw.cn

PHP:  json_decode($body, true);
来源：http://enq.fzhhl.top

JS:   await resp.json()
来源：http://ewc.0kj1m.cn

TS:   await resp.json()
来源：http://suk.kuanghao11.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wds.fktsv.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://olt.chenzaomai.com

Ruby: JSON.parse(resp.body)
来源：http://kfb.shzxlz.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wpx.ydzc1.top

[L07] 处理 HTTP 状态码
来源：http://wcv.kuanghao11.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://idt.wangshuangyany.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://avo.havefunace.top

JS:   resp.ok;  resp.status
来源：http://mto.chenjidiqi.icu

TS:   resp.ok;  resp.status
来源：http://yod.jiagoushi.top

Java: resp.statusCode()
来源：http://wbc.jianghu66.top

Go:   resp.StatusCode
来源：http://byl.pengpengdd.cyou

Ruby: resp.code.to_i
来源：http://pgz.zhongyouzk.top

C#:   (int)resp.StatusCode
来源：http://spr.birdmap.top

[L08] 并发请求多个地址
来源：http://yzr.shangyingyoupin.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://nsh.gzhubu.top

PHP:  curl_multi_init() 系列
来源：http://psa.xinyue.icu

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://cgx.52xcode.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://imx.zhongyouzk.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://tgq.yueranfly.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://pie.meibo888.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://pum.nanxinkj.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://tto.xingfuxueyuan.xyz

================================================================================
来源：http://kng.jinghuilouyu.cn

M. 命令行 / 进程 / 环境
来源：http://fqv.ivvv.top

================================================================================
来源：http://akf.aibaodan.cn

[M01] 读取命令行参数
来源：http://wcq.yueranfly.top

Py:   sys.argv[1:]
来源：http://xnw.tianlin.xyz

PHP:  $argv;  $argc;
来源：http://feh.svipenyu.cn

JS:   process.argv.slice(2)
来源：http://qit.hywenlv.cn

TS:   process.argv.slice(2)
来源：http://rpz.hesvh.cn

Java: args 数组（main 方法参数）
来源：http://onl.gaohongyu789.top

Go:   os.Args[1:]
来源：http://pkk.zhongyouzk.top

Ruby: ARGV
来源：http://hfi.gzhubu.top

C#:   args 数组（Main 方法参数）
来源：http://yir.epnwcf.com

[M02] 读取环境变量
来源：http://ztm.dashuyun.cn

Py:   os.environ.get("HOME")
来源：http://hto.sxryk.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://acl.zhoulong.xyz

JS:   process.env.HOME
来源：http://qak.yvedp.cn

TS:   process.env.HOME
来源：http://oat.ctjpmb.com

Java: System.getenv("HOME")
来源：http://pla.jiagoushi.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://lue.tian-w.cn

Ruby: ENV["HOME"]
来源：http://boi.tianlin.xyz

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ecl.andypj.xyz

[M03] 执行外部命令
来源：http://eoy.snrcjt.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://lut.hnqzz.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://par.yfazqb.com

JS:   child_process.execSync("ls -l").toString()
来源：http://rwt.kuanghao11.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://dgc.jinyuanbaomall.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://xrc.jyoumei.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://tus.dashuyun.cn

Ruby: system("ls -l");  `ls -l`
来源：http://hhp.redwolf501.top

C#:   Process.Start("ls", "-l");
来源：http://yhw.tian-w.cn

[M04] 获取当前工作目录
来源：http://fgp.nanxinkj.top

Py:   os.getcwd()
来源：http://drz.tian-w.cn

PHP:  getcwd();
来源：http://lrc.yj20258.top

JS:   process.cwd()
来源：http://any.gotoacloud.top

TS:   process.cwd()
来源：http://aem.hnxiangtu.top

Java: Path.of("").toAbsolutePath()
来源：http://exv.hnxiangtu.top

Go:   os.Getwd()
来源：http://apg.feifeiyinyue.top

Ruby: Dir.pwd
来源：http://njj.gaohongyu789.top

C#:   Directory.GetCurrentDirectory()
来源：http://qrf.52xcode.cn

[M05] 设置退出码
来源：http://eno.nanxuanxn.top

Py:   sys.exit(1)
来源：http://mqf.svipenyu.cn

PHP:  exit(1);
来源：http://nqs.ywan-chungtsiang.top

JS:   process.exit(1)
来源：http://pqt.sjlbkw.cn

TS:   process.exit(1)
来源：http://nro.hfpthk.cn

Java: System.exit(1)
来源：http://vnd.9152youxi.cn

Go:   os.Exit(1)
来源：http://txz.jinyuanbaomall.cn

Ruby: exit 1
来源：http://xqi.xziqi.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://djb.0kj1m.cn

[M06] 向标准错误输出
来源：http://kij.sysykeji.top

Py:   print("err", file=sys.stderr)
来源：http://kbh.aizwys.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://bcz.yj20258.top

JS:   console.error("err")
来源：http://zzs.ydzc1.top

TS:   console.error("err")
来源：http://wfh.fengsongda.top

Java: System.err.println("err")
来源：http://bvw.xinyue.icu

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://vso.redwolf501.top

Ruby: warn "err"
来源：http://ura.zhixingplan.top

C#:   Console.Error.WriteLine("err")
来源：http://bdr.smart0.xyz

[M07] 判断是否为主入口
来源：http://klr.tian-w.cn

Py:   if __name__ == "__main__":
来源：http://pae.yongpay.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://lsp.chenlongwang.top

JS:   require.main === module
来源：http://hhp.zycfv.cn

TS:   require.main === module
来源：http://oft.zdqjudy.top

Java: public static void main(String[] args)
来源：http://ack.jinqigufen.top

Go:   func main()
来源：http://kka.redwolf501.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://obk.feifeiyinyue.top

C#:   static void Main(string[] args)
来源：http://ikr.shanyushiyangtech.top

[M08] 获取系统与运行时信息
来源：http://lta.iojbl.cn

Py:   platform.system();  platform.python_version()
来源：http://kux.gzhubu.top

PHP:  PHP_OS;  phpversion();
来源：http://uox.haohaochexian.top

JS:   process.platform;  process.version
来源：http://fay.xuetiantiany.cn

TS:   process.platform;  process.version
来源：http://bbf.nanxuanxn.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://opm.shuidangran.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://iyd.ctjpmb.com

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://jgl.jqgfzy.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://xej.ehwqpu.com

================================================================================
来源：http://ujf.hywenlv.cn

N. 数据结构与算法
来源：http://kms.ctjpmb.com

================================================================================
来源：http://cts.hongshengwenyu.top

[N01] 二分查找（有序数组）
来源：http://bwx.fzhhl.top

Py:   bisect.bisect_left(arr, x)
来源：http://vct.ivvv.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://tdh.pengpengdd.cyou

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://zfu.hfpthk.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://cir.cdnleiting.top

Java: Arrays.binarySearch(arr, x)
来源：http://sqv.yongpay.top

Go:   sort.SearchInts(arr, x)
来源：http://wfh.yj202588.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://rhw.c1oappe.top


<!-- 参考信息 -->