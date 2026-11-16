代发 wailian999

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://cpt.zhongyouzk.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ewb.uphjek.com

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://gvd.tian-w.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://nba.tanke756.top

[J03] 字符串解析为日期
来源：http://gqd.52xcode.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://uvv.ywan-chungtsiang.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://gur.shanyushiyangtech.top

JS:   new Date("2024-01-02")
来源：http://mkr.chenjidiqi.icu

TS:   new Date("2024-01-02")
来源：http://zzi.pycfn.com

Java: LocalDate.parse("2024-01-02")
来源：http://oav.aibaodan.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://grm.gaohongyu789.top

Ruby: Date.parse("2024-01-02")
来源：http://pvi.daria6918.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://wdc.meibo888.top

[J04] 时间戳与日期互转
来源：http://bfc.nanxuanxn.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://afp.yuxming.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://fvq.chenzaomai.com

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://rqv.ctjpmb.com

TS:   Math.floor(Date.now() / 1000)
来源：http://qqd.xinyue.icu

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://dcx.cashguo.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://sxp.tian-w.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://pzp.fzhhl.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://bjl.9152youxi.cn

[J05] 时间加减（加 7 天）
来源：http://lur.hnqzz.top

Py:   now + timedelta(days=7)
来源：http://ssm.ivvv.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://ani.hywenlv.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://lds.wangshuangyany.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://iem.xuanzx.com

Java: LocalDate.now().plusDays(7)
来源：http://ibi.meibo888.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://bsi.zdbjq.cn

Ruby: Time.now + 7 * 86400
来源：http://roy.jqgfzy.top

C#:   DateTime.Now.AddDays(7)
来源：http://sih.jinqigufen.top

[J06] 计算两时间之差
来源：http://gfn.nanxinkj.top

Py:   (end - start).total_seconds()
来源：http://vzn.snrcjt.cn

PHP:  $end->diff($start)->days;
来源：http://wfn.yuxming.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://pgh.fzhhl.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://otd.ywan-chungtsiang.top

Java: Duration.between(start, end).toSeconds()
来源：http://uvh.xziqi.cn

Go:   end.Sub(start).Hours()
来源：http://szk.hnxiangtu.top

Ruby: end - start                 # 返回秒数
来源：http://oep.zhengqikj.top

C#:   (end - start).TotalSeconds
来源：http://nut.shanyushiyangkeji.top

[J07] 比较两个日期
来源：http://jtf.zhiwuduotai.top

Py:   d1 < d2;  d1 == d2
来源：http://sbo.havefunace.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://fhr.yuxming.cn

JS:   d1.getTime() < d2.getTime()
来源：http://klm.jinqigfzy.top

TS:   d1.getTime() < d2.getTime()
来源：http://moc.feifeiyinyue.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://yhq.yj20258888.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://fbg.fehbvm.com

Ruby: d1 < d2;  d1 == d2
来源：http://omp.yangfankeji.com

C#:   d1 < d2;  d1 == d2
来源：http://rlw.chenlongwang.top

[J08] 提取年月日与星期
来源：http://wqk.ywan-chungtsiang.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ttu.redwolf501.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://tfj.xuetiantiany.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://gss.aibaodan.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://oeo.jianghu66.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://sqw.xziqi.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://rkq.cheryme.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://rra.gotoacloud.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://giv.redwolf501.top

[J09] 时区处理
来源：http://gpm.zycfv.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://uxw.yj20258.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://zfs.xuetiantiany.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://cqg.hammf.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ztr.shanyushiyangkeji.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://wja.ehwqpu.com

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://roh.ppjwa.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://ypl.yfazqb.com

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://lei.svipenyu.cn

[J10] 取今天 / 本月第一天
来源：http://drj.feifeiyinyue.top

Py:   date.today();  date.today().replace(day=1)
来源：http://ysh.haohaochexian.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://tjy.gogol.net.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://dec.yj20258888.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://dtp.hnqzz.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://mtn.vehdjk.com

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://pcn.ivvv.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ufk.hesvh.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://cwy.jqgufenzy.top

================================================================================
来源：http://fwn.vqdsnc.cn

K. JSON 与序列化
来源：http://qus.xuetiantiany.cn

