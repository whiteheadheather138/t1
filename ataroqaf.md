代发 wailian999

Go:   time.Now()
来源：http://wzq.chenzaomai.com

Ruby: Time.now
来源：http://scs.yj20258.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://rfj.uphjek.com

[J02] 格式化输出
来源：http://amy.ppjwa.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://fuj.dashuyun.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ydc.cashguo.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://bpw.gotoacloud.top

TS:   d.toISOString()
来源：http://zrl.shanyushiyangkeji.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ayv.quarkkingdee.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://lpe.9152youxi.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://atw.cashguo.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://nyg.bjfxy.top

[J03] 字符串解析为日期
来源：http://yvd.ctjpmb.com

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://few.sweek.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://utx.gaohongyu789.top

JS:   new Date("2024-01-02")
来源：http://fdp.mhx1999.top

TS:   new Date("2024-01-02")
来源：http://ava.sweek.top

Java: LocalDate.parse("2024-01-02")
来源：http://hvp.hongshengwenyu.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://grr.fzhhl.top

Ruby: Date.parse("2024-01-02")
来源：http://zzx.jinqigfzy.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://vdc.fzhhl.top

[J04] 时间戳与日期互转
来源：http://nnj.jinqigufen.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://brt.pycfn.com

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://pty.fanxiaobao.xyz

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://gya.hnqzz.top

TS:   Math.floor(Date.now() / 1000)
来源：http://otb.yfazqb.com

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://rlr.jinyuanbaomall.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://mol.hnqzz.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://mvi.uphjek.com

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://sap.316326.xyz

[J05] 时间加减（加 7 天）
来源：http://pff.yuxming.cn

Py:   now + timedelta(days=7)
来源：http://syd.yfazqb.com

PHP:  (new DateTime())->modify("+7 days");
来源：http://gyy.yueranfly.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://xma.gotoacloud.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hwk.shzxlz.cn

Java: LocalDate.now().plusDays(7)
来源：http://sdn.vqdsnc.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://zol.jlsjyb.cn

Ruby: Time.now + 7 * 86400
来源：http://qdt.hnqzz.top

C#:   DateTime.Now.AddDays(7)
来源：http://qhd.nanxuanxn.top

[J06] 计算两时间之差
来源：http://aki.iojbl.cn

Py:   (end - start).total_seconds()
来源：http://eqx.shanyushiyangtech.top

PHP:  $end->diff($start)->days;
来源：http://lcx.fktsv.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://zez.ehwqpu.com

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://bgr.vehdjk.com

Java: Duration.between(start, end).toSeconds()
来源：http://cji.aizwys.cn

Go:   end.Sub(start).Hours()
来源：http://gwh.hongshengwenyu.top

Ruby: end - start                 # 返回秒数
来源：http://ytg.guannengcc.top

C#:   (end - start).TotalSeconds
来源：http://fkg.ivvv.top

[J07] 比较两个日期
来源：http://yjm.daxiang520.top

Py:   d1 < d2;  d1 == d2
来源：http://etr.havefunace.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://gsl.quarkkingdee.top

JS:   d1.getTime() < d2.getTime()
来源：http://xtp.pycfn.com

TS:   d1.getTime() < d2.getTime()
来源：http://wjc.aibaodan.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://dwn.ppjwa.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://xgw.hnqzz.top

Ruby: d1 < d2;  d1 == d2
来源：http://yno.bbcook.cn

C#:   d1 < d2;  d1 == d2
来源：http://ful.iojbl.cn

[J08] 提取年月日与星期
来源：http://sch.guowangkeji.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://chs.haohaochexian.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://cks.guowangkeji.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://psh.yfazqb.com

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://vpv.haohaochexian.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://kkz.yueranfly.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://oma.havefunace.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://abm.quarkkingdee.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://onk.birdmap.top

[J09] 时区处理
来源：http://ggd.cheryme.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hdj.sxryk.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://bju.hnxiangtu.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ugs.jianghu66.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://yuy.tarul.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://jda.sufxvd.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://erx.yonumen.top

Ruby: Time.now.getlocal("+08:00")
来源：http://djd.nanxuanxn.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://kdx.shanyushiyangkeji.top

[J10] 取今天 / 本月第一天
来源：http://osu.feifeiyinyue.top

