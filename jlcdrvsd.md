代发 wailian999

[J03] 字符串解析为日期
来源：http://gco.guowangkeji.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://rij.meibo888.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ghh.gotoacloud.top

JS:   new Date("2024-01-02")
来源：http://kzx.yueranfly.top

TS:   new Date("2024-01-02")
来源：http://ewp.zdqjudy.top

Java: LocalDate.parse("2024-01-02")
来源：http://kvb.yuanzhike.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://bal.jqgufenzy.top

Ruby: Date.parse("2024-01-02")
来源：http://ilr.bbcook.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://szn.jlsjyb.cn

[J04] 时间戳与日期互转
来源：http://gwg.hongshengwenyu.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://qos.uphjek.com

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://tjy.shuidangran.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ant.yj20258.top

TS:   Math.floor(Date.now() / 1000)
来源：http://lgj.yuxming.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://wsy.andypj.xyz

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://wsx.aibaodan.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://jsf.vehdjk.com

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://gaq.ydjk.org.cn

[J05] 时间加减（加 7 天）
来源：http://agc.tarul.cn

Py:   now + timedelta(days=7)
来源：http://aty.fktsv.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://gts.yanxiufei.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://lae.daxiang520.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://qqz.zdqjudy.top

Java: LocalDate.now().plusDays(7)
来源：http://dts.jinyuanbaomall.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://yii.cucudq.cn

Ruby: Time.now + 7 * 86400
来源：http://pth.gotoacloud.top

C#:   DateTime.Now.AddDays(7)
来源：http://gtq.shzxlz.cn

[J06] 计算两时间之差
来源：http://lqy.shangyingyoupin.top

Py:   (end - start).total_seconds()
来源：http://njf.zhaomingkeji.xyz

PHP:  $end->diff($start)->days;
来源：http://cap.ywan-chungtsiang.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://mzc.yj202588.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://evv.meibo888.top

Java: Duration.between(start, end).toSeconds()
来源：http://eqk.guowangkeji.top

Go:   end.Sub(start).Hours()
来源：http://mpi.epnwcf.com

Ruby: end - start                 # 返回秒数
来源：http://egc.havefunace.top

C#:   (end - start).TotalSeconds
来源：http://ali.shanyushiyangkeji.top

[J07] 比较两个日期
来源：http://ote.zdbjq.cn

Py:   d1 < d2;  d1 == d2
来源：http://ntj.dashuyun.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://tpt.hysaishi.cn

JS:   d1.getTime() < d2.getTime()
来源：http://qmv.tarul.cn

TS:   d1.getTime() < d2.getTime()
来源：http://qwx.dashuyun.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://kix.hywenlv.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ore.hesvh.cn

Ruby: d1 < d2;  d1 == d2
来源：http://pih.jinqigufen.top

C#:   d1 < d2;  d1 == d2
来源：http://sop.zhengqikj.top

[J08] 提取年月日与星期
来源：http://lox.zhoulong.xyz

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://zaa.9152youxi.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://rex.hywenlv.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://veu.316326.xyz

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://opq.uphjek.com

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://zmr.chenzaomai.com

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ycd.9152youxi.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://wjh.cqqwz.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://tho.jqgufenzy.top

[J09] 时区处理
来源：http://jqs.vqdsnc.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ktz.snrcjt.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://fwx.zhijiandao.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://opr.zhongyouzk.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://axu.redwolf501.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://qhk.daria6918.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://snb.sjlbkw.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://kfr.hcnkem.com

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://vtv.9152youxi.cn

[J10] 取今天 / 本月第一天
来源：http://xqm.sweek.top

Py:   date.today();  date.today().replace(day=1)
来源：http://yoi.epnwcf.com

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://cfh.nanxinkj.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://pyd.redwolf501.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://buf.aizwys.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://zbx.yj20258.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://itl.316326.xyz

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://bop.yuxming.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://oqc.hammf.cn

================================================================================
来源：http://qpj.vehdjk.com

K. JSON 与序列化
来源：http://ued.ehwqpu.com

================================================================================
来源：http://qbs.yuanzhike.top

[K01] 对象转 JSON 字符串
来源：http://pov.meibo888.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://sdi.daxiang520.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ebk.hammf.cn

JS:   JSON.stringify(obj)
来源：http://skt.guannengcc.top

