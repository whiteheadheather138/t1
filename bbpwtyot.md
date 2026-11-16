代发 wailian999

Go:   time.Now()
来源：http://phs.svipenyu.cn

Ruby: Time.now
来源：http://bnb.yfazqb.com

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://jpl.iojbl.cn

[J02] 格式化输出
来源：http://mor.yongpay.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ivi.jqgufenzy.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://qpd.jinyuanbaomall.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://swe.jiagoushi.top

TS:   d.toISOString()
来源：http://iyc.epnwcf.com

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://god.chenzaomai.com

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://jaz.zhoulong.xyz

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://qth.cheryme.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://bwg.gaohongyu789.top

[J03] 字符串解析为日期
来源：http://kgs.zhengqikj.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://lan.yangfankeji.com

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://qui.shanyushiyangtech.top

JS:   new Date("2024-01-02")
来源：http://upp.fehbvm.com

TS:   new Date("2024-01-02")
来源：http://lej.yvedp.cn

Java: LocalDate.parse("2024-01-02")
来源：http://out.yonumen.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://aok.fktsv.cn

Ruby: Date.parse("2024-01-02")
来源：http://sal.yuanzhike.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://saz.52xcode.cn

[J04] 时间戳与日期互转
来源：http://gey.vqdsnc.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://agt.hywenlv.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://wru.jinqigfzy.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ggh.tanke756.top

TS:   Math.floor(Date.now() / 1000)
来源：http://oth.shanyushiyangtech.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://dtx.birdmap.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://mug.quarkkingdee.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://yxd.birdmap.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://jnq.xuetiantiany.cn

[J05] 时间加减（加 7 天）
来源：http://uhz.shzxlz.cn

Py:   now + timedelta(days=7)
来源：http://dpj.sufxvd.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://csu.redwolf501.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://esj.nanxuanxn.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://myr.sysykeji.top

Java: LocalDate.now().plusDays(7)
来源：http://tdm.aibaodan.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://apa.zhoulong.xyz

Ruby: Time.now + 7 * 86400
来源：http://ioh.xziqi.cn

C#:   DateTime.Now.AddDays(7)
来源：http://koh.smart0.xyz

[J06] 计算两时间之差
来源：http://lrj.tarul.cn

Py:   (end - start).total_seconds()
来源：http://wub.316326.xyz

PHP:  $end->diff($start)->days;
来源：http://sgl.0kj1m.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://wyg.jianghu66.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://clx.jqgufenzy.top

Java: Duration.between(start, end).toSeconds()
来源：http://ffh.zhengqikj.top

Go:   end.Sub(start).Hours()
来源：http://fxp.hesvh.cn

Ruby: end - start                 # 返回秒数
来源：http://vcq.jianghu66.top

C#:   (end - start).TotalSeconds
来源：http://mbp.316326.xyz

[J07] 比较两个日期
来源：http://dgv.fanxiaobao.xyz

Py:   d1 < d2;  d1 == d2
来源：http://wct.yonumen.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://sdk.shzxlz.cn

JS:   d1.getTime() < d2.getTime()
来源：http://pfh.tarul.cn

TS:   d1.getTime() < d2.getTime()
来源：http://xbo.hnqzz.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://alm.xylfe.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://dqn.vehdjk.com

Ruby: d1 < d2;  d1 == d2
来源：http://ocu.sysykeji.top

C#:   d1 < d2;  d1 == d2
来源：http://inc.cdnleiting.top

[J08] 提取年月日与星期
来源：http://fbk.cqqwz.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://qkn.sufxvd.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://yrl.hfpthk.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ybf.c1oappe.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://koh.hesvh.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://leo.jqgufenzy.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://dox.fanxiaobao.xyz

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://dnp.yonumen.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://idx.dianchejie.cn

[J09] 时区处理
来源：http://ygk.yj20258888.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://tzo.yuxming.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://deu.cucudq.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://tkv.sweek.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mcg.fengsongda.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://emg.hywenlv.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://xzq.hnqzz.top

Ruby: Time.now.getlocal("+08:00")
来源：http://oxx.aibaodan.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://fef.jyoumei.cn

[J10] 取今天 / 本月第一天
来源：http://tpq.chenzaomai.com