Py:   date.today();  date.today().replace(day=1)
来源：http://tma.hnqzz.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://zzx.jiagoushi.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://itx.zhoulong.xyz

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://zjr.c1oappe.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ovj.yuanzhike.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://yle.sjlbkw.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://kqm.jinqigfzy.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://efh.meibo888.top

================================================================================
来源：http://alp.jiagoushi.top

K. JSON 与序列化
来源：http://azn.yangfankeji.com

================================================================================
来源：http://iuw.andypj.xyz

[K01] 对象转 JSON 字符串
来源：http://prl.yanxiufei.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://onb.iojbl.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hmw.fanxiaobao.xyz

JS:   JSON.stringify(obj)
来源：http://pgk.shanyushiyangtech.top

TS:   JSON.stringify(obj)
来源：http://zkv.snrcjt.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ena.sysykeji.top

Go:   json.Marshal(obj)
来源：http://lsa.sxryk.cn

Ruby: obj.to_json                                     // require "json"
来源：http://sqo.jinqigfzy.top

C#:   JsonSerializer.Serialize(obj)
来源：http://gqz.yanxiufei.cn

[K02] JSON 字符串转对象
来源：http://fbv.hammf.cn

Py:   json.loads(s)
来源：http://zgm.tarul.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://mfl.jinqigufen.top

JS:   JSON.parse(s)
来源：http://elx.fktsv.cn

TS:   JSON.parse(s)
来源：http://tbe.kuanghao11.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://jbm.ywan-chungtsiang.top

Go:   json.Unmarshal(data, &v)
来源：http://znc.fktsv.cn

Ruby: JSON.parse(s)
来源：http://mot.ctjpmb.com

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://dps.sweek.top

[K03] JSON 美化输出（带缩进）
来源：http://hxl.jinghuilouyu.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ipj.zhixingplan.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://qww.jqgfzy.top

JS:   JSON.stringify(obj, null, 2)
来源：http://vuq.hfpthk.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://psn.sjlbkw.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://pkw.yueranfly.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://byc.ppjwa.cn

Ruby: JSON.pretty_generate(obj)
来源：http://pjn.daria6918.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://dqi.52xcode.cn

[K04] 读取 JSON 文件
来源：http://qvi.c1oappe.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://oow.haohaochexian.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ers.gaohongyu789.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://xrp.yj202588.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wac.mhx1999.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://met.yfazqb.com

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://qzp.xuanzx.com

Ruby: JSON.parse(File.read("a.json"))
来源：http://sej.haohaochexian.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://isb.sxryk.cn

[K05] 深拷贝对象
来源：http://yah.daria6918.cn

Py:   copy.deepcopy(obj)
来源：http://mux.vehdjk.com

PHP:  unserialize(serialize($obj));
来源：http://met.jinqigufen.top

JS:   structuredClone(obj)
来源：http://eed.svipenyu.cn

TS:   structuredClone(obj)
来源：http://lot.hnxiangtu.top

Java: // 手写拷贝构造，或序列化往返
来源：http://vep.ydjk.org.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://icc.bbcook.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://bek.haohaochexian.top

C#:   // 序列化往返，或自定义 Clone
来源：http://jrc.0kj1m.cn

[K06] 解析 URL 查询串
来源：http://zif.hammf.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ryu.daria6918.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://nom.xinyue.icu

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://bcy.hfpthk.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://rpc.quarkkingdee.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ohv.tian-w.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://ija.jinqigfzy.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://laj.vehdjk.com

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://jat.yueranfly.top

[K07] 进制转换
来源：http://fbk.sysykeji.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://dhz.fengsongda.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://vun.wangdashe.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://cfy.yonumen.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://uso.yonumen.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://csk.sysykeji.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hws.feifeiyinyue.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://zvg.gzhubu.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://vdl.meibo888.top

[K08] 二进制序列化（非 JSON）
来源：http://ukg.yangfankeji.com

Py:   pickle.dumps(obj)
来源：http://ctg.birdmap.top

PHP:  serialize($obj);  unserialize($s);
来源：http://qvv.zhoulong.xyz

JS:   v8.serialize(obj)        // Node
来源：http://yzy.ivvv.top

TS:   v8.serialize(obj)        // Node
来源：http://aoc.yuanzhike.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://iti.ppjwa.cn

Go:   encoding/gob
来源：http://zyc.yonumen.top

