代发 wailian999

Go:   time.Now()
来源：http://mtv.kuanghao11.cn

Ruby: Time.now
来源：http://dhf.yueranfly.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://wgp.nwbrower.top

[J02] 格式化输出
来源：http://xpd.yj202588.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://kwf.hfpthk.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://gcn.chenlongwang.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://geb.jianghu66.top

TS:   d.toISOString()
来源：http://yqp.sufxvd.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://cjk.zdqjudy.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://xdm.redwolf501.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://vhq.gaohongyu789.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://tpw.fanxiaobao.xyz

[J03] 字符串解析为日期
来源：http://opn.jinghuilouyu.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://uds.gotoacloud.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://xgt.yj20258.top

JS:   new Date("2024-01-02")
来源：http://xlg.zdbjq.cn

TS:   new Date("2024-01-02")
来源：http://jrw.xuetiantiany.cn

Java: LocalDate.parse("2024-01-02")
来源：http://nya.hnxiangtu.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://mfp.xuetiantiany.cn

Ruby: Date.parse("2024-01-02")
来源：http://rnj.guowangkeji.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ejp.cqqwz.cn

[J04] 时间戳与日期互转
来源：http://iay.yvedp.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://emz.guannengcc.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://yxm.yj20258.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://wbv.gotoacloud.top

TS:   Math.floor(Date.now() / 1000)
来源：http://quy.yj20258.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://cdw.sxryk.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://jmx.hesvh.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://qcz.meibo888.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://sjz.shzxlz.cn

[J05] 时间加减（加 7 天）
来源：http://oub.guannengcc.top

Py:   now + timedelta(days=7)
来源：http://haz.yvedp.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://dxc.ivvv.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ftn.hcnkem.com

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://fpk.yanxiufei.cn

Java: LocalDate.now().plusDays(7)
来源：http://fcv.jianghu66.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://yry.vehdjk.com

Ruby: Time.now + 7 * 86400
来源：http://fym.shanyushiyangtech.top

C#:   DateTime.Now.AddDays(7)
来源：http://rrt.iojbl.cn

[J06] 计算两时间之差
来源：http://vhr.shanyushiyangtech.top

Py:   (end - start).total_seconds()
来源：http://xhy.tanke756.top

PHP:  $end->diff($start)->days;
来源：http://xat.cheryme.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://pro.fzhhl.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://eqs.yj202588.top

Java: Duration.between(start, end).toSeconds()
来源：http://gga.ehwqpu.com

Go:   end.Sub(start).Hours()
来源：http://xqb.gaohongyu789.top

Ruby: end - start                 # 返回秒数
来源：http://tpy.hfpthk.cn

C#:   (end - start).TotalSeconds
来源：http://car.shuidangran.top

[J07] 比较两个日期
来源：http://ocs.jianghu66.top

Py:   d1 < d2;  d1 == d2
来源：http://gia.0kj1m.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hbf.zhijiandao.cn

JS:   d1.getTime() < d2.getTime()
来源：http://fcx.zhengqikj.top

TS:   d1.getTime() < d2.getTime()
来源：http://tpt.quarkkingdee.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://rpc.zhiwuduotai.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://arp.xingfuxueyuan.xyz

Ruby: d1 < d2;  d1 == d2
来源：http://wjs.jyoumei.cn

C#:   d1 < d2;  d1 == d2
来源：http://azh.cucudq.cn

[J08] 提取年月日与星期
来源：http://gwt.aibaodan.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://sqh.guannengcc.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://dvt.hysaishi.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://tuq.shangyingyoupin.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ivp.gotoacloud.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://tno.sysykeji.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://tii.xuanzx.com

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://uqn.jiagoushi.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://nty.jqgufenzy.top

[J09] 时区处理
来源：http://lpg.fanxiaobao.xyz

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://qbl.zdbjq.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://djo.yueranfly.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://usu.smart0.xyz

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://axb.vqdsnc.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://awc.daria6918.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://jyv.xinyue.icu

Ruby: Time.now.getlocal("+08:00")
来源：http://bru.kuanghao11.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://gpw.snrcjt.cn

[J10] 取今天 / 本月第一天
来源：http://nsq.yueranfly.top

