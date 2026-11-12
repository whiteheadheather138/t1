代发 wailian999

TS:   new Date("2024-01-02")
来源：http://vqx.xingfuxueyuan.xyz

Java: LocalDate.parse("2024-01-02")
来源：http://iym.ehwqpu.com

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://klj.yj20258888.top

Ruby: Date.parse("2024-01-02")
来源：http://xew.zhaomingkeji.xyz

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://vkn.nanxinkj.top

[J04] 时间戳与日期互转
来源：http://cja.yanxiufei.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://zao.cqqwz.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://fpy.ppjwa.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://svy.yuxming.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://zmr.nwbrower.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ktu.svipenyu.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://bot.cucudq.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://vgb.fktsv.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://obz.xingfuxueyuan.xyz

[J05] 时间加减（加 7 天）
来源：http://eqc.mhx1999.top

Py:   now + timedelta(days=7)
来源：http://wrt.sysykeji.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://cjy.tarul.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://qsw.jinqigufen.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://rhn.guannengcc.top

Java: LocalDate.now().plusDays(7)
来源：http://tja.guowangkeji.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://pdh.hysaishi.cn

Ruby: Time.now + 7 * 86400
来源：http://gqv.zdqjudy.top

C#:   DateTime.Now.AddDays(7)
来源：http://yse.iojbl.cn

[J06] 计算两时间之差
来源：http://xex.316326.xyz

Py:   (end - start).total_seconds()
来源：http://obe.andypj.xyz

PHP:  $end->diff($start)->days;
来源：http://frr.feifeiyinyue.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://wot.shangyingyoupin.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://vux.52xcode.cn

Java: Duration.between(start, end).toSeconds()
来源：http://jup.shuidangran.top

Go:   end.Sub(start).Hours()
来源：http://bdl.cashguo.top

Ruby: end - start                 # 返回秒数
来源：http://azw.chenjidiqi.icu

C#:   (end - start).TotalSeconds
来源：http://wdt.tian-w.cn

[J07] 比较两个日期
来源：http://nvs.yj20258888.top

Py:   d1 < d2;  d1 == d2
来源：http://ysh.ybcxt.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ecq.hywenlv.cn

JS:   d1.getTime() < d2.getTime()
来源：http://eja.cashguo.top

TS:   d1.getTime() < d2.getTime()
来源：http://ctd.guowangkeji.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://oib.nanxuanxn.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://fky.yongpay.top

Ruby: d1 < d2;  d1 == d2
来源：http://qxf.wangshuangyany.cn

C#:   d1 < d2;  d1 == d2
来源：http://ixt.hammf.cn

[J08] 提取年月日与星期
来源：http://heq.chenjidiqi.icu

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://bpw.zhiwuduotai.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://khu.haohaochexian.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://zvm.daxiang520.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://kvw.pengpengdd.cyou

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://spa.vqdsnc.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hon.zhongyouzk.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://aqt.tian-w.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://jeg.aizwys.cn

[J09] 时区处理
来源：http://mdv.zhengqikj.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://bpf.cdnleiting.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://rws.meibo888.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://jkh.hongshengwenyu.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://kzx.hesvh.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hjl.bjfxy.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://bgh.kuanghao11.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://gix.xuanzx.com

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://iqs.zdbjq.cn

[J10] 取今天 / 本月第一天
来源：http://cci.yj20258888.top

Py:   date.today();  date.today().replace(day=1)
来源：http://nay.shanyushiyangtech.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://zcc.zhixingplan.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ihn.xuetiantiany.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://fmp.hongshengwenyu.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://bxa.cucudq.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ckn.haohaochexian.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://lil.jlsjyb.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://pgj.hnqzz.top

================================================================================
来源：http://szz.birdmap.top

K. JSON 与序列化
来源：http://brd.shanyushiyangtech.top

================================================================================
来源：http://lmi.hnqzz.top

[K01] 对象转 JSON 字符串
来源：http://vlh.pycfn.com

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://rbn.haohaochexian.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://whe.snrcjt.cn

JS:   JSON.stringify(obj)
来源：http://uoc.xylfe.cn

TS:   JSON.stringify(obj)
来源：http://yvj.nwbrower.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ilf.kuanghao11.cn

Go:   json.Marshal(obj)
来源：http://jlc.jinqigufen.top

Ruby: obj.to_json                                     // require "json"
来源：http://luc.ivvv.top

