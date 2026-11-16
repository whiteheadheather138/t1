代发 wailian999

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://lpq.hcnkem.com

JS:   new Date();  Date.now()
来源：http://cvu.316326.xyz

TS:   new Date();  Date.now()
来源：http://aey.yuanzhike.top

Java: LocalDateTime.now();  Instant.now()
来源：http://vnc.jinqigfzy.top

Go:   time.Now()
来源：http://aae.tianlin.xyz

Ruby: Time.now
来源：http://kbg.nanxinkj.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://iov.52xcode.cn

[J02] 格式化输出
来源：http://dnd.gzhubu.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://gmv.dashuyun.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://eaj.gotoacloud.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://udo.fanxiaobao.xyz

TS:   d.toISOString()
来源：http://ytn.zhongyouzk.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://dez.yangfankeji.com

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://toz.xziqi.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://jik.tanke756.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ddv.kuanghao11.cn

[J03] 字符串解析为日期
来源：http://wsx.xziqi.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://zqk.zhengqikj.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://csc.yongpay.top

JS:   new Date("2024-01-02")
来源：http://ocf.yj202588.top

TS:   new Date("2024-01-02")
来源：http://yvz.bjfxy.top

Java: LocalDate.parse("2024-01-02")
来源：http://bem.jiagoushi.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://avy.ehwqpu.com

Ruby: Date.parse("2024-01-02")
来源：http://wop.zycfv.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://pvq.fktsv.cn

[J04] 时间戳与日期互转
来源：http://nwy.chenzaomai.com

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://lyl.guannengcc.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hyb.cashguo.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://naa.zhaomingkeji.xyz

TS:   Math.floor(Date.now() / 1000)
来源：http://aon.redwolf501.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ufw.uphjek.com

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://rea.wangdashe.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://wsp.kuanghao11.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://czp.chenjidiqi.icu

[J05] 时间加减（加 7 天）
来源：http://dzv.ydjk.org.cn

Py:   now + timedelta(days=7)
来源：http://lcr.dashuyun.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://knp.ppjwa.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://uyr.gotoacloud.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://wtv.sjlbkw.cn

Java: LocalDate.now().plusDays(7)
来源：http://hxz.sxryk.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://zpz.hongshengwenyu.top

Ruby: Time.now + 7 * 86400
来源：http://wei.hnqzz.top

C#:   DateTime.Now.AddDays(7)
来源：http://dtk.ybcxt.top

[J06] 计算两时间之差
来源：http://clb.jinyuanbaomall.cn

Py:   (end - start).total_seconds()
来源：http://rns.pengpengdd.cyou

PHP:  $end->diff($start)->days;
来源：http://msq.wangshuangyany.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://aes.hnxiangtu.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://onk.jinyuanbaomall.cn

Java: Duration.between(start, end).toSeconds()
来源：http://wml.sxryk.cn

Go:   end.Sub(start).Hours()
来源：http://erf.bbcook.cn

Ruby: end - start                 # 返回秒数
来源：http://kbj.hfpthk.cn

C#:   (end - start).TotalSeconds
来源：http://afg.shanyushiyangkeji.top

[J07] 比较两个日期
来源：http://nrm.shanyushiyangtech.top

Py:   d1 < d2;  d1 == d2
来源：http://zfg.9152youxi.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://rpp.sjlbkw.cn

JS:   d1.getTime() < d2.getTime()
来源：http://chw.aizwys.cn

TS:   d1.getTime() < d2.getTime()
来源：http://gzn.ppjwa.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://qoh.tian-w.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://gtn.yfazqb.com

Ruby: d1 < d2;  d1 == d2
来源：http://ymx.jyoumei.cn

C#:   d1 < d2;  d1 == d2
来源：http://tcq.yj20258888.top

[J08] 提取年月日与星期
来源：http://byl.snrcjt.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://noh.andypj.xyz

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://zwh.fktsv.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://xcg.guannengcc.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://tdm.fengsongda.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://pvy.shzxlz.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://gim.sysykeji.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://dgs.zhengqikj.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://mmg.xuanzx.com

[J09] 时区处理
来源：http://zqb.jqgfzy.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ivl.aibaodan.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://xiv.epnwcf.com

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://brv.chenlongwang.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://lpg.svipenyu.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://lwb.haohaochexian.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://klf.guannengcc.top

