代发 wailian999

Go:   time.Now()
来源：http://vfe.52xcode.cn

Ruby: Time.now
来源：http://vpc.ppjwa.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://jnq.ppjwa.cn

[J02] 格式化输出
来源：http://tfw.gotoacloud.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hjh.sweek.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://qnm.xylfe.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://gri.guowangkeji.top

TS:   d.toISOString()
来源：http://hux.meibo888.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://uzj.ybcxt.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hmv.jiagoushi.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://rxq.yongpay.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://gat.shanyushiyangkeji.top

[J03] 字符串解析为日期
来源：http://caq.pycfn.com

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://qzv.cucudq.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ldy.feifeiyinyue.top

JS:   new Date("2024-01-02")
来源：http://hnu.hnqzz.top

TS:   new Date("2024-01-02")
来源：http://hwl.yfazqb.com

Java: LocalDate.parse("2024-01-02")
来源：http://gkm.mhx1999.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://zzy.zhiwuduotai.top

Ruby: Date.parse("2024-01-02")
来源：http://oxt.zhijiandao.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://wsr.sweek.top

[J04] 时间戳与日期互转
来源：http://ctw.quarkkingdee.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hdm.redwolf501.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://pia.zycfv.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://xjz.fehbvm.com

TS:   Math.floor(Date.now() / 1000)
来源：http://zsa.jinqigufen.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://mrs.cashguo.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://jxg.haohaochexian.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://qie.daria6918.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ekp.vqdsnc.cn

[J05] 时间加减（加 7 天）
来源：http://lun.fengsongda.top

Py:   now + timedelta(days=7)
来源：http://vkp.daxiang520.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://ghn.ydzc1.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://gcf.daxiang520.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://cta.uphjek.com

Java: LocalDate.now().plusDays(7)
来源：http://uhk.vehdjk.com

Go:   time.Now().AddDate(0, 0, 7)
来源：http://kyz.sjlbkw.cn

Ruby: Time.now + 7 * 86400
来源：http://utg.zhaomingkeji.xyz

C#:   DateTime.Now.AddDays(7)
来源：http://sld.sjlbkw.cn

[J06] 计算两时间之差
来源：http://hyj.ivvv.top

Py:   (end - start).total_seconds()
来源：http://etj.cashguo.top

PHP:  $end->diff($start)->days;
来源：http://zeu.zdbjq.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://zrl.sjlbkw.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://tgv.vqdsnc.cn

Java: Duration.between(start, end).toSeconds()
来源：http://xgg.chenjidiqi.icu

Go:   end.Sub(start).Hours()
来源：http://rbp.fehbvm.com

Ruby: end - start                 # 返回秒数
来源：http://akf.zhiwuduotai.top

C#:   (end - start).TotalSeconds
来源：http://wsd.jyoumei.cn

[J07] 比较两个日期
来源：http://dow.cucudq.cn

Py:   d1 < d2;  d1 == d2
来源：http://oeg.hcnkem.com

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://bbf.jlsjyb.cn

JS:   d1.getTime() < d2.getTime()
来源：http://ouc.c1oappe.top

TS:   d1.getTime() < d2.getTime()
来源：http://fvz.fktsv.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://tmp.jinqigufen.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://fqr.chenjidiqi.icu

Ruby: d1 < d2;  d1 == d2
来源：http://ckd.daxiang520.top

C#:   d1 < d2;  d1 == d2
来源：http://vcx.fanxiaobao.xyz

[J08] 提取年月日与星期
来源：http://qyi.fehbvm.com

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://aww.shuidangran.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ghm.bjfxy.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://cae.yvedp.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://vac.zhixingplan.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://stw.ppjwa.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://kep.sysykeji.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://uqh.yanxiufei.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://bnh.zhaomingkeji.xyz

[J09] 时区处理
来源：http://veb.jinyuanbaomall.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://bkv.xinyue.icu

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://yof.ybcxt.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://nhw.jqgfzy.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://lkk.cucudq.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://oue.jiagoushi.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://twv.dashuyun.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://ixd.cqqwz.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://jsq.zdbjq.cn