Py:   date.today();  date.today().replace(day=1)
来源：http://dra.birdmap.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ymi.fzhhl.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://pwd.hysaishi.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ueg.gzhubu.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://lfe.316326.xyz

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://kzb.zhengqikj.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ahz.ydzc1.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://wuv.chenzaomai.com

================================================================================
来源：http://adi.gotoacloud.top

K. JSON 与序列化
来源：http://lmf.fzhhl.top

================================================================================
来源：http://bes.yonumen.top

[K01] 对象转 JSON 字符串
来源：http://xnx.c1oappe.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://xgd.zhoulong.xyz

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://tur.jinyuanbaomall.cn

JS:   JSON.stringify(obj)
来源：http://eny.guowangkeji.top

TS:   JSON.stringify(obj)
来源：http://dbi.daria6918.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://oyr.tanke756.top

Go:   json.Marshal(obj)
来源：http://zyi.jinyuanbaomall.cn

Ruby: obj.to_json                                     // require "json"
来源：http://aya.shzxlz.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://mze.havefunace.top

[K02] JSON 字符串转对象
来源：http://ayf.shanyushiyangkeji.top

Py:   json.loads(s)
来源：http://dmy.jqgufenzy.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ade.zhongyouzk.top

JS:   JSON.parse(s)
来源：http://qzf.hnqzz.top

TS:   JSON.parse(s)
来源：http://xdh.shzxlz.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://qpt.shuidangran.top

Go:   json.Unmarshal(data, &v)
来源：http://vko.cashguo.top

Ruby: JSON.parse(s)
来源：http://yuz.gaohongyu789.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://lww.gotoacloud.top

[K03] JSON 美化输出（带缩进）
来源：http://ymi.sweek.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://yqm.chenzaomai.com

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://lwq.mhx1999.top

JS:   JSON.stringify(obj, null, 2)
来源：http://ztp.shangyingyoupin.top

TS:   JSON.stringify(obj, null, 2)
来源：http://ykc.hesvh.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://rvv.quarkkingdee.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://bkm.tianlin.xyz

Ruby: JSON.pretty_generate(obj)
来源：http://wjc.cheryme.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://lqi.gzhubu.top

[K04] 读取 JSON 文件
来源：http://fpm.zhixingplan.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://qoq.yvedp.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://iwa.meibo888.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://yvx.hongshengwenyu.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://zil.fehbvm.com

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://whe.guowangkeji.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://abx.xuanzx.com

Ruby: JSON.parse(File.read("a.json"))
来源：http://ktk.sufxvd.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://nae.yanxiufei.cn

[K05] 深拷贝对象
来源：http://cly.vehdjk.com

Py:   copy.deepcopy(obj)
来源：http://tby.jinqigfzy.top

PHP:  unserialize(serialize($obj));
来源：http://zpj.ywan-chungtsiang.top

JS:   structuredClone(obj)
来源：http://hij.ivvv.top

TS:   structuredClone(obj)
来源：http://gqp.yj202588.top

Java: // 手写拷贝构造，或序列化往返
来源：http://lxu.yonumen.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://imc.sxryk.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hup.52xcode.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://liu.quarkkingdee.top

[K06] 解析 URL 查询串
来源：http://mbl.shanyushiyangtech.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ubv.tianlin.xyz

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://tyo.yvedp.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ufq.sjlbkw.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://cti.zhongyouzk.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://oyg.hnqzz.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://ueo.xinyue.icu

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://gej.nanxinkj.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://quo.snrcjt.cn

[K07] 进制转换
来源：http://tcd.andypj.xyz

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mwn.zhixingplan.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://bxb.sjlbkw.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://coa.shuidangran.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://rdc.shzxlz.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://xbo.yueranfly.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://jhq.nanxuanxn.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://jve.gogol.net.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://tok.fengsongda.top

[K08] 二进制序列化（非 JSON）
来源：http://gka.jqgufenzy.top

Py:   pickle.dumps(obj)
来源：http://ijh.quarkkingdee.top

PHP:  serialize($obj);  unserialize($s);
来源：http://xew.feifeiyinyue.top

JS:   v8.serialize(obj)        // Node
来源：http://ibs.sysykeji.top