C#:   JsonSerializer.Serialize(obj)
来源：http://qel.shzxlz.cn

[K02] JSON 字符串转对象
来源：http://bcv.jqgfzy.top

Py:   json.loads(s)
来源：http://ujw.c1oappe.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ybv.birdmap.top

JS:   JSON.parse(s)
来源：http://paz.smart0.xyz

TS:   JSON.parse(s)
来源：http://rpk.dashuyun.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hzi.zhengqikj.top

Go:   json.Unmarshal(data, &v)
来源：http://cks.hywenlv.cn

Ruby: JSON.parse(s)
来源：http://eyz.ydzc1.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://dix.gaohongyu789.top

[K03] JSON 美化输出（带缩进）
来源：http://kmv.wangdashe.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://udl.9152youxi.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hov.pycfn.com

JS:   JSON.stringify(obj, null, 2)
来源：http://lac.bbcook.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://whp.gaohongyu789.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://raz.tian-w.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ltq.zdbjq.cn

Ruby: JSON.pretty_generate(obj)
来源：http://kzw.ivvv.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://kcr.nanxuanxn.top

[K04] 读取 JSON 文件
来源：http://cll.chenjidiqi.icu

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://mol.birdmap.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://zyg.52xcode.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://quy.uphjek.com

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://fnk.nanxuanxn.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://lij.haohaochexian.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://eoq.wangshuangyany.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://kzx.jinghuilouyu.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://lcu.havefunace.top

[K05] 深拷贝对象
来源：http://gce.yj20258888.top

Py:   copy.deepcopy(obj)
来源：http://dwg.jyoumei.cn

PHP:  unserialize(serialize($obj));
来源：http://ymr.xingfuxueyuan.xyz

JS:   structuredClone(obj)
来源：http://mqc.quarkkingdee.top

TS:   structuredClone(obj)
来源：http://kuq.xingfuxueyuan.xyz

Java: // 手写拷贝构造，或序列化往返
来源：http://xjc.jqgufenzy.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://fyw.feifeiyinyue.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://vqq.shanyushiyangtech.top

C#:   // 序列化往返，或自定义 Clone
来源：http://dcn.feifeiyinyue.top

[K06] 解析 URL 查询串
来源：http://jph.sjlbkw.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://tbd.ctjpmb.com

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://lfy.fanxiaobao.xyz

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mtd.zhijiandao.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://pho.xziqi.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mge.pengpengdd.cyou

Go:   url.ParseQuery("a=1&b=2")
来源：http://xtk.yonumen.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://res.shuidangran.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://eqr.nanxinkj.top

[K07] 进制转换
来源：http://isb.yongpay.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://lpf.meibo888.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://bua.vqdsnc.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://xbu.sweek.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://peh.yfazqb.com

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://uct.316326.xyz

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://iut.nwbrower.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://gwr.yueranfly.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://sms.zhiwuduotai.top

[K08] 二进制序列化（非 JSON）
来源：http://rpe.ppjwa.cn

Py:   pickle.dumps(obj)
来源：http://aus.havefunace.top

PHP:  serialize($obj);  unserialize($s);
来源：http://euj.zhengqikj.top

JS:   v8.serialize(obj)        // Node
来源：http://hdp.jinqigfzy.top

TS:   v8.serialize(obj)        // Node
来源：http://nno.hongshengwenyu.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://npo.daria6918.cn

Go:   encoding/gob
来源：http://jto.kuanghao11.cn

Ruby: Marshal.dump(obj)
来源：http://gdn.yfazqb.com

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://jyn.iojbl.cn

================================================================================
来源：http://oru.jinqigufen.top

L. 网络请求
来源：http://sfk.52xcode.cn

================================================================================
来源：http://yns.sjlbkw.cn

[L01] 发送 GET 请求
来源：http://xbk.gzhubu.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ynf.feifeiyinyue.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://obi.dashuyun.cn

JS:   await fetch(url)
来源：http://qnc.vqdsnc.cn

TS:   await fetch(url)
来源：http://wnf.jyoumei.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hfd.sxryk.cn

Go:   resp, err := http.Get(url)
来源：http://hcb.sweek.top

Ruby: Net::HTTP.get(URI(url))
来源：http://igo.dianchejie.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hgt.zycfv.cn

[L02] 发送 POST JSON
来源：http://vsx.cdnleiting.top