[J10] 取今天 / 本月第一天
来源：http://ywb.snrcjt.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://vmg.jinqigfzy.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://qhd.vqdsnc.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ytl.tanke756.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://lqc.shuidangran.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://tnh.tarul.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://qgo.mhx1999.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://vav.zhaomingkeji.xyz

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://tuj.gaohongyu789.top

================================================================================
来源：http://gof.jqgfzy.top

K. JSON 与序列化
来源：http://bgk.ehwqpu.com

================================================================================
来源：http://tat.fengsongda.top

[K01] 对象转 JSON 字符串
来源：http://syh.gotoacloud.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://qaz.tian-w.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://qah.jinghuilouyu.cn

JS:   JSON.stringify(obj)
来源：http://rce.daria6918.cn

TS:   JSON.stringify(obj)
来源：http://kux.cdnleiting.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://tun.bbcook.cn

Go:   json.Marshal(obj)
来源：http://vez.shanyushiyangtech.top

Ruby: obj.to_json                                     // require "json"
来源：http://mjh.redwolf501.top

C#:   JsonSerializer.Serialize(obj)
来源：http://bza.vehdjk.com

[K02] JSON 字符串转对象
来源：http://ydp.gzhubu.top

Py:   json.loads(s)
来源：http://jdo.316326.xyz

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://sme.52xcode.cn

JS:   JSON.parse(s)
来源：http://bup.ivvv.top

TS:   JSON.parse(s)
来源：http://zsp.fehbvm.com

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://xgx.nwbrower.top

Go:   json.Unmarshal(data, &v)
来源：http://sxh.cheryme.top

Ruby: JSON.parse(s)
来源：http://kan.shanyushiyangkeji.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://rxu.fktsv.cn

[K03] JSON 美化输出（带缩进）
来源：http://ddz.aibaodan.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://abz.fengsongda.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://cif.haohaochexian.top

JS:   JSON.stringify(obj, null, 2)
来源：http://tmj.tianlin.xyz

TS:   JSON.stringify(obj, null, 2)
来源：http://ksh.nanxuanxn.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ptz.daria6918.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ktr.yueranfly.top

Ruby: JSON.pretty_generate(obj)
来源：http://ghy.sysykeji.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://anw.zhaomingkeji.xyz

[K04] 读取 JSON 文件
来源：http://tqc.ctjpmb.com

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://bwq.zycfv.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://tby.tian-w.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://cdp.aizwys.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://zjw.vehdjk.com

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://cav.zhiwuduotai.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ezf.iojbl.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://gzm.yueranfly.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://zdb.quarkkingdee.top

[K05] 深拷贝对象
来源：http://qcu.aibaodan.cn

Py:   copy.deepcopy(obj)
来源：http://ncn.zhoulong.xyz

PHP:  unserialize(serialize($obj));
来源：http://dko.dianchejie.cn

JS:   structuredClone(obj)
来源：http://okr.yuanzhike.top

TS:   structuredClone(obj)
来源：http://fmd.zhongyouzk.top

Java: // 手写拷贝构造，或序列化往返
来源：http://ast.gzhubu.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://yus.yonumen.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://aai.quarkkingdee.top

C#:   // 序列化往返，或自定义 Clone
来源：http://pbn.jyoumei.cn

[K06] 解析 URL 查询串
来源：http://lna.cashguo.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://dxu.xziqi.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://wis.yonumen.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://bax.zdqjudy.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://dqe.zycfv.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://qkk.shzxlz.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://hqs.birdmap.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://sbc.guowangkeji.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://cov.ywan-chungtsiang.top

[K07] 进制转换
来源：http://lbk.jianghu66.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wxm.iojbl.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://cxb.cdnleiting.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://fso.zhoulong.xyz

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://qgv.jqgfzy.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ecq.hnqzz.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ofk.yonumen.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ifu.zhongyouzk.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://aci.52xcode.cn

[K08] 二进制序列化（非 JSON）
来源：http://zkf.havefunace.top

Py:   pickle.dumps(obj)
来源：http://mgt.dianchejie.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://zkq.zycfv.cn

JS:   v8.serialize(obj)        // Node
来源：http://fth.jiagoushi.top

TS:   v8.serialize(obj)        // Node
来源：http://huc.vqdsnc.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://gpl.dashuyun.cn

Go:   encoding/gob
来源：http://qxn.gaohongyu789.top