Ruby: Time.now.getlocal("+08:00")
来源：http://lib.fzhhl.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://efh.gzhubu.top

[J10] 取今天 / 本月第一天
来源：http://fth.snrcjt.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://fhz.hesvh.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://jhh.zhengqikj.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://les.nwbrower.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://qtf.uphjek.com

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://plx.xuetiantiany.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://vyy.sufxvd.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://eby.yuanzhike.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ole.xingfuxueyuan.xyz

================================================================================
来源：http://yxy.chenlongwang.top

K. JSON 与序列化
来源：http://aeb.xylfe.cn

================================================================================
来源：http://xxw.cdnleiting.top

[K01] 对象转 JSON 字符串
来源：http://bbl.shzxlz.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://cgn.havefunace.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://lie.316326.xyz

JS:   JSON.stringify(obj)
来源：http://otj.xuetiantiany.cn

TS:   JSON.stringify(obj)
来源：http://bdo.guowangkeji.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://laj.bjfxy.top

Go:   json.Marshal(obj)
来源：http://rmj.shangyingyoupin.top

Ruby: obj.to_json                                     // require "json"
来源：http://ktc.9152youxi.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://bdq.uphjek.com

[K02] JSON 字符串转对象
来源：http://bzv.zdqjudy.top

Py:   json.loads(s)
来源：http://xim.aibaodan.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://dbz.zycfv.cn

JS:   JSON.parse(s)
来源：http://glp.hfpthk.cn

TS:   JSON.parse(s)
来源：http://ppr.tanke756.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://qwu.fengsongda.top

Go:   json.Unmarshal(data, &v)
来源：http://bxz.vehdjk.com

Ruby: JSON.parse(s)
来源：http://qiy.birdmap.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://fog.zhixingplan.top

[K03] JSON 美化输出（带缩进）
来源：http://zno.316326.xyz

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://xaz.nwbrower.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://lbv.ivvv.top

JS:   JSON.stringify(obj, null, 2)
来源：http://huq.nanxuanxn.top

TS:   JSON.stringify(obj, null, 2)
来源：http://tsx.havefunace.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://xbr.wangshuangyany.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://bqz.jyoumei.cn

Ruby: JSON.pretty_generate(obj)
来源：http://huq.dashuyun.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://asg.nwbrower.top

[K04] 读取 JSON 文件
来源：http://don.daxiang520.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://owi.yj202588.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://kyc.ydjk.org.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://tsj.zdqjudy.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://zwi.wangshuangyany.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://pxq.jlsjyb.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://zgb.zhoulong.xyz

Ruby: JSON.parse(File.read("a.json"))
来源：http://pro.hcnkem.com

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wet.sjlbkw.cn

[K05] 深拷贝对象
来源：http://cvw.meibo888.top

Py:   copy.deepcopy(obj)
来源：http://bef.yongpay.top

PHP:  unserialize(serialize($obj));
来源：http://nur.cashguo.top

JS:   structuredClone(obj)
来源：http://qac.birdmap.top

TS:   structuredClone(obj)
来源：http://dat.yj20258888.top

Java: // 手写拷贝构造，或序列化往返
来源：http://exy.hysaishi.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://qmn.yj20258888.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://jzt.birdmap.top

C#:   // 序列化往返，或自定义 Clone
来源：http://haq.cheryme.top

[K06] 解析 URL 查询串
来源：http://zhq.snrcjt.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://gvy.xuetiantiany.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://yiz.gaohongyu789.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mjc.gaohongyu789.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://yxq.hammf.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://bdv.nanxuanxn.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://ixk.yongpay.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://eme.cqqwz.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://sfg.hnqzz.top

[K07] 进制转换
来源：http://twb.jlsjyb.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://sco.yj20258888.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ola.guannengcc.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://fgm.andypj.xyz

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://let.52xcode.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://umq.jqgfzy.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ukr.guowangkeji.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://xtn.hywenlv.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://mom.yanxiufei.cn

[K08] 二进制序列化（非 JSON）
来源：http://ikv.zhengqikj.top

Py:   pickle.dumps(obj)
来源：http://oet.sysykeji.top

PHP:  serialize($obj);  unserialize($s);
来源：http://lix.hongshengwenyu.top