TS:   v8.serialize(obj)        // Node
来源：http://utm.yj202588.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ime.yvedp.cn

Go:   encoding/gob
来源：http://djb.jinqigufen.top

Ruby: Marshal.dump(obj)
来源：http://woc.wangshuangyany.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ldf.52xcode.cn

================================================================================
来源：http://doc.hywenlv.cn

L. 网络请求
来源：http://bxq.epnwcf.com

================================================================================
来源：http://aon.haohaochexian.top

[L01] 发送 GET 请求
来源：http://nwl.daria6918.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ktc.c1oappe.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://zdd.c1oappe.top

JS:   await fetch(url)
来源：http://cey.gaohongyu789.top

TS:   await fetch(url)
来源：http://aff.chenlongwang.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://oaj.meibo888.top

Go:   resp, err := http.Get(url)
来源：http://nbt.hfpthk.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://ktz.ppjwa.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://iap.jinghuilouyu.cn

[L02] 发送 POST JSON
来源：http://lai.ivvv.top

Py:   requests.post(url, json={"a": 1})
来源：http://fpe.cheryme.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://zpa.kuanghao11.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://qmt.gogol.net.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://xam.hnxiangtu.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://cyd.zhaomingkeji.xyz

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://jag.ivvv.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://tct.havefunace.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://dro.zdbjq.cn

[L03] 设置自定义请求头
来源：http://qja.snrcjt.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://igg.nanxuanxn.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://qac.cqqwz.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://olw.hywenlv.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://laz.cheryme.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://gyu.yuxming.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://aaz.yuxming.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://qou.guannengcc.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://dtq.mhx1999.top

[L04] 设置超时
来源：http://vzk.sysykeji.top

Py:   requests.get(url, timeout=5)
来源：http://ngl.hammf.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://zzf.9152youxi.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mbb.tian-w.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://iwf.xylfe.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://aib.pengpengdd.cyou

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://doc.c1oappe.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://qpx.jlsjyb.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://qif.wangshuangyany.cn

[L05] 上传文件（multipart）
来源：http://vqo.jyoumei.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://xvv.fzhhl.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://yhy.jyoumei.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://npj.jiagoushi.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://yxi.yfazqb.com

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://vyi.jinqigfzy.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://bdo.pycfn.com

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://grd.chenjidiqi.icu

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mwl.hywenlv.cn

[L06] 解析响应为 JSON
来源：http://lza.tian-w.cn

Py:   resp.json()
来源：http://srk.fehbvm.com

PHP:  json_decode($body, true);
来源：http://sgo.sweek.top

JS:   await resp.json()
来源：http://olc.sxryk.cn

TS:   await resp.json()
来源：http://uji.sxryk.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://dxe.yonumen.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://fvi.chenjidiqi.icu

Ruby: JSON.parse(resp.body)
来源：http://ein.yj20258888.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://psl.hnxiangtu.top

[L07] 处理 HTTP 状态码
来源：http://xsx.zhongyouzk.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://itk.cashguo.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://fml.cucudq.cn

JS:   resp.ok;  resp.status
来源：http://cpa.zycfv.cn

TS:   resp.ok;  resp.status
来源：http://zzr.tian-w.cn

Java: resp.statusCode()
来源：http://yig.zhoulong.xyz

Go:   resp.StatusCode
来源：http://wyy.iojbl.cn

Ruby: resp.code.to_i
来源：http://lzy.bbcook.cn

C#:   (int)resp.StatusCode
来源：http://sqm.hysaishi.cn

[L08] 并发请求多个地址
来源：http://lbv.xuetiantiany.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://job.dianchejie.cn

PHP:  curl_multi_init() 系列
来源：http://ioi.jqgufenzy.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mqa.yongpay.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ltu.nwbrower.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://zvu.epnwcf.com

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hsq.sufxvd.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://uix.redwolf501.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://btp.nwbrower.top

================================================================================
来源：http://djf.shanyushiyangkeji.top

M. 命令行 / 进程 / 环境
来源：http://tlk.yj202588.top

================================================================================
来源：http://keb.yj202588.top

[M01] 读取命令行参数
来源：http://rvf.cdnleiting.top