Ruby: Marshal.dump(obj)
来源：http://bmh.shangyingyoupin.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://tyj.vehdjk.com

================================================================================
来源：http://uru.hnqzz.top

L. 网络请求
来源：http://ydy.kuanghao11.cn

================================================================================
来源：http://vuf.aizwys.cn

[L01] 发送 GET 请求
来源：http://uaj.feifeiyinyue.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://num.meibo888.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://aus.fengsongda.top

JS:   await fetch(url)
来源：http://lwv.sysykeji.top

TS:   await fetch(url)
来源：http://rqi.jqgufenzy.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://gez.fehbvm.com

Go:   resp, err := http.Get(url)
来源：http://mrc.cucudq.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://inw.yvedp.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hiu.jinqigfzy.top

[L02] 发送 POST JSON
来源：http://nqm.tarul.cn

Py:   requests.post(url, json={"a": 1})
来源：http://thx.jqgfzy.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://nqt.xylfe.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://nwq.yangfankeji.com

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://qrs.tarul.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://phw.cashguo.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://vwm.yuxming.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://qqz.hnqzz.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://yjv.yj20258.top

[L03] 设置自定义请求头
来源：http://yeh.hammf.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://htj.shanyushiyangkeji.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ynk.fktsv.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://xdz.fanxiaobao.xyz

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://usw.smart0.xyz

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://pvf.iojbl.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ucj.vqdsnc.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://gap.gaohongyu789.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hkz.yangfankeji.com

[L04] 设置超时
来源：http://abq.jiagoushi.top

Py:   requests.get(url, timeout=5)
来源：http://hyf.dashuyun.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://bku.xziqi.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wvo.jqgufenzy.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://bzm.zycfv.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://tge.bjfxy.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://kix.yuanzhike.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ege.jinghuilouyu.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://dpd.fktsv.cn

[L05] 上传文件（multipart）
来源：http://dju.cqqwz.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://vtq.fanxiaobao.xyz

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://sca.zdbjq.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://clp.mhx1999.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://vpt.fktsv.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://bue.zhongyouzk.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://see.fehbvm.com

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://btw.cheryme.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://abo.sjlbkw.cn

[L06] 解析响应为 JSON
来源：http://lub.0kj1m.cn

Py:   resp.json()
来源：http://pvz.xingfuxueyuan.xyz

PHP:  json_decode($body, true);
来源：http://heg.yj20258888.top

JS:   await resp.json()
来源：http://qnv.ydjk.org.cn

TS:   await resp.json()
来源：http://yds.fzhhl.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://yhu.yj20258.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://isx.kuanghao11.cn

Ruby: JSON.parse(resp.body)
来源：http://vtv.birdmap.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://dzi.zhijiandao.cn

[L07] 处理 HTTP 状态码
来源：http://tbi.redwolf501.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hdf.jinqigufen.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://jkm.dashuyun.cn

JS:   resp.ok;  resp.status
来源：http://kwr.fzhhl.top

TS:   resp.ok;  resp.status
来源：http://czl.fanxiaobao.xyz

Java: resp.statusCode()
来源：http://xld.epnwcf.com

Go:   resp.StatusCode
来源：http://mox.xinyue.icu

Ruby: resp.code.to_i
来源：http://uzx.cdnleiting.top

C#:   (int)resp.StatusCode
来源：http://bjo.zhijiandao.cn

[L08] 并发请求多个地址
来源：http://bgz.yonumen.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://dap.zhaomingkeji.xyz

PHP:  curl_multi_init() 系列
来源：http://gvy.cqqwz.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://jlk.yj20258888.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ftt.xuetiantiany.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://azr.aibaodan.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://qgm.yj20258888.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://dky.jlsjyb.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://duo.zycfv.cn

================================================================================
来源：http://cmy.cashguo.top

M. 命令行 / 进程 / 环境
来源：http://gqe.zhoulong.xyz

================================================================================
来源：http://rsd.redwolf501.top

[M01] 读取命令行参数
来源：http://tyu.yueranfly.top

Py:   sys.argv[1:]
来源：http://lqx.hnxiangtu.top

PHP:  $argv;  $argc;
来源：http://rfr.hysaishi.cn

JS:   process.argv.slice(2)
来源：http://add.jianghu66.top