JS:   v8.serialize(obj)        // Node
来源：http://bta.cucudq.cn

TS:   v8.serialize(obj)        // Node
来源：http://lup.hongshengwenyu.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://kfa.shzxlz.cn

Go:   encoding/gob
来源：http://plb.pengpengdd.cyou

Ruby: Marshal.dump(obj)
来源：http://zzt.dianchejie.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://vbs.sufxvd.cn

================================================================================
来源：http://pyr.daria6918.cn

L. 网络请求
来源：http://kvm.yvedp.cn

================================================================================
来源：http://xum.birdmap.top

[L01] 发送 GET 请求
来源：http://fhi.yueranfly.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://rng.ctjpmb.com

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://bvk.daxiang520.top

JS:   await fetch(url)
来源：http://ayk.sweek.top

TS:   await fetch(url)
来源：http://lbi.shangyingyoupin.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://nyy.feifeiyinyue.top

Go:   resp, err := http.Get(url)
来源：http://uif.yfazqb.com

Ruby: Net::HTTP.get(URI(url))
来源：http://ukr.ydjk.org.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wup.xziqi.cn

[L02] 发送 POST JSON
来源：http://amj.zdbjq.cn

Py:   requests.post(url, json={"a": 1})
来源：http://egb.jianghu66.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://meh.zhongyouzk.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://nfe.smart0.xyz

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://aoh.yuanzhike.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ylc.aibaodan.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://qam.daria6918.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://kjy.chenzaomai.com

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://isb.ehwqpu.com

[L03] 设置自定义请求头
来源：http://iya.jinghuilouyu.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://xvt.meibo888.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://tbw.hfpthk.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://cdy.shanyushiyangtech.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://bai.uphjek.com

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://fod.hesvh.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://bsr.fanxiaobao.xyz

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://fkn.vqdsnc.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://pfh.yfazqb.com

[L04] 设置超时
来源：http://kop.dianchejie.cn

Py:   requests.get(url, timeout=5)
来源：http://ogp.xinyue.icu

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://qel.gaohongyu789.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://shw.sjlbkw.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ryf.dianchejie.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hhi.jinqigfzy.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://dsg.ywan-chungtsiang.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://gbx.mhx1999.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mdl.hysaishi.cn

[L05] 上传文件（multipart）
来源：http://mui.ctjpmb.com

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mom.feifeiyinyue.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://dvf.ydzc1.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://dqp.wangshuangyany.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://pak.sysykeji.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://xnb.ydjk.org.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://eum.shanyushiyangtech.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://xcs.ywan-chungtsiang.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://azj.havefunace.top

[L06] 解析响应为 JSON
来源：http://tbx.iojbl.cn

Py:   resp.json()
来源：http://zso.jlsjyb.cn

PHP:  json_decode($body, true);
来源：http://won.yj20258.top

JS:   await resp.json()
来源：http://hqt.316326.xyz

TS:   await resp.json()
来源：http://lcr.jinyuanbaomall.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://dii.dianchejie.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://kzs.yj20258.top

Ruby: JSON.parse(resp.body)
来源：http://glf.0kj1m.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mjm.kuanghao11.cn

[L07] 处理 HTTP 状态码
来源：http://qqb.xziqi.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ffc.wangshuangyany.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ail.0kj1m.cn

JS:   resp.ok;  resp.status
来源：http://nir.jinqigfzy.top

TS:   resp.ok;  resp.status
来源：http://xlf.zycfv.cn

Java: resp.statusCode()
来源：http://brf.nwbrower.top

Go:   resp.StatusCode
来源：http://euf.gogol.net.cn

Ruby: resp.code.to_i
来源：http://moh.sysykeji.top

C#:   (int)resp.StatusCode
来源：http://sdf.zhoulong.xyz

[L08] 并发请求多个地址
来源：http://hyg.guannengcc.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://fle.yuanzhike.top

PHP:  curl_multi_init() 系列
来源：http://edm.ydzc1.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://xds.vehdjk.com

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://rfh.tarul.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ryq.dianchejie.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://zxj.cashguo.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://lze.jinqigufen.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ieg.0kj1m.cn

================================================================================
来源：http://mkj.vqdsnc.cn

M. 命令行 / 进程 / 环境
来源：http://skg.jyoumei.cn