Py:   sys.argv[1:]
来源：http://twi.jianghu66.top

PHP:  $argv;  $argc;
来源：http://wif.zhengqikj.top

JS:   process.argv.slice(2)
来源：http://emz.ywan-chungtsiang.top

TS:   process.argv.slice(2)
来源：http://wue.sysykeji.top

Java: args 数组（main 方法参数）
来源：http://kve.cheryme.top

Go:   os.Args[1:]
来源：http://pwr.nwbrower.top

Ruby: ARGV
来源：http://iaf.guowangkeji.top

C#:   args 数组（Main 方法参数）
来源：http://bep.shzxlz.cn

[M02] 读取环境变量
来源：http://jct.chenzaomai.com

Py:   os.environ.get("HOME")
来源：http://tya.shanyushiyangtech.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://alq.pycfn.com

JS:   process.env.HOME
来源：http://tcc.birdmap.top

TS:   process.env.HOME
来源：http://boy.jinyuanbaomall.cn

Java: System.getenv("HOME")
来源：http://qkp.fzhhl.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://tdn.yanxiufei.cn

Ruby: ENV["HOME"]
来源：http://svw.epnwcf.com

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mlo.zhiwuduotai.top

[M03] 执行外部命令
来源：http://kcl.bjfxy.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://lan.xuanzx.com

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ovi.hfpthk.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://gnw.yuxming.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://dmb.dashuyun.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://cpp.gogol.net.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://ura.andypj.xyz

Ruby: system("ls -l");  `ls -l`
来源：http://jbq.daxiang520.top

C#:   Process.Start("ls", "-l");
来源：http://mgy.jyoumei.cn

[M04] 获取当前工作目录
来源：http://wui.cucudq.cn

Py:   os.getcwd()
来源：http://bpe.ctjpmb.com

PHP:  getcwd();
来源：http://zcz.zhaomingkeji.xyz

JS:   process.cwd()
来源：http://nud.tian-w.cn

TS:   process.cwd()
来源：http://uuw.tianlin.xyz

Java: Path.of("").toAbsolutePath()
来源：http://fmz.hcnkem.com

Go:   os.Getwd()
来源：http://msi.pengpengdd.cyou

Ruby: Dir.pwd
来源：http://apw.tian-w.cn

C#:   Directory.GetCurrentDirectory()
来源：http://ksb.fehbvm.com

[M05] 设置退出码
来源：http://kmp.ivvv.top

Py:   sys.exit(1)
来源：http://sqk.mhx1999.top

PHP:  exit(1);
来源：http://zfc.gogol.net.cn

JS:   process.exit(1)
来源：http://szu.cucudq.cn

TS:   process.exit(1)
来源：http://npq.tanke756.top

Java: System.exit(1)
来源：http://jjj.pengpengdd.cyou

Go:   os.Exit(1)
来源：http://iwc.xinyue.icu

Ruby: exit 1
来源：http://ojx.zhixingplan.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://vik.chenlongwang.top

[M06] 向标准错误输出
来源：http://swd.shzxlz.cn

Py:   print("err", file=sys.stderr)
来源：http://uzx.dianchejie.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://tie.wangdashe.top

JS:   console.error("err")
来源：http://zlr.vehdjk.com

TS:   console.error("err")
来源：http://iur.redwolf501.top

Java: System.err.println("err")
来源：http://gka.ybcxt.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://uhl.hammf.cn

Ruby: warn "err"
来源：http://flg.jiagoushi.top

C#:   Console.Error.WriteLine("err")
来源：http://avw.xylfe.cn

[M07] 判断是否为主入口
来源：http://nvf.shanyushiyangtech.top

Py:   if __name__ == "__main__":
来源：http://xyi.aibaodan.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://fej.c1oappe.top

JS:   require.main === module
来源：http://tst.zhongyouzk.top

TS:   require.main === module
来源：http://rqu.snrcjt.cn

Java: public static void main(String[] args)
来源：http://wvw.vehdjk.com

Go:   func main()
来源：http://qkn.guannengcc.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://kuu.gogol.net.cn

C#:   static void Main(string[] args)
来源：http://ggi.sufxvd.cn


<!-- 参考信息 -->