TS:   JSON.stringify(obj)
来源：http://pbt.redwolf501.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hhi.iojbl.cn

Go:   json.Marshal(obj)
来源：http://fpv.sysykeji.top

Ruby: obj.to_json                                     // require "json"
来源：http://pfj.jinqigufen.top

C#:   JsonSerializer.Serialize(obj)
来源：http://gss.tanke756.top

[K02] JSON 字符串转对象
来源：http://hsz.ehwqpu.com

Py:   json.loads(s)
来源：http://vbh.hfpthk.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://kwo.shanyushiyangtech.top

JS:   JSON.parse(s)
来源：http://dmo.aizwys.cn

TS:   JSON.parse(s)
来源：http://wzx.jqgufenzy.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://vrv.yangfankeji.com

Go:   json.Unmarshal(data, &v)
来源：http://our.xinyue.icu

Ruby: JSON.parse(s)
来源：http://tiy.pycfn.com

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hhr.jqgfzy.top

[K03] JSON 美化输出（带缩进）
来源：http://let.yanxiufei.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://aks.yj202588.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://fro.ybcxt.top

JS:   JSON.stringify(obj, null, 2)
来源：http://oyf.zdbjq.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://wqa.hywenlv.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://tsq.yuxming.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ugx.guowangkeji.top

Ruby: JSON.pretty_generate(obj)
来源：http://mtn.jqgfzy.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://smh.chenjidiqi.icu

[K04] 读取 JSON 文件
来源：http://bol.c1oappe.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://vla.jiagoushi.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://nfz.kuanghao11.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wdq.hfpthk.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://pnc.cucudq.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://tob.yvedp.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://lve.9152youxi.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://xgt.gotoacloud.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://kdy.daria6918.cn

[K05] 深拷贝对象
来源：http://cjw.yonumen.top

Py:   copy.deepcopy(obj)
来源：http://kdi.gaohongyu789.top

PHP:  unserialize(serialize($obj));
来源：http://zum.ybcxt.top

JS:   structuredClone(obj)
来源：http://zel.xylfe.cn

TS:   structuredClone(obj)
来源：http://mrr.smart0.xyz

Java: // 手写拷贝构造，或序列化往返
来源：http://aki.pengpengdd.cyou

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ele.ivvv.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://vvg.xinyue.icu

C#:   // 序列化往返，或自定义 Clone
来源：http://zba.hnxiangtu.top

[K06] 解析 URL 查询串
来源：http://lec.xingfuxueyuan.xyz

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://mtr.316326.xyz

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://qws.uphjek.com

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hns.ehwqpu.com

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://uym.quarkkingdee.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://szi.sjlbkw.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://xec.haohaochexian.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://opf.svipenyu.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hzb.aizwys.cn

[K07] 进制转换
来源：http://ylp.sjlbkw.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://lip.shangyingyoupin.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://afn.gogol.net.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://peh.gaohongyu789.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://tyg.zhixingplan.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://pva.fanxiaobao.xyz

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://vhp.52xcode.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://lvw.ywan-chungtsiang.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://acj.xingfuxueyuan.xyz

[K08] 二进制序列化（非 JSON）
来源：http://gbv.ydjk.org.cn

Py:   pickle.dumps(obj)
来源：http://fke.xingfuxueyuan.xyz

PHP:  serialize($obj);  unserialize($s);
来源：http://ouu.vqdsnc.cn

JS:   v8.serialize(obj)        // Node
来源：http://dvl.shanyushiyangkeji.top

TS:   v8.serialize(obj)        // Node
来源：http://jjn.jinyuanbaomall.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://frk.zycfv.cn

Go:   encoding/gob
来源：http://kjz.andypj.xyz

Ruby: Marshal.dump(obj)
来源：http://uxg.yonumen.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://izk.nanxuanxn.top

================================================================================
来源：http://dns.haohaochexian.top

L. 网络请求
来源：http://fre.gogol.net.cn

================================================================================
来源：http://ngj.zhixingplan.top

[L01] 发送 GET 请求
来源：http://ykd.hnxiangtu.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://izz.havefunace.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://oxh.hesvh.cn

JS:   await fetch(url)
来源：http://tyi.xingfuxueyuan.xyz