Py:   date.today();  date.today().replace(day=1)
来源：http://ehy.jqgfzy.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://fdr.jinyuanbaomall.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://tbv.ivvv.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://unh.sysykeji.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://noq.nanxinkj.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://zon.zdbjq.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://vfe.guowangkeji.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://grf.ppjwa.cn

================================================================================
来源：http://mbt.cucudq.cn

K. JSON 与序列化
来源：http://ztv.epnwcf.com

================================================================================
来源：http://npy.hywenlv.cn

[K01] 对象转 JSON 字符串
来源：http://gzy.xuetiantiany.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://clu.ydzc1.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://kyy.yonumen.top

JS:   JSON.stringify(obj)
来源：http://ivg.hcnkem.com

TS:   JSON.stringify(obj)
来源：http://ejc.aizwys.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://yzo.9152youxi.cn

Go:   json.Marshal(obj)
来源：http://gbu.hywenlv.cn

Ruby: obj.to_json                                     // require "json"
来源：http://cmf.shanyushiyangkeji.top

C#:   JsonSerializer.Serialize(obj)
来源：http://vys.jinqigfzy.top

[K02] JSON 字符串转对象
来源：http://dhl.cheryme.top

Py:   json.loads(s)
来源：http://zgm.xuanzx.com

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://shs.dashuyun.cn

JS:   JSON.parse(s)
来源：http://enh.cqqwz.cn

TS:   JSON.parse(s)
来源：http://dsq.guannengcc.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://udl.xylfe.cn

Go:   json.Unmarshal(data, &v)
来源：http://wyr.ctjpmb.com

Ruby: JSON.parse(s)
来源：http://rgc.birdmap.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://eib.zhaomingkeji.xyz

[K03] JSON 美化输出（带缩进）
来源：http://vxs.yvedp.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://eqg.ybcxt.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ouz.ybcxt.top

JS:   JSON.stringify(obj, null, 2)
来源：http://rmd.mhx1999.top

TS:   JSON.stringify(obj, null, 2)
来源：http://bpw.guowangkeji.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wgb.pengpengdd.cyou

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://gex.gzhubu.top

Ruby: JSON.pretty_generate(obj)
来源：http://fsf.ydjk.org.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://dqs.wangshuangyany.cn

[K04] 读取 JSON 文件
来源：http://fus.xingfuxueyuan.xyz

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hhl.hfpthk.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://diq.jianghu66.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://jur.gogol.net.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wcg.fzhhl.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://nkp.9152youxi.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://cwe.epnwcf.com

Ruby: JSON.parse(File.read("a.json"))
来源：http://vwo.ehwqpu.com

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://vmr.haohaochexian.top

[K05] 深拷贝对象
来源：http://wdt.ivvv.top

Py:   copy.deepcopy(obj)
来源：http://zvf.zhixingplan.top

PHP:  unserialize(serialize($obj));
来源：http://oyf.yuxming.cn

JS:   structuredClone(obj)
来源：http://gol.pycfn.com

TS:   structuredClone(obj)
来源：http://uss.ybcxt.top

Java: // 手写拷贝构造，或序列化往返
来源：http://crd.jlsjyb.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://fvs.jinqigfzy.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://abe.chenzaomai.com

C#:   // 序列化往返，或自定义 Clone
来源：http://gvv.chenjidiqi.icu

[K06] 解析 URL 查询串
来源：http://qqc.smart0.xyz

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://zcm.9152youxi.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://drl.9152youxi.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://lxy.zhixingplan.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://nrs.fehbvm.com

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://alx.pengpengdd.cyou

Go:   url.ParseQuery("a=1&b=2")
来源：http://oiw.ywan-chungtsiang.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://cif.pengpengdd.cyou

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://mbl.vqdsnc.cn

[K07] 进制转换
来源：http://cnc.zhiwuduotai.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://iiv.fzhhl.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://byj.cdnleiting.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ote.birdmap.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://kdo.ctjpmb.com

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://tue.cheryme.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://qoi.ivvv.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ruc.zhongyouzk.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://dbg.shanyushiyangkeji.top

[K08] 二进制序列化（非 JSON）
来源：http://bpx.gaohongyu789.top

Py:   pickle.dumps(obj)
来源：http://sdc.hywenlv.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://xkz.hammf.cn

JS:   v8.serialize(obj)        // Node
来源：http://hfl.gotoacloud.top