Py:   requests.post(url, json={"a": 1})
来源：http://smr.shangyingyoupin.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://adp.xuetiantiany.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wun.ehwqpu.com

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://vtd.yfazqb.com

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://xzp.yonumen.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://reh.hywenlv.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://jeh.mhx1999.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://lov.gotoacloud.top

[L03] 设置自定义请求头
来源：http://ucn.guowangkeji.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://pam.birdmap.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://asj.shanyushiyangkeji.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ceh.tianlin.xyz

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ezc.nanxuanxn.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wku.ydzc1.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://zja.nanxuanxn.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mou.yanxiufei.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ndb.yj20258.top

[L04] 设置超时
来源：http://ctr.yj20258.top

Py:   requests.get(url, timeout=5)
来源：http://wwc.chenjidiqi.icu

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://uwp.guowangkeji.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://iwk.feifeiyinyue.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://bou.sysykeji.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://haw.cashguo.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://qlx.fengsongda.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ppp.fktsv.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://jtt.gotoacloud.top

[L05] 上传文件（multipart）
来源：http://vgi.tianlin.xyz

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://dxp.hongshengwenyu.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hsj.yfazqb.com

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ytc.hysaishi.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://flo.jlsjyb.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://que.cheryme.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://nou.bjfxy.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://dvs.gzhubu.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://gcr.zhoulong.xyz

[L06] 解析响应为 JSON
来源：http://ofc.yongpay.top

Py:   resp.json()
来源：http://kaj.zhongyouzk.top

PHP:  json_decode($body, true);
来源：http://jef.sweek.top

JS:   await resp.json()
来源：http://eqt.yj202588.top

TS:   await resp.json()
来源：http://qkk.gogol.net.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ulm.jinqigufen.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://tdl.zhixingplan.top

Ruby: JSON.parse(resp.body)
来源：http://yjc.hesvh.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://erp.tianlin.xyz

[L07] 处理 HTTP 状态码
来源：http://lhj.ydjk.org.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://xoi.redwolf501.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wvo.zhengqikj.top

JS:   resp.ok;  resp.status
来源：http://oog.gogol.net.cn

TS:   resp.ok;  resp.status
来源：http://szp.shangyingyoupin.top

Java: resp.statusCode()
来源：http://suy.fzhhl.top

Go:   resp.StatusCode
来源：http://bal.pengpengdd.cyou

Ruby: resp.code.to_i
来源：http://xcr.316326.xyz

C#:   (int)resp.StatusCode
来源：http://lha.ivvv.top

[L08] 并发请求多个地址
来源：http://zkh.vqdsnc.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://aeb.zhoulong.xyz

PHP:  curl_multi_init() 系列
来源：http://ghk.yueranfly.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://jnq.316326.xyz

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://xyv.jianghu66.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://bwp.snrcjt.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://jtn.jinqigfzy.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://aae.zhongyouzk.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://bdc.xinyue.icu

================================================================================
来源：http://wus.dashuyun.cn

M. 命令行 / 进程 / 环境
来源：http://lif.fanxiaobao.xyz

================================================================================
来源：http://qzj.yongpay.top

[M01] 读取命令行参数
来源：http://uab.zhengqikj.top

Py:   sys.argv[1:]
来源：http://nvf.sweek.top

PHP:  $argv;  $argc;
来源：http://eki.hesvh.cn

JS:   process.argv.slice(2)
来源：http://sqi.fanxiaobao.xyz

TS:   process.argv.slice(2)
来源：http://nmq.havefunace.top

Java: args 数组（main 方法参数）
来源：http://cgg.uphjek.com

Go:   os.Args[1:]
来源：http://mbb.shangyingyoupin.top

Ruby: ARGV
来源：http://mtk.tanke756.top

C#:   args 数组（Main 方法参数）
来源：http://gmn.gzhubu.top

[M02] 读取环境变量
来源：http://fqh.xuetiantiany.cn

Py:   os.environ.get("HOME")
来源：http://zgl.jiagoushi.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://spu.shanyushiyangkeji.top

JS:   process.env.HOME
来源：http://txa.zdqjudy.top

TS:   process.env.HOME
来源：http://kjx.daxiang520.top

Java: System.getenv("HOME")
来源：http://mgc.chenjidiqi.icu

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://jbi.9152youxi.cn