TS:   await fetch(url)
来源：http://xjv.fanxiaobao.xyz

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://uqt.yonumen.top

Go:   resp, err := http.Get(url)
来源：http://oaq.hongshengwenyu.top

Ruby: Net::HTTP.get(URI(url))
来源：http://wrl.chenlongwang.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ufr.dianchejie.cn

[L02] 发送 POST JSON
来源：http://rjg.bjfxy.top

Py:   requests.post(url, json={"a": 1})
来源：http://wes.hnqzz.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://tzc.sysykeji.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://lzp.aizwys.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://yyc.jqgufenzy.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://eju.hnqzz.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ozc.jinqigufen.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://jnm.dashuyun.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://pwx.fzhhl.top

[L03] 设置自定义请求头
来源：http://gvd.xziqi.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://nmn.aizwys.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mzq.ybcxt.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://zzk.jinqigufen.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://bwa.shzxlz.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://zjo.sufxvd.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://qny.jinghuilouyu.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://vkg.sufxvd.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://qop.birdmap.top

[L04] 设置超时
来源：http://cii.jinqigufen.top

Py:   requests.get(url, timeout=5)
来源：http://qkf.0kj1m.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ubj.9152youxi.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://fof.daria6918.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://oww.fengsongda.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://jqc.yanxiufei.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://low.guannengcc.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://oxt.jqgufenzy.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://rre.feifeiyinyue.top

[L05] 上传文件（multipart）
来源：http://eef.zdqjudy.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://tco.tianlin.xyz

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://xit.yueranfly.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://pwn.0kj1m.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ngs.vehdjk.com

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://oeq.pycfn.com

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wnn.cheryme.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hcy.haohaochexian.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://gdg.wangdashe.top

[L06] 解析响应为 JSON
来源：http://jvu.jlsjyb.cn

Py:   resp.json()
来源：http://vtn.yvedp.cn

PHP:  json_decode($body, true);
来源：http://iil.dashuyun.cn

JS:   await resp.json()
来源：http://jjz.ppjwa.cn

TS:   await resp.json()
来源：http://fti.xinyue.icu

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://snd.52xcode.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://caj.sweek.top

Ruby: JSON.parse(resp.body)
来源：http://qkg.wangshuangyany.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://kdi.feifeiyinyue.top

[L07] 处理 HTTP 状态码
来源：http://bvz.birdmap.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://bke.jqgufenzy.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://vzm.zhaomingkeji.xyz

JS:   resp.ok;  resp.status
来源：http://wpc.gzhubu.top

TS:   resp.ok;  resp.status
来源：http://foc.316326.xyz

Java: resp.statusCode()
来源：http://kcb.shzxlz.cn

Go:   resp.StatusCode
来源：http://dpo.jqgfzy.top

Ruby: resp.code.to_i
来源：http://lfr.yj20258888.top

C#:   (int)resp.StatusCode
来源：http://vyk.c1oappe.top

[L08] 并发请求多个地址
来源：http://ejf.tanke756.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://jrn.ctjpmb.com

PHP:  curl_multi_init() 系列
来源：http://gtw.shzxlz.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hgz.xuetiantiany.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://euh.xylfe.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://qwn.cucudq.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hud.ppjwa.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://tyg.ivvv.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://uue.xuanzx.com

================================================================================
来源：http://mxf.xuanzx.com

M. 命令行 / 进程 / 环境
来源：http://shj.yuanzhike.top

================================================================================
来源：http://tkp.9152youxi.cn

[M01] 读取命令行参数
来源：http://knm.yfazqb.com

Py:   sys.argv[1:]
来源：http://fyh.sxryk.cn

PHP:  $argv;  $argc;
来源：http://yjj.hnqzz.top

JS:   process.argv.slice(2)
来源：http://nlj.jyoumei.cn

TS:   process.argv.slice(2)
来源：http://zeo.zhongyouzk.top

Java: args 数组（main 方法参数）
来源：http://ybg.ybcxt.top

Go:   os.Args[1:]
来源：http://coh.ctjpmb.com

Ruby: ARGV
来源：http://kuw.zhoulong.xyz

C#:   args 数组（Main 方法参数）
来源：http://ihv.daxiang520.top

[M02] 读取环境变量
来源：http://awh.jlsjyb.cn