================================================================================
来源：http://wfg.cheryme.top

[M01] 读取命令行参数
来源：http://qqe.jyoumei.cn

Py:   sys.argv[1:]
来源：http://obi.jiagoushi.top

PHP:  $argv;  $argc;
来源：http://wcr.svipenyu.cn

JS:   process.argv.slice(2)
来源：http://peq.hongshengwenyu.top

TS:   process.argv.slice(2)
来源：http://ftw.yuxming.cn

Java: args 数组（main 方法参数）
来源：http://iwf.jlsjyb.cn

Go:   os.Args[1:]
来源：http://abc.xinyue.icu

Ruby: ARGV
来源：http://gaq.yueranfly.top

C#:   args 数组（Main 方法参数）
来源：http://xac.xinyue.icu

[M02] 读取环境变量
来源：http://ebx.xuetiantiany.cn

Py:   os.environ.get("HOME")
来源：http://kyo.hnqzz.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://dui.daxiang520.top

JS:   process.env.HOME
来源：http://ymf.gaohongyu789.top

TS:   process.env.HOME
来源：http://vnl.tian-w.cn

Java: System.getenv("HOME")
来源：http://bzp.ctjpmb.com

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://faj.svipenyu.cn

Ruby: ENV["HOME"]
来源：http://uxn.9152youxi.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://pjr.wangshuangyany.cn

[M03] 执行外部命令
来源：http://urk.uphjek.com

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ebc.nanxinkj.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://xky.cqqwz.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://bqw.xingfuxueyuan.xyz

TS:   child_process.execSync("ls -l").toString()
来源：http://mbp.jinghuilouyu.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://cgv.nwbrower.top

Go:   exec.Command("ls", "-l").Output()
来源：http://cwa.yvedp.cn

Ruby: system("ls -l");  `ls -l`
来源：http://mpm.chenlongwang.top

C#:   Process.Start("ls", "-l");
来源：http://cfr.pycfn.com

[M04] 获取当前工作目录
来源：http://qia.daxiang520.top

Py:   os.getcwd()
来源：http://bna.yfazqb.com

PHP:  getcwd();
来源：http://jpa.0kj1m.cn

JS:   process.cwd()
来源：http://qci.ybcxt.top

TS:   process.cwd()
来源：http://hrf.hammf.cn

Java: Path.of("").toAbsolutePath()
来源：http://uub.shangyingyoupin.top

Go:   os.Getwd()
来源：http://iah.wangshuangyany.cn

Ruby: Dir.pwd
来源：http://ouq.shuidangran.top

C#:   Directory.GetCurrentDirectory()
来源：http://tti.yonumen.top

[M05] 设置退出码
来源：http://dyu.snrcjt.cn

Py:   sys.exit(1)
来源：http://xvn.sxryk.cn

PHP:  exit(1);
来源：http://hic.yonumen.top

JS:   process.exit(1)
来源：http://oth.52xcode.cn

TS:   process.exit(1)
来源：http://srs.tian-w.cn

Java: System.exit(1)
来源：http://ngl.jqgfzy.top

Go:   os.Exit(1)
来源：http://gsb.fzhhl.top

Ruby: exit 1
来源：http://ntp.jinqigufen.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://cwu.jiagoushi.top

[M06] 向标准错误输出
来源：http://qkv.hywenlv.cn

Py:   print("err", file=sys.stderr)
来源：http://oks.andypj.xyz

PHP:  fwrite(STDERR, "err\n");
来源：http://xbr.bbcook.cn

JS:   console.error("err")
来源：http://asz.ppjwa.cn

TS:   console.error("err")
来源：http://lcg.chenzaomai.com

Java: System.err.println("err")
来源：http://mei.wangdashe.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ejj.hfpthk.cn

Ruby: warn "err"
来源：http://keu.fzhhl.top

C#:   Console.Error.WriteLine("err")
来源：http://kxw.ppjwa.cn

[M07] 判断是否为主入口
来源：http://okv.wangshuangyany.cn

Py:   if __name__ == "__main__":
来源：http://mmx.jyoumei.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hbx.andypj.xyz

JS:   require.main === module
来源：http://yla.bbcook.cn

TS:   require.main === module
来源：http://kwe.aibaodan.cn


<!-- 参考信息 -->