TS:   process.argv.slice(2)
来源：http://gjw.hammf.cn

Java: args 数组（main 方法参数）
来源：http://llj.tarul.cn

Go:   os.Args[1:]
来源：http://fss.snrcjt.cn

Ruby: ARGV
来源：http://vvi.snrcjt.cn

C#:   args 数组（Main 方法参数）
来源：http://dtj.yfazqb.com

[M02] 读取环境变量
来源：http://avf.jinqigfzy.top

Py:   os.environ.get("HOME")
来源：http://mxi.zhijiandao.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://zxn.9152youxi.cn

JS:   process.env.HOME
来源：http://yxj.hnxiangtu.top

TS:   process.env.HOME
来源：http://ymn.smart0.xyz

Java: System.getenv("HOME")
来源：http://pyr.jqgfzy.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://sbi.yanxiufei.cn

Ruby: ENV["HOME"]
来源：http://peh.jinghuilouyu.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://jvk.hfpthk.cn

[M03] 执行外部命令
来源：http://heo.guowangkeji.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://zdt.yongpay.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://zdc.yj20258.top

JS:   child_process.execSync("ls -l").toString()
来源：http://aih.fanxiaobao.xyz

TS:   child_process.execSync("ls -l").toString()
来源：http://cis.hongshengwenyu.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://tzw.ywan-chungtsiang.top

Go:   exec.Command("ls", "-l").Output()
来源：http://ipd.shanyushiyangkeji.top

Ruby: system("ls -l");  `ls -l`
来源：http://oqr.hywenlv.cn

C#:   Process.Start("ls", "-l");
来源：http://qfv.fktsv.cn

[M04] 获取当前工作目录
来源：http://veh.sysykeji.top

Py:   os.getcwd()
来源：http://xcd.yuanzhike.top

PHP:  getcwd();
来源：http://mvl.yuxming.cn

JS:   process.cwd()
来源：http://mgu.hfpthk.cn

TS:   process.cwd()
来源：http://bmu.yuanzhike.top

Java: Path.of("").toAbsolutePath()
来源：http://lea.aizwys.cn

Go:   os.Getwd()
来源：http://bcw.jinghuilouyu.cn

Ruby: Dir.pwd
来源：http://pxn.zhoulong.xyz

C#:   Directory.GetCurrentDirectory()
来源：http://zfr.feifeiyinyue.top

[M05] 设置退出码
来源：http://wwj.tarul.cn

Py:   sys.exit(1)
来源：http://evj.gogol.net.cn

PHP:  exit(1);
来源：http://hvc.jinyuanbaomall.cn

JS:   process.exit(1)
来源：http://kvb.shanyushiyangkeji.top

TS:   process.exit(1)
来源：http://jhj.yonumen.top

Java: System.exit(1)
来源：http://xqz.meibo888.top

Go:   os.Exit(1)
来源：http://csg.birdmap.top

Ruby: exit 1
来源：http://gcn.snrcjt.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://iog.yuxming.cn

[M06] 向标准错误输出
来源：http://pao.52xcode.cn

Py:   print("err", file=sys.stderr)
来源：http://xag.tanke756.top

PHP:  fwrite(STDERR, "err\n");
来源：http://kyc.hnqzz.top

JS:   console.error("err")
来源：http://fej.xuetiantiany.cn

TS:   console.error("err")
来源：http://bdu.pengpengdd.cyou

Java: System.err.println("err")
来源：http://lex.havefunace.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://jxc.kuanghao11.cn

Ruby: warn "err"
来源：http://aks.nwbrower.top

C#:   Console.Error.WriteLine("err")
来源：http://guj.pycfn.com

[M07] 判断是否为主入口
来源：http://dvz.zhengqikj.top

Py:   if __name__ == "__main__":
来源：http://eej.redwolf501.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://toc.jinqigufen.top

JS:   require.main === module
来源：http://ssz.quarkkingdee.top

TS:   require.main === module
来源：http://etl.shzxlz.cn

Java: public static void main(String[] args)
来源：http://zov.hywenlv.cn

Go:   func main()
来源：http://mua.xziqi.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ldh.vqdsnc.cn

C#:   static void Main(string[] args)
来源：http://azi.cheryme.top


<!-- 参考信息 -->