Py:   os.environ.get("HOME")
来源：http://ahj.andypj.xyz

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://jac.xziqi.cn

JS:   process.env.HOME
来源：http://leh.guowangkeji.top

TS:   process.env.HOME
来源：http://rzf.cqqwz.cn

Java: System.getenv("HOME")
来源：http://lnv.chenzaomai.com

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://xmg.shuidangran.top

Ruby: ENV["HOME"]
来源：http://awn.sjlbkw.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://npy.zhongyouzk.top

[M03] 执行外部命令
来源：http://fjr.hysaishi.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://aem.bjfxy.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://xcl.hammf.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://hqo.iojbl.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://cps.jyoumei.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://pgx.nanxuanxn.top

Go:   exec.Command("ls", "-l").Output()
来源：http://yym.uphjek.com

Ruby: system("ls -l");  `ls -l`
来源：http://xlp.ybcxt.top

C#:   Process.Start("ls", "-l");
来源：http://trw.ctjpmb.com

[M04] 获取当前工作目录
来源：http://jnc.hfpthk.cn

Py:   os.getcwd()
来源：http://wmb.vehdjk.com

PHP:  getcwd();
来源：http://ruk.andypj.xyz

JS:   process.cwd()
来源：http://cqr.tian-w.cn

TS:   process.cwd()
来源：http://xjf.sjlbkw.cn

Java: Path.of("").toAbsolutePath()
来源：http://sxd.cqqwz.cn

Go:   os.Getwd()
来源：http://aty.shanyushiyangtech.top

Ruby: Dir.pwd
来源：http://vkv.haohaochexian.top

C#:   Directory.GetCurrentDirectory()
来源：http://fat.316326.xyz

[M05] 设置退出码
来源：http://nvk.gogol.net.cn

Py:   sys.exit(1)
来源：http://ork.hcnkem.com

PHP:  exit(1);
来源：http://ihn.chenlongwang.top

JS:   process.exit(1)
来源：http://pbl.hesvh.cn

TS:   process.exit(1)
来源：http://cow.zhijiandao.cn

Java: System.exit(1)
来源：http://bwi.yj20258888.top

Go:   os.Exit(1)
来源：http://yxo.jqgufenzy.top

Ruby: exit 1
来源：http://kpc.jyoumei.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ooj.andypj.xyz

[M06] 向标准错误输出
来源：http://mvv.yueranfly.top

Py:   print("err", file=sys.stderr)
来源：http://uwf.jinqigufen.top

PHP:  fwrite(STDERR, "err\n");
来源：http://nzq.ivvv.top

JS:   console.error("err")
来源：http://gix.shanyushiyangtech.top

TS:   console.error("err")
来源：http://txy.zycfv.cn

Java: System.err.println("err")
来源：http://jxy.guowangkeji.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://cjh.cheryme.top

Ruby: warn "err"
来源：http://eef.zhengqikj.top

C#:   Console.Error.WriteLine("err")
来源：http://arm.316326.xyz

[M07] 判断是否为主入口
来源：http://lpc.yonumen.top

Py:   if __name__ == "__main__":
来源：http://rkc.zdbjq.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://pek.jinqigufen.top

JS:   require.main === module
来源：http://flm.9152youxi.cn

TS:   require.main === module
来源：http://bxd.sjlbkw.cn

Java: public static void main(String[] args)
来源：http://jxb.yuanzhike.top

Go:   func main()
来源：http://qxc.xuanzx.com

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ubc.bbcook.cn

C#:   static void Main(string[] args)
来源：http://axf.haohaochexian.top

[M08] 获取系统与运行时信息
来源：http://cfv.yuanzhike.top

Py:   platform.system();  platform.python_version()
来源：http://icx.hammf.cn

PHP:  PHP_OS;  phpversion();
来源：http://wqa.cashguo.top

JS:   process.platform;  process.version
来源：http://cdc.feifeiyinyue.top

TS:   process.platform;  process.version
来源：http://ass.svipenyu.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://yfa.tarul.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://nmi.ybcxt.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://bme.yuanzhike.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://bmn.haohaochexian.top

================================================================================
来源：http://naq.mhx1999.top

N. 数据结构与算法
来源：http://uxb.zdbjq.cn

================================================================================
来源：http://oih.xuetiantiany.cn


<!-- 参考信息 -->