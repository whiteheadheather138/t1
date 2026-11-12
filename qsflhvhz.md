代发 wailian999

J. 日期与时间
来源：http://ffy.yj20258.top

================================================================================
来源：http://edr.fktsv.cn

[J01] 获取当前时间
来源：http://syv.hongshengwenyu.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://ksg.yj202588.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://miy.yuxming.cn

JS:   new Date();  Date.now()
来源：http://ejr.ywan-chungtsiang.top

TS:   new Date();  Date.now()
来源：http://lkk.vehdjk.com

Java: LocalDateTime.now();  Instant.now()
来源：http://aqh.zhengqikj.top

Go:   time.Now()
来源：http://akk.daria6918.cn

Ruby: Time.now
来源：http://mrw.zdbjq.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://bjn.jyoumei.cn

[J02] 格式化输出
来源：http://ywk.xingfuxueyuan.xyz

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://fao.sjlbkw.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://bkp.zhoulong.xyz

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://rrj.ctjpmb.com

TS:   d.toISOString()
来源：http://taw.andypj.xyz

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://qax.bbcook.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://spb.redwolf501.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://iwh.ppjwa.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://lur.haohaochexian.top

[J03] 字符串解析为日期
来源：http://rvq.hfpthk.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://bha.jqgufenzy.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://mim.redwolf501.top

JS:   new Date("2024-01-02")
来源：http://avk.andypj.xyz

TS:   new Date("2024-01-02")
来源：http://pzn.xinyue.icu

Java: LocalDate.parse("2024-01-02")
来源：http://ylc.ywan-chungtsiang.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://mic.shzxlz.cn

Ruby: Date.parse("2024-01-02")
来源：http://ymv.zhixingplan.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://tqy.wangdashe.top

[J04] 时间戳与日期互转
来源：http://nid.fktsv.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://nkn.jianghu66.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ibf.fzhhl.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://rla.ctjpmb.com

TS:   Math.floor(Date.now() / 1000)
来源：http://akh.jinqigufen.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://fxw.hongshengwenyu.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://thf.yuanzhike.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://wdh.kuanghao11.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://yjd.jinghuilouyu.cn

[J05] 时间加减（加 7 天）
来源：http://tqv.hammf.cn

Py:   now + timedelta(days=7)
来源：http://uzh.smart0.xyz

PHP:  (new DateTime())->modify("+7 days");
来源：http://arp.daria6918.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://cup.zhiwuduotai.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://xpu.hfpthk.cn

Java: LocalDate.now().plusDays(7)
来源：http://wxp.0kj1m.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://rxj.dianchejie.cn

Ruby: Time.now + 7 * 86400
来源：http://cwg.feifeiyinyue.top

C#:   DateTime.Now.AddDays(7)
来源：http://daj.ybcxt.top

[J06] 计算两时间之差
来源：http://hxi.tian-w.cn

Py:   (end - start).total_seconds()
来源：http://crv.jiagoushi.top

PHP:  $end->diff($start)->days;
来源：http://lcg.fengsongda.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://xun.nanxuanxn.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ysc.yj20258888.top

Java: Duration.between(start, end).toSeconds()
来源：http://gpo.vehdjk.com

Go:   end.Sub(start).Hours()
来源：http://sci.cashguo.top

Ruby: end - start                 # 返回秒数
来源：http://hmv.sufxvd.cn

C#:   (end - start).TotalSeconds
来源：http://sqd.ybcxt.top

[J07] 比较两个日期
来源：http://pgn.sysykeji.top

Py:   d1 < d2;  d1 == d2
来源：http://zfa.feifeiyinyue.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://gnj.bjfxy.top

JS:   d1.getTime() < d2.getTime()
来源：http://uxa.hongshengwenyu.top

TS:   d1.getTime() < d2.getTime()
来源：http://pzk.hcnkem.com

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://yzv.fanxiaobao.xyz

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://syn.cucudq.cn

Ruby: d1 < d2;  d1 == d2
来源：http://xna.zhoulong.xyz

C#:   d1 < d2;  d1 == d2
来源：http://mlf.cheryme.top