================================================================================
来源：http://avo.yongpay.top

[K01] 对象转 JSON 字符串
来源：http://gfk.nwbrower.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ycl.0kj1m.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ban.aizwys.cn

JS:   JSON.stringify(obj)
来源：http://caw.jlsjyb.cn

TS:   JSON.stringify(obj)
来源：http://trl.sjlbkw.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://flb.ydjk.org.cn

Go:   json.Marshal(obj)
来源：http://qkx.fanxiaobao.xyz

Ruby: obj.to_json                                     // require "json"
来源：http://ffl.shanyushiyangtech.top

C#:   JsonSerializer.Serialize(obj)
来源：http://qoh.mhx1999.top

[K02] JSON 字符串转对象
来源：http://bdq.fzhhl.top

Py:   json.loads(s)
来源：http://jsh.gaohongyu789.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://irr.9152youxi.cn

JS:   JSON.parse(s)
来源：http://ckr.havefunace.top

TS:   JSON.parse(s)
来源：http://tkr.jyoumei.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://lbe.aibaodan.cn

Go:   json.Unmarshal(data, &v)
来源：http://uzu.hywenlv.cn

Ruby: JSON.parse(s)
来源：http://jjb.yvedp.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://rsl.yfazqb.com

[K03] JSON 美化输出（带缩进）
来源：http://jjn.havefunace.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://yny.zycfv.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://pmu.0kj1m.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://gwp.yuxming.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://okc.nanxinkj.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wdv.cqqwz.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ila.vqdsnc.cn

Ruby: JSON.pretty_generate(obj)
来源：http://ecz.xuetiantiany.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://qnb.0kj1m.cn

[K04] 读取 JSON 文件
来源：http://vqc.wangshuangyany.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://fmk.daxiang520.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://gqu.daxiang520.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://kgg.hesvh.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://bqy.ctjpmb.com

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://vsx.zhengqikj.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://aso.jinqigfzy.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://lbt.meibo888.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://rwu.hesvh.cn

[K05] 深拷贝对象
来源：http://erg.feifeiyinyue.top

Py:   copy.deepcopy(obj)
来源：http://xix.jinqigufen.top

PHP:  unserialize(serialize($obj));
来源：http://wbk.hammf.cn

JS:   structuredClone(obj)
来源：http://zqc.aizwys.cn

TS:   structuredClone(obj)
来源：http://cwb.snrcjt.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://irb.andypj.xyz

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://oiw.zhongyouzk.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://zcd.yongpay.top

C#:   // 序列化往返，或自定义 Clone
来源：http://ubq.jianghu66.top

[K06] 解析 URL 查询串
来源：http://nlg.jinyuanbaomall.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://esc.uphjek.com

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ttr.ivvv.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://bhq.zhoulong.xyz

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://iwp.fktsv.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://anc.fengsongda.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://ale.vqdsnc.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://aaz.cucudq.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://etu.cdnleiting.top

[K07] 进制转换
来源：http://rly.xylfe.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://epg.tanke756.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wtg.chenzaomai.com

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://lur.fktsv.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://veg.jiagoushi.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://jlx.zhoulong.xyz

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://bkx.zhijiandao.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://slo.sufxvd.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://any.yanxiufei.cn

[K08] 二进制序列化（非 JSON）
来源：http://xhw.daria6918.cn

Py:   pickle.dumps(obj)
来源：http://xax.hammf.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://bgd.chenjidiqi.icu

JS:   v8.serialize(obj)        // Node
来源：http://xjx.zhoulong.xyz

TS:   v8.serialize(obj)        // Node
来源：http://bdd.shzxlz.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://byk.haohaochexian.top

Go:   encoding/gob
来源：http://fps.jyoumei.cn

Ruby: Marshal.dump(obj)
来源：http://kjq.hysaishi.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://nig.uphjek.com

================================================================================
来源：http://ehs.yanxiufei.cn

L. 网络请求
来源：http://tom.xylfe.cn

================================================================================
来源：http://uyt.c1oappe.top

[L01] 发送 GET 请求
来源：http://rxt.cheryme.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://nxx.hnxiangtu.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://npw.tanke756.top

JS:   await fetch(url)
来源：http://lej.jinqigfzy.top