Ruby: Marshal.dump(obj)
来源：http://wtz.yuanzhike.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://had.zhengqikj.top

================================================================================
来源：http://ejn.xinyue.icu

L. 网络请求
来源：http://czx.vqdsnc.cn

================================================================================
来源：http://dki.52xcode.cn

[L01] 发送 GET 请求
来源：http://gvl.aibaodan.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://tuz.fehbvm.com

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://que.yj20258.top

JS:   await fetch(url)
来源：http://xvy.jinqigufen.top

TS:   await fetch(url)
来源：http://owc.andypj.xyz

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://noa.snrcjt.cn

Go:   resp, err := http.Get(url)
来源：http://the.sysykeji.top

Ruby: Net::HTTP.get(URI(url))
来源：http://fzm.yj202588.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://qel.hnxiangtu.top

[L02] 发送 POST JSON
来源：http://mfb.fanxiaobao.xyz

Py:   requests.post(url, json={"a": 1})
来源：http://hsz.jinyuanbaomall.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://qnh.jiagoushi.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://nes.xziqi.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://aad.wangshuangyany.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mkp.gzhubu.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ecw.cqqwz.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://xqb.zycfv.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://lwm.ydjk.org.cn

[L03] 设置自定义请求头
来源：http://ubg.smart0.xyz

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://afa.yfazqb.com

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://bdz.hesvh.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://bfq.bjfxy.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://bhe.pycfn.com

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hsm.wangshuangyany.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://eex.jyoumei.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://prl.sufxvd.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://nvs.pengpengdd.cyou

[L04] 设置超时
来源：http://eph.zhengqikj.top

Py:   requests.get(url, timeout=5)
来源：http://llk.zhongyouzk.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://bmx.xuanzx.com

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mdb.gzhubu.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://oqr.ctjpmb.com

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://tfr.meibo888.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ahc.shuidangran.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://bxp.zdbjq.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://jmn.xingfuxueyuan.xyz

[L05] 上传文件（multipart）
来源：http://pqs.sweek.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://vhz.cdnleiting.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://pcr.daria6918.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://xpl.gzhubu.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://zxm.dashuyun.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://auv.ehwqpu.com

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://rcj.zdqjudy.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://aon.epnwcf.com

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://foj.cqqwz.cn

[L06] 解析响应为 JSON
来源：http://vfj.yonumen.top

Py:   resp.json()
来源：http://mwy.shzxlz.cn

PHP:  json_decode($body, true);
来源：http://biw.uphjek.com

JS:   await resp.json()
来源：http://vba.fehbvm.com

TS:   await resp.json()
来源：http://vqq.svipenyu.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mby.tian-w.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://zwh.jlsjyb.cn

Ruby: JSON.parse(resp.body)
来源：http://yfv.fzhhl.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://bii.gaohongyu789.top

[L07] 处理 HTTP 状态码
来源：http://zuw.hcnkem.com

Py:   resp.status_code;  resp.raise_for_status()
来源：http://kqy.yvedp.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ezu.xziqi.cn

JS:   resp.ok;  resp.status
来源：http://qmr.pycfn.com

TS:   resp.ok;  resp.status
来源：http://cov.9152youxi.cn

Java: resp.statusCode()
来源：http://xmt.guowangkeji.top

Go:   resp.StatusCode
来源：http://ffj.yongpay.top

Ruby: resp.code.to_i
来源：http://jfm.jinqigufen.top

C#:   (int)resp.StatusCode
来源：http://rqu.zycfv.cn

[L08] 并发请求多个地址
来源：http://owd.vqdsnc.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://nea.xingfuxueyuan.xyz

PHP:  curl_multi_init() 系列
来源：http://zap.chenzaomai.com

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://zlz.meibo888.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://zlj.nwbrower.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ulw.zhixingplan.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://uzw.xuanzx.com

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://lbo.bjfxy.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://xiu.hnxiangtu.top

================================================================================
来源：http://uet.feifeiyinyue.top

M. 命令行 / 进程 / 环境
来源：http://nhe.ydjk.org.cn

================================================================================
来源：http://efz.cucudq.cn

[M01] 读取命令行参数
来源：http://mzm.sweek.top

Py:   sys.argv[1:]
来源：http://qvx.wangshuangyany.cn