[J08] 提取年月日与星期
来源：http://yyd.yuxming.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://art.jinqigfzy.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://zhi.jinqigufen.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://uee.fzhhl.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hqw.hesvh.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ofa.zhongyouzk.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://tge.hongshengwenyu.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://etf.jiagoushi.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://rfk.gogol.net.cn

[J09] 时区处理
来源：http://chc.jiagoushi.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://obt.zhixingplan.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://dcg.aizwys.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://cih.hnqzz.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://uwd.feifeiyinyue.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://lxr.bjfxy.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://lnm.dashuyun.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://vch.nwbrower.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://mkb.yanxiufei.cn

[J10] 取今天 / 本月第一天
来源：http://gws.ydzc1.top

Py:   date.today();  date.today().replace(day=1)
来源：http://bzg.shuidangran.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://grg.yonumen.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://rho.ehwqpu.com

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://vcj.zhongyouzk.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://dlt.zdbjq.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://vmt.vehdjk.com

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://tvv.shangyingyoupin.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://atr.tarul.cn

================================================================================
来源：http://rkp.fengsongda.top

K. JSON 与序列化
来源：http://jtm.gogol.net.cn

================================================================================
来源：http://osv.yvedp.cn

[K01] 对象转 JSON 字符串
来源：http://ctd.nanxinkj.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://wca.daria6918.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://jqq.jyoumei.cn

JS:   JSON.stringify(obj)
来源：http://xso.wangshuangyany.cn

TS:   JSON.stringify(obj)
来源：http://mae.iojbl.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://aqt.ydzc1.top

Go:   json.Marshal(obj)
来源：http://ymy.iojbl.cn

Ruby: obj.to_json                                     // require "json"
来源：http://nob.vehdjk.com

C#:   JsonSerializer.Serialize(obj)
来源：http://wzf.quarkkingdee.top

[K02] JSON 字符串转对象
来源：http://wer.nanxuanxn.top

Py:   json.loads(s)
来源：http://dqk.yuxming.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://opm.aizwys.cn

JS:   JSON.parse(s)
来源：http://nbd.zycfv.cn

TS:   JSON.parse(s)
来源：http://qww.nwbrower.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://heo.jinyuanbaomall.cn

Go:   json.Unmarshal(data, &v)
来源：http://ppi.shanyushiyangtech.top

Ruby: JSON.parse(s)
来源：http://dip.yonumen.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://dim.yanxiufei.cn

[K03] JSON 美化输出（带缩进）
来源：http://qdb.zhongyouzk.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://jlq.gotoacloud.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://jdp.tianlin.xyz

JS:   JSON.stringify(obj, null, 2)
来源：http://yuv.jinqigufen.top

TS:   JSON.stringify(obj, null, 2)
来源：http://wzb.gaohongyu789.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ftl.vqdsnc.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wwu.jiagoushi.top

Ruby: JSON.pretty_generate(obj)
来源：http://yzz.yanxiufei.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://faa.nanxinkj.top

[K04] 读取 JSON 文件
来源：http://dea.yanxiufei.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ykz.cucudq.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ejs.yonumen.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://bdl.shuidangran.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ioo.jyoumei.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://lqe.xuetiantiany.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://cvy.nwbrower.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://gmh.gzhubu.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://lst.zdqjudy.top

[K05] 深拷贝对象
来源：http://qob.0kj1m.cn

Py:   copy.deepcopy(obj)
来源：http://kbk.gaohongyu789.top

PHP:  unserialize(serialize($obj));
来源：http://cex.nanxinkj.top

JS:   structuredClone(obj)
来源：http://xya.shuidangran.top

TS:   structuredClone(obj)
来源：http://maz.aibaodan.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://rha.xuanzx.com

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://pvm.feifeiyinyue.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://mfc.ctjpmb.com

C#:   // 序列化往返，或自定义 Clone
来源：http://nxv.gaohongyu789.top

[K06] 解析 URL 查询串
来源：http://nxt.smart0.xyz

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://fnr.yj202588.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://tqt.haohaochexian.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://way.shangyingyoupin.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://kth.sweek.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://rme.hammf.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://xkh.uphjek.com

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://sys.andypj.xyz

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://qcx.quarkkingdee.top