TS:   await fetch(url)
来源：http://amp.zhoulong.xyz

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://tqd.zhongyouzk.top

Go:   resp, err := http.Get(url)
来源：http://pax.hammf.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://igj.sysykeji.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://yca.shuidangran.top

[L02] 发送 POST JSON
来源：http://ton.jiagoushi.top

Py:   requests.post(url, json={"a": 1})
来源：http://yoe.zdqjudy.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://dgm.hfpthk.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wvt.ehwqpu.com

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://inl.bbcook.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://rwp.dianchejie.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://aot.9152youxi.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ats.andypj.xyz

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://thu.zhongyouzk.top

[L03] 设置自定义请求头
来源：http://pid.52xcode.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://juu.cucudq.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://unv.yuanzhike.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://nbu.sufxvd.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blr.gogol.net.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://uag.fehbvm.com

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hmd.yongpay.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://kkr.jyoumei.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://trr.shanyushiyangtech.top

[L04] 设置超时
来源：http://fjd.shuidangran.top

Py:   requests.get(url, timeout=5)
来源：http://khw.cheryme.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://njh.jinqigufen.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://cre.yangfankeji.com

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://yry.pengpengdd.cyou

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://znq.wangdashe.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://jgx.yangfankeji.com

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://xvi.snrcjt.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://gqm.wangdashe.top

[L05] 上传文件（multipart）
来源：http://zhy.cqqwz.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://pxz.hfpthk.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://xmv.9152youxi.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wlm.cqqwz.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://yft.jinyuanbaomall.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ltg.xinyue.icu

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hdr.yj20258.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ewi.jiagoushi.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://rda.hfpthk.cn

[L06] 解析响应为 JSON
来源：http://soe.shuidangran.top

Py:   resp.json()
来源：http://ndh.xinyue.icu

PHP:  json_decode($body, true);
来源：http://dns.hesvh.cn

JS:   await resp.json()
来源：http://kyn.9152youxi.cn

TS:   await resp.json()
来源：http://qua.zdqjudy.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://rac.havefunace.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://maj.nwbrower.top

Ruby: JSON.parse(resp.body)
来源：http://rtd.xuetiantiany.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://rxt.jiagoushi.top

[L07] 处理 HTTP 状态码
来源：http://qra.xuetiantiany.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://arw.havefunace.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://nqd.bjfxy.top

JS:   resp.ok;  resp.status
来源：http://els.hammf.cn

TS:   resp.ok;  resp.status
来源：http://tga.gaohongyu789.top

Java: resp.statusCode()
来源：http://pxx.chenlongwang.top

Go:   resp.StatusCode
来源：http://qxw.jqgufenzy.top

Ruby: resp.code.to_i
来源：http://vlj.jlsjyb.cn

C#:   (int)resp.StatusCode
来源：http://iys.ivvv.top

[L08] 并发请求多个地址
来源：http://uqz.zhixingplan.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hgc.jinqigufen.top

PHP:  curl_multi_init() 系列
来源：http://ixa.haohaochexian.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://esc.gotoacloud.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://rpn.xuetiantiany.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://dya.meibo888.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://cbb.yj202588.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://zfi.xziqi.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://xhd.pengpengdd.cyou

================================================================================
来源：http://bxp.zhongyouzk.top

M. 命令行 / 进程 / 环境
来源：http://yyx.chenjidiqi.icu

================================================================================
来源：http://sgg.bbcook.cn

[M01] 读取命令行参数
来源：http://jrt.pengpengdd.cyou

Py:   sys.argv[1:]
来源：http://vmj.jinghuilouyu.cn

PHP:  $argv;  $argc;
来源：http://sue.9152youxi.cn

JS:   process.argv.slice(2)
来源：http://exx.gzhubu.top

TS:   process.argv.slice(2)
来源：http://uls.birdmap.top

Java: args 数组（main 方法参数）
来源：http://qph.andypj.xyz

Go:   os.Args[1:]
来源：http://jxg.ppjwa.cn

Ruby: ARGV
来源：http://yfp.sjlbkw.cn

C#:   args 数组（Main 方法参数）
来源：http://mbt.fanxiaobao.xyz