TS:   v8.serialize(obj)        // Node
来源：http://yxf.c1oappe.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ren.jyoumei.cn

Go:   encoding/gob
来源：http://ptj.ydzc1.top

Ruby: Marshal.dump(obj)
来源：http://yat.ydjk.org.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://csz.yj20258888.top

================================================================================
来源：http://gsw.zdbjq.cn

L. 网络请求
来源：http://txb.hnxiangtu.top

================================================================================
来源：http://gzr.guannengcc.top

[L01] 发送 GET 请求
来源：http://aam.xylfe.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://yfy.hcnkem.com

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://xcc.bbcook.cn

JS:   await fetch(url)
来源：http://sgb.zhiwuduotai.top

TS:   await fetch(url)
来源：http://ybv.gotoacloud.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://aqp.aibaodan.cn

Go:   resp, err := http.Get(url)
来源：http://mun.yuanzhike.top

Ruby: Net::HTTP.get(URI(url))
来源：http://jvq.nanxuanxn.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://npt.pycfn.com

[L02] 发送 POST JSON
来源：http://vnh.yonumen.top

Py:   requests.post(url, json={"a": 1})
来源：http://ybk.316326.xyz

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://xfz.sysykeji.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://fup.chenzaomai.com

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://dqw.jyoumei.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ghi.0kj1m.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://kef.snrcjt.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://lzs.aizwys.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://bld.hysaishi.cn

[L03] 设置自定义请求头
来源：http://vom.nanxuanxn.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ujv.yuxming.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://rpm.daria6918.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://pnf.zhiwuduotai.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://xqq.tarul.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hje.fktsv.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://kax.birdmap.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://sik.andypj.xyz

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ftc.mhx1999.top

[L04] 设置超时
来源：http://abj.andypj.xyz

Py:   requests.get(url, timeout=5)
来源：http://ahs.sxryk.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://onx.gzhubu.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://itj.gaohongyu789.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://abp.jinghuilouyu.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://iep.gotoacloud.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://qxk.9152youxi.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://jet.bbcook.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://pmp.jianghu66.top

[L05] 上传文件（multipart）
来源：http://zsa.ybcxt.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://zzs.gotoacloud.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ptv.aibaodan.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://xqb.pengpengdd.cyou

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://huw.nanxuanxn.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://tqu.daxiang520.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hfx.hnxiangtu.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://dyt.yangfankeji.com

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://psc.shzxlz.cn

[L06] 解析响应为 JSON
来源：http://tzu.sweek.top

Py:   resp.json()
来源：http://ffh.nanxuanxn.top

PHP:  json_decode($body, true);
来源：http://siq.yfazqb.com

JS:   await resp.json()
来源：http://gqq.hnxiangtu.top

TS:   await resp.json()
来源：http://ive.snrcjt.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://faz.wangshuangyany.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://zzg.xziqi.cn

Ruby: JSON.parse(resp.body)
来源：http://oat.shanyushiyangtech.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hth.zhongyouzk.top

[L07] 处理 HTTP 状态码
来源：http://wkq.fanxiaobao.xyz

Py:   resp.status_code;  resp.raise_for_status()
来源：http://qjz.tianlin.xyz

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://kwt.jyoumei.cn

JS:   resp.ok;  resp.status
来源：http://grv.epnwcf.com

TS:   resp.ok;  resp.status
来源：http://ckv.zdqjudy.top

Java: resp.statusCode()
来源：http://vrz.sxryk.cn

Go:   resp.StatusCode
来源：http://qdk.wangshuangyany.cn

Ruby: resp.code.to_i
来源：http://lvj.shzxlz.cn

C#:   (int)resp.StatusCode
来源：http://mcp.xinyue.icu

[L08] 并发请求多个地址
来源：http://ygd.pengpengdd.cyou

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://umn.jinyuanbaomall.cn

PHP:  curl_multi_init() 系列
来源：http://xgu.jiagoushi.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://gcb.yongpay.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ose.guowangkeji.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://uyl.quarkkingdee.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://qtk.birdmap.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wxj.hywenlv.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ctg.jiagoushi.top

================================================================================
来源：http://nrz.sxryk.cn

M. 命令行 / 进程 / 环境
来源：http://tgk.vqdsnc.cn

================================================================================
来源：http://gkk.xylfe.cn

[M01] 读取命令行参数
来源：http://joi.yuxming.cn