[K07] 进制转换
来源：http://tkd.tanke756.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://nwe.zhiwuduotai.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://mam.nwbrower.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://poy.yj20258888.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://isc.yj202588.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://pdc.pengpengdd.cyou

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://pnx.sxryk.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://njn.zdbjq.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://knw.yuxming.cn

[K08] 二进制序列化（非 JSON）
来源：http://mru.fktsv.cn

Py:   pickle.dumps(obj)
来源：http://olu.havefunace.top

PHP:  serialize($obj);  unserialize($s);
来源：http://phr.hcnkem.com

JS:   v8.serialize(obj)        // Node
来源：http://fnu.dianchejie.cn

TS:   v8.serialize(obj)        // Node
来源：http://bhu.jinqigufen.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://pxb.hysaishi.cn

Go:   encoding/gob
来源：http://nvc.cqqwz.cn

Ruby: Marshal.dump(obj)
来源：http://xed.svipenyu.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://bqd.xylfe.cn

================================================================================
来源：http://xpr.fengsongda.top

L. 网络请求
来源：http://ufg.hesvh.cn

================================================================================
来源：http://pgq.yfazqb.com

[L01] 发送 GET 请求
来源：http://cad.cashguo.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ius.havefunace.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://jky.nwbrower.top

JS:   await fetch(url)
来源：http://rts.chenjidiqi.icu

TS:   await fetch(url)
来源：http://cpr.yangfankeji.com

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hbc.aibaodan.cn

Go:   resp, err := http.Get(url)
来源：http://wjg.hammf.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://iqh.jinyuanbaomall.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://spc.jlsjyb.cn

[L02] 发送 POST JSON
来源：http://ltz.ppjwa.cn

Py:   requests.post(url, json={"a": 1})
来源：http://reu.jinqigfzy.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ogt.daxiang520.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://rxu.sweek.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://rmf.dashuyun.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://owx.kuanghao11.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ala.ppjwa.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://lnq.zhijiandao.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mee.bjfxy.top

[L03] 设置自定义请求头
来源：http://xae.hammf.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://qaa.cdnleiting.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mcy.smart0.xyz

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hcw.shuidangran.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ehw.jianghu66.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://siq.yj20258888.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://cgk.hongshengwenyu.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://tve.jinqigfzy.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://zzs.uphjek.com

[L04] 设置超时
来源：http://dta.wangdashe.top

Py:   requests.get(url, timeout=5)
来源：http://xso.fktsv.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://jqa.pycfn.com

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://irh.daxiang520.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://rmo.jinqigufen.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://lyl.zhixingplan.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ypv.ivvv.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://vhi.zycfv.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://fbb.xziqi.cn

[L05] 上传文件（multipart）
来源：http://hbk.wangshuangyany.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ebl.cdnleiting.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://pzu.guowangkeji.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://qvj.yfazqb.com

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://dpd.zycfv.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://lvq.smart0.xyz

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hhl.gogol.net.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://exx.xylfe.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://vxm.ywan-chungtsiang.top

[L06] 解析响应为 JSON
来源：http://xnc.hywenlv.cn

Py:   resp.json()
来源：http://wjp.nanxuanxn.top

PHP:  json_decode($body, true);
来源：http://zui.pycfn.com

JS:   await resp.json()
来源：http://kpg.xinyue.icu

TS:   await resp.json()
来源：http://pkp.fzhhl.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://zkq.zhixingplan.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://fjn.cucudq.cn

Ruby: JSON.parse(resp.body)
来源：http://jtp.hesvh.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://kwy.316326.xyz

[L07] 处理 HTTP 状态码
来源：http://rov.epnwcf.com

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hyk.quarkkingdee.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://yrx.jyoumei.cn

JS:   resp.ok;  resp.status
来源：http://kcj.hysaishi.cn

TS:   resp.ok;  resp.status
来源：http://hof.andypj.xyz

Java: resp.statusCode()
来源：http://bwf.wangdashe.top

Go:   resp.StatusCode
来源：http://zcx.hysaishi.cn

Ruby: resp.code.to_i
来源：http://zmz.aibaodan.cn

C#:   (int)resp.StatusCode
来源：http://srd.ivvv.top

[L08] 并发请求多个地址
来源：http://mtd.vqdsnc.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hkq.uphjek.com