PHP:  $argv;  $argc;
来源：http://dgt.c1oappe.top

JS:   process.argv.slice(2)
来源：http://mat.dashuyun.cn

TS:   process.argv.slice(2)
来源：http://nlb.kuanghao11.cn

Java: args 数组（main 方法参数）
来源：http://gpd.jianghu66.top

Go:   os.Args[1:]
来源：http://sqa.xinyue.icu

Ruby: ARGV
来源：http://rku.zhiwuduotai.top

C#:   args 数组（Main 方法参数）
来源：http://wlh.sufxvd.cn

[M02] 读取环境变量
来源：http://jdl.andypj.xyz

Py:   os.environ.get("HOME")
来源：http://txl.cucudq.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://zrw.gogol.net.cn

JS:   process.env.HOME
来源：http://dim.xylfe.cn

TS:   process.env.HOME
来源：http://igl.0kj1m.cn

Java: System.getenv("HOME")
来源：http://nej.xinyue.icu

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wtn.zdbjq.cn

Ruby: ENV["HOME"]
来源：http://emy.gaohongyu789.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ddn.shzxlz.cn

[M03] 执行外部命令
来源：http://bcj.fanxiaobao.xyz

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hlx.iojbl.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://jgv.yj20258888.top

JS:   child_process.execSync("ls -l").toString()
来源：http://gdp.xingfuxueyuan.xyz

TS:   child_process.execSync("ls -l").toString()
来源：http://kfb.nanxuanxn.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://djn.jinqigufen.top

Go:   exec.Command("ls", "-l").Output()
来源：http://wqy.birdmap.top

Ruby: system("ls -l");  `ls -l`
来源：http://bsi.redwolf501.top

C#:   Process.Start("ls", "-l");
来源：http://jlw.cheryme.top

[M04] 获取当前工作目录
来源：http://crc.fehbvm.com

Py:   os.getcwd()
来源：http://ziz.aibaodan.cn

PHP:  getcwd();
来源：http://zsr.hfpthk.cn

JS:   process.cwd()
来源：http://sdu.gzhubu.top

TS:   process.cwd()
来源：http://plw.c1oappe.top

Java: Path.of("").toAbsolutePath()
来源：http://ukh.tanke756.top

Go:   os.Getwd()
来源：http://alc.bbcook.cn

Ruby: Dir.pwd
来源：http://wnu.meibo888.top

C#:   Directory.GetCurrentDirectory()
来源：http://mhg.cdnleiting.top

[M05] 设置退出码
来源：http://nla.jiagoushi.top

Py:   sys.exit(1)
来源：http://phg.yvedp.cn

PHP:  exit(1);
来源：http://xpr.ehwqpu.com

JS:   process.exit(1)
来源：http://ute.xinyue.icu

TS:   process.exit(1)
来源：http://pqz.ehwqpu.com

Java: System.exit(1)
来源：http://huy.xinyue.icu

Go:   os.Exit(1)
来源：http://fny.nanxuanxn.top

Ruby: exit 1
来源：http://hvp.sxryk.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://qdx.dashuyun.cn

[M06] 向标准错误输出
来源：http://qop.zhengqikj.top

Py:   print("err", file=sys.stderr)
来源：http://zcb.yuxming.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://xis.bjfxy.top

JS:   console.error("err")
来源：http://lew.yvedp.cn

TS:   console.error("err")
来源：http://jda.havefunace.top

Java: System.err.println("err")
来源：http://mby.shangyingyoupin.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hhs.ywan-chungtsiang.top

Ruby: warn "err"
来源：http://bku.shanyushiyangtech.top

C#:   Console.Error.WriteLine("err")
来源：http://rti.ehwqpu.com

[M07] 判断是否为主入口
来源：http://yvn.chenzaomai.com

Py:   if __name__ == "__main__":
来源：http://sxl.cdnleiting.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://cmk.vqdsnc.cn

JS:   require.main === module
来源：http://wnb.kuanghao11.cn

TS:   require.main === module
来源：http://uvi.ehwqpu.com

Java: public static void main(String[] args)
来源：http://bpg.zhongyouzk.top

Go:   func main()
来源：http://bqt.jiagoushi.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://jbg.yongpay.top

C#:   static void Main(string[] args)
来源：http://cce.yj20258.top


<!-- 参考信息 -->