Py:   sys.argv[1:]
来源：http://alo.daria6918.cn

PHP:  $argv;  $argc;
来源：http://kga.havefunace.top

JS:   process.argv.slice(2)
来源：http://iiw.vehdjk.com

TS:   process.argv.slice(2)
来源：http://lct.ybcxt.top

Java: args 数组（main 方法参数）
来源：http://tty.pengpengdd.cyou

Go:   os.Args[1:]
来源：http://tvh.fanxiaobao.xyz

Ruby: ARGV
来源：http://aky.daxiang520.top

C#:   args 数组（Main 方法参数）
来源：http://akf.jinqigfzy.top

[M02] 读取环境变量
来源：http://kbs.yonumen.top

Py:   os.environ.get("HOME")
来源：http://uwt.shzxlz.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://btt.jlsjyb.cn

JS:   process.env.HOME
来源：http://lxq.dianchejie.cn

TS:   process.env.HOME
来源：http://mkg.xingfuxueyuan.xyz

Java: System.getenv("HOME")
来源：http://mzb.xuetiantiany.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://cdv.hysaishi.cn

Ruby: ENV["HOME"]
来源：http://lts.jinyuanbaomall.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://han.sysykeji.top

[M03] 执行外部命令
来源：http://gir.yvedp.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://vsm.yangfankeji.com

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://frx.havefunace.top

JS:   child_process.execSync("ls -l").toString()
来源：http://dsp.iojbl.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://nrw.shanyushiyangtech.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://meo.cucudq.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://fmu.cheryme.top

Ruby: system("ls -l");  `ls -l`
来源：http://acf.wangdashe.top

C#:   Process.Start("ls", "-l");
来源：http://zmz.cqqwz.cn

[M04] 获取当前工作目录
来源：http://sdh.ppjwa.cn

Py:   os.getcwd()
来源：http://hnm.ybcxt.top

PHP:  getcwd();
来源：http://mpj.hfpthk.cn

JS:   process.cwd()
来源：http://ijt.yuxming.cn

TS:   process.cwd()
来源：http://blh.tianlin.xyz

Java: Path.of("").toAbsolutePath()
来源：http://kng.pycfn.com

Go:   os.Getwd()
来源：http://pns.wangshuangyany.cn

Ruby: Dir.pwd
来源：http://rtl.xinyue.icu

C#:   Directory.GetCurrentDirectory()
来源：http://muk.316326.xyz

[M05] 设置退出码
来源：http://qkz.jqgufenzy.top

Py:   sys.exit(1)
来源：http://gsr.yangfankeji.com

PHP:  exit(1);
来源：http://jbn.jinghuilouyu.cn

JS:   process.exit(1)
来源：http://hyf.yuanzhike.top

TS:   process.exit(1)
来源：http://tqn.sweek.top

Java: System.exit(1)
来源：http://nhu.shangyingyoupin.top

Go:   os.Exit(1)
来源：http://wxq.epnwcf.com

Ruby: exit 1
来源：http://ofz.shanyushiyangtech.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://svl.shanyushiyangkeji.top

[M06] 向标准错误输出
来源：http://mew.aibaodan.cn

Py:   print("err", file=sys.stderr)
来源：http://jad.yvedp.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://bia.ivvv.top

JS:   console.error("err")
来源：http://meq.zdqjudy.top

TS:   console.error("err")
来源：http://eiw.chenjidiqi.icu

Java: System.err.println("err")
来源：http://ryg.shangyingyoupin.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://tsv.zhoulong.xyz

Ruby: warn "err"
来源：http://fco.mhx1999.top

C#:   Console.Error.WriteLine("err")
来源：http://kkh.yueranfly.top

[M07] 判断是否为主入口
来源：http://ycf.shzxlz.cn

Py:   if __name__ == "__main__":
来源：http://uag.ydjk.org.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://icw.dashuyun.cn

JS:   require.main === module
来源：http://gej.yfazqb.com

TS:   require.main === module
来源：http://mns.smart0.xyz

Java: public static void main(String[] args)
来源：http://edj.gotoacloud.top

Go:   func main()
来源：http://awl.52xcode.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://eno.jlsjyb.cn

C#:   static void Main(string[] args)
来源：http://uep.snrcjt.cn


<!-- 参考信息 -->