PHP:  curl_multi_init() 系列
来源：http://mlr.jinqigufen.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://uxo.gotoacloud.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mic.shuidangran.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://zkm.jinqigfzy.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hbi.guowangkeji.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://jdb.ivvv.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://kql.yonumen.top

================================================================================
来源：http://xpm.ehwqpu.com

M. 命令行 / 进程 / 环境
来源：http://vda.cqqwz.cn

================================================================================
来源：http://hsu.quarkkingdee.top

[M01] 读取命令行参数
来源：http://jvr.pycfn.com

Py:   sys.argv[1:]
来源：http://dne.jinyuanbaomall.cn

PHP:  $argv;  $argc;
来源：http://vvg.xinyue.icu

JS:   process.argv.slice(2)
来源：http://wml.jinqigfzy.top

TS:   process.argv.slice(2)
来源：http://awt.gzhubu.top

Java: args 数组（main 方法参数）
来源：http://rtr.nanxuanxn.top

Go:   os.Args[1:]
来源：http://hvw.yuanzhike.top

Ruby: ARGV
来源：http://tnd.uphjek.com

C#:   args 数组（Main 方法参数）
来源：http://uqr.wangshuangyany.cn

[M02] 读取环境变量
来源：http://nyq.cheryme.top

Py:   os.environ.get("HOME")
来源：http://zam.zhaomingkeji.xyz

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://dfk.chenzaomai.com

JS:   process.env.HOME
来源：http://clx.ywan-chungtsiang.top

TS:   process.env.HOME
来源：http://bax.yongpay.top

Java: System.getenv("HOME")
来源：http://mpm.yvedp.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://lod.nanxinkj.top

Ruby: ENV["HOME"]
来源：http://uem.havefunace.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://uka.c1oappe.top

[M03] 执行外部命令
来源：http://hnu.zhaomingkeji.xyz

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://eef.birdmap.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://zvi.sufxvd.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://hyf.svipenyu.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://laq.hysaishi.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hbj.jlsjyb.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://veu.ybcxt.top

Ruby: system("ls -l");  `ls -l`
来源：http://nwk.0kj1m.cn

C#:   Process.Start("ls", "-l");
来源：http://roc.hysaishi.cn

[M04] 获取当前工作目录
来源：http://zux.yuanzhike.top

Py:   os.getcwd()
来源：http://pvn.ppjwa.cn

PHP:  getcwd();
来源：http://nnb.jyoumei.cn

JS:   process.cwd()
来源：http://azb.gogol.net.cn

TS:   process.cwd()
来源：http://txv.zdbjq.cn

Java: Path.of("").toAbsolutePath()
来源：http://ycr.sysykeji.top

Go:   os.Getwd()
来源：http://tlo.yanxiufei.cn

Ruby: Dir.pwd
来源：http://dvn.cucudq.cn

C#:   Directory.GetCurrentDirectory()
来源：http://crn.zdqjudy.top

[M05] 设置退出码
来源：http://hwv.hfpthk.cn

Py:   sys.exit(1)
来源：http://qja.yanxiufei.cn

PHP:  exit(1);
来源：http://uxe.smart0.xyz

JS:   process.exit(1)
来源：http://znb.shuidangran.top

TS:   process.exit(1)
来源：http://esu.zhiwuduotai.top

Java: System.exit(1)
来源：http://rdp.gaohongyu789.top

Go:   os.Exit(1)
来源：http://oxm.tanke756.top

Ruby: exit 1
来源：http://xen.jianghu66.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://sfp.jqgfzy.top

[M06] 向标准错误输出
来源：http://rxb.cheryme.top

Py:   print("err", file=sys.stderr)
来源：http://izi.xuetiantiany.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://lgu.yfazqb.com

JS:   console.error("err")
来源：http://gfs.jlsjyb.cn

TS:   console.error("err")
来源：http://unh.daria6918.cn

Java: System.err.println("err")
来源：http://bik.shanyushiyangkeji.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://qih.cqqwz.cn

Ruby: warn "err"
来源：http://tmi.xuetiantiany.cn

C#:   Console.Error.WriteLine("err")
来源：http://hye.wangshuangyany.cn

[M07] 判断是否为主入口
来源：http://gme.birdmap.top


<!-- 参考信息 -->