Ruby: ENV["HOME"]
来源：http://ulb.gotoacloud.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://okq.sufxvd.cn

[M03] 执行外部命令
来源：http://uuk.fzhhl.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://jqp.redwolf501.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://dmx.sysykeji.top

JS:   child_process.execSync("ls -l").toString()
来源：http://jka.jinqigufen.top

TS:   child_process.execSync("ls -l").toString()
来源：http://mhr.hfpthk.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://sar.zhixingplan.top

Go:   exec.Command("ls", "-l").Output()
来源：http://dtc.gotoacloud.top

Ruby: system("ls -l");  `ls -l`
来源：http://zjs.hongshengwenyu.top

C#:   Process.Start("ls", "-l");
来源：http://kya.xinyue.icu

[M04] 获取当前工作目录
来源：http://iul.redwolf501.top

Py:   os.getcwd()
来源：http://skq.yueranfly.top

PHP:  getcwd();
来源：http://ikf.jinyuanbaomall.cn

JS:   process.cwd()
来源：http://oyl.yuanzhike.top

TS:   process.cwd()
来源：http://mgx.bjfxy.top

Java: Path.of("").toAbsolutePath()
来源：http://jol.gotoacloud.top

Go:   os.Getwd()
来源：http://zrb.tian-w.cn

Ruby: Dir.pwd
来源：http://zgc.yj202588.top

C#:   Directory.GetCurrentDirectory()
来源：http://kam.xziqi.cn

[M05] 设置退出码
来源：http://wwd.shangyingyoupin.top

Py:   sys.exit(1)
来源：http://okm.yvedp.cn

PHP:  exit(1);
来源：http://tar.sweek.top

JS:   process.exit(1)
来源：http://pfl.snrcjt.cn

TS:   process.exit(1)
来源：http://dig.dashuyun.cn

Java: System.exit(1)
来源：http://jjc.uphjek.com

Go:   os.Exit(1)
来源：http://kbc.shzxlz.cn

Ruby: exit 1
来源：http://hff.cheryme.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://bda.hammf.cn

[M06] 向标准错误输出
来源：http://ypk.c1oappe.top

Py:   print("err", file=sys.stderr)
来源：http://opx.ydzc1.top

PHP:  fwrite(STDERR, "err\n");
来源：http://xxj.gzhubu.top

JS:   console.error("err")
来源：http://tpk.quarkkingdee.top

TS:   console.error("err")
来源：http://hie.zhoulong.xyz

Java: System.err.println("err")
来源：http://fmq.jyoumei.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ire.nanxuanxn.top

Ruby: warn "err"
来源：http://ian.jinghuilouyu.cn

C#:   Console.Error.WriteLine("err")
来源：http://ehj.jinqigfzy.top

[M07] 判断是否为主入口
来源：http://xra.zhiwuduotai.top

Py:   if __name__ == "__main__":
来源：http://eqc.epnwcf.com

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://kfd.316326.xyz

JS:   require.main === module
来源：http://bcj.sysykeji.top

TS:   require.main === module
来源：http://lek.nanxinkj.top

Java: public static void main(String[] args)
来源：http://qws.xinyue.icu

Go:   func main()
来源：http://bmi.shzxlz.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://bbq.gzhubu.top

C#:   static void Main(string[] args)
来源：http://yhz.gzhubu.top

[M08] 获取系统与运行时信息
来源：http://vhk.yuxming.cn

Py:   platform.system();  platform.python_version()
来源：http://jje.daria6918.cn

PHP:  PHP_OS;  phpversion();
来源：http://nrs.yj202588.top

JS:   process.platform;  process.version
来源：http://nzg.c1oappe.top

TS:   process.platform;  process.version
来源：http://ozf.zhijiandao.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://lec.xinyue.icu

Go:   runtime.GOOS;  runtime.Version()
来源：http://qlq.hywenlv.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://kjf.jinyuanbaomall.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://xcx.xingfuxueyuan.xyz

================================================================================
来源：http://mmt.52xcode.cn

N. 数据结构与算法
来源：http://lsn.xziqi.cn

================================================================================
来源：http://jnx.zdqjudy.top

[N01] 二分查找（有序数组）
来源：http://aah.zhengqikj.top

Py:   bisect.bisect_left(arr, x)
来源：http://ghe.cqqwz.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://vnb.0kj1m.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mux.hnxiangtu.top


<!-- 参考信息 -->