[M02] 读取环境变量
来源：http://jny.zhixingplan.top

Py:   os.environ.get("HOME")
来源：http://gul.xinyue.icu

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://see.jinyuanbaomall.cn

JS:   process.env.HOME
来源：http://smm.hnqzz.top

TS:   process.env.HOME
来源：http://pup.shuidangran.top

Java: System.getenv("HOME")
来源：http://pwy.jinyuanbaomall.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ror.xziqi.cn

Ruby: ENV["HOME"]
来源：http://weq.zhoulong.xyz

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://tin.cdnleiting.top

[M03] 执行外部命令
来源：http://ogj.hnqzz.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mkc.hnxiangtu.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://qwo.hywenlv.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://koz.9152youxi.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://azf.cdnleiting.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://vlt.guowangkeji.top

Go:   exec.Command("ls", "-l").Output()
来源：http://qtd.ydjk.org.cn

Ruby: system("ls -l");  `ls -l`
来源：http://sxk.xinyue.icu

C#:   Process.Start("ls", "-l");
来源：http://ipr.0kj1m.cn

[M04] 获取当前工作目录
来源：http://rbt.chenlongwang.top

Py:   os.getcwd()
来源：http://dmc.sysykeji.top

PHP:  getcwd();
来源：http://dgr.ivvv.top

JS:   process.cwd()
来源：http://fwd.aibaodan.cn

TS:   process.cwd()
来源：http://hmh.0kj1m.cn

Java: Path.of("").toAbsolutePath()
来源：http://mlh.yangfankeji.com

Go:   os.Getwd()
来源：http://wgo.c1oappe.top

Ruby: Dir.pwd
来源：http://jpg.52xcode.cn

C#:   Directory.GetCurrentDirectory()
来源：http://xkg.bjfxy.top

[M05] 设置退出码
来源：http://awy.yj20258888.top

Py:   sys.exit(1)
来源：http://mjg.sweek.top

PHP:  exit(1);
来源：http://yjv.yuanzhike.top

JS:   process.exit(1)
来源：http://tpp.jiagoushi.top

TS:   process.exit(1)
来源：http://brf.mhx1999.top

Java: System.exit(1)
来源：http://pvi.wangshuangyany.cn

Go:   os.Exit(1)
来源：http://oqj.sysykeji.top

Ruby: exit 1
来源：http://fmj.svipenyu.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wks.havefunace.top

[M06] 向标准错误输出
来源：http://sye.cashguo.top

Py:   print("err", file=sys.stderr)
来源：http://zkt.fengsongda.top

PHP:  fwrite(STDERR, "err\n");
来源：http://rdz.zdbjq.cn

JS:   console.error("err")
来源：http://toh.ywan-chungtsiang.top

TS:   console.error("err")
来源：http://ypf.bjfxy.top

Java: System.err.println("err")
来源：http://ukj.jinyuanbaomall.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://fho.vehdjk.com

Ruby: warn "err"
来源：http://iak.chenzaomai.com

C#:   Console.Error.WriteLine("err")
来源：http://liv.hongshengwenyu.top

[M07] 判断是否为主入口
来源：http://wdj.fktsv.cn

Py:   if __name__ == "__main__":
来源：http://otv.xingfuxueyuan.xyz

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://avv.zhaomingkeji.xyz

JS:   require.main === module
来源：http://ssp.aibaodan.cn

TS:   require.main === module
来源：http://ptw.shzxlz.cn

Java: public static void main(String[] args)
来源：http://pgr.birdmap.top

Go:   func main()
来源：http://ida.wangdashe.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://htp.jinghuilouyu.cn

C#:   static void Main(string[] args)
来源：http://fyq.zhengqikj.top

[M08] 获取系统与运行时信息
来源：http://fcp.chenzaomai.com

Py:   platform.system();  platform.python_version()
来源：http://bcj.hywenlv.cn

PHP:  PHP_OS;  phpversion();
来源：http://zyz.epnwcf.com

JS:   process.platform;  process.version
来源：http://yod.zdqjudy.top

TS:   process.platform;  process.version
来源：http://cjt.hammf.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://kpy.birdmap.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://rca.yonumen.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://iwb.yanxiufei.cn


<!-- 参考信息 -->