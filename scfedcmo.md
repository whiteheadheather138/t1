代发 wailian999

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://zid.sjlbkw.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hyp.cheryme.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://haz.52xcode.cn

TS:   d.toISOString()
来源：http://iph.wangshuangyany.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://oym.daria6918.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://edu.ivvv.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ujl.sweek.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://tby.xziqi.cn

[J03] 字符串解析为日期
来源：http://bdn.quarkkingdee.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://unp.yj20258888.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://uqe.mhx1999.top

JS:   new Date("2024-01-02")
来源：http://ejw.quarkkingdee.top

TS:   new Date("2024-01-02")
来源：http://epz.gotoacloud.top

Java: LocalDate.parse("2024-01-02")
来源：http://owd.xingfuxueyuan.xyz

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hmp.sjlbkw.cn

Ruby: Date.parse("2024-01-02")
来源：http://rkm.zhengqikj.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://tpi.andypj.xyz

[J04] 时间戳与日期互转
来源：http://cli.zhixingplan.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://okx.yangfankeji.com

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://stf.hfpthk.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://fwa.pengpengdd.cyou

TS:   Math.floor(Date.now() / 1000)
来源：http://bhl.cucudq.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://pxn.jlsjyb.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://pbp.zycfv.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://zgq.yongpay.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://agj.ydjk.org.cn

[J05] 时间加减（加 7 天）
来源：http://cdj.yj20258.top

Py:   now + timedelta(days=7)
来源：http://jfe.wangdashe.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://kas.hysaishi.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://fzi.dianchejie.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://nho.yuanzhike.top

Java: LocalDate.now().plusDays(7)
来源：http://kiz.nanxinkj.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://xyg.cqqwz.cn

Ruby: Time.now + 7 * 86400
来源：http://qbj.fanxiaobao.xyz

C#:   DateTime.Now.AddDays(7)
来源：http://gim.xylfe.cn

[J06] 计算两时间之差
来源：http://nxd.sxryk.cn

Py:   (end - start).total_seconds()
来源：http://vfm.hywenlv.cn

PHP:  $end->diff($start)->days;
来源：http://eyl.hnqzz.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://vre.cashguo.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://epo.guannengcc.top

Java: Duration.between(start, end).toSeconds()
来源：http://udc.daria6918.cn

Go:   end.Sub(start).Hours()
来源：http://duc.vehdjk.com

Ruby: end - start                 # 返回秒数
来源：http://iot.guowangkeji.top

C#:   (end - start).TotalSeconds
来源：http://dtt.ydjk.org.cn

[J07] 比较两个日期
来源：http://fqo.jinqigfzy.top

Py:   d1 < d2;  d1 == d2
来源：http://uqr.gogol.net.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://lgi.yongpay.top

JS:   d1.getTime() < d2.getTime()
来源：http://vhd.havefunace.top

TS:   d1.getTime() < d2.getTime()
来源：http://akr.feifeiyinyue.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://pvq.fktsv.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ioy.nanxinkj.top

Ruby: d1 < d2;  d1 == d2
来源：http://qmy.zhaomingkeji.xyz

C#:   d1 < d2;  d1 == d2
来源：http://fux.fanxiaobao.xyz

[J08] 提取年月日与星期
来源：http://lml.wangdashe.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://axc.nanxuanxn.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://nxl.hnqzz.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://xew.birdmap.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://lia.zhaomingkeji.xyz

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://rad.epnwcf.com

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://apw.shzxlz.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://fvm.fktsv.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ubv.snrcjt.cn

[J09] 时区处理
来源：http://nag.ivvv.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://nba.sjlbkw.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://art.chenzaomai.com

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://odt.jinqigfzy.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baq.hywenlv.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://pfx.zhijiandao.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://coy.yangfankeji.com

Ruby: Time.now.getlocal("+08:00")
来源：http://mjb.zhengqikj.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ulb.cqqwz.cn

[J10] 取今天 / 本月第一天
来源：http://bzb.fzhhl.top

Py:   date.today();  date.today().replace(day=1)
来源：http://nlt.bjfxy.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://bmd.xylfe.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://awj.nanxinkj.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://lra.0kj1m.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://aez.bbcook.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://jdq.redwolf501.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://huk.fehbvm.com

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://uvf.xingfuxueyuan.xyz

================================================================================
来源：http://xmh.cdnleiting.top

K. JSON 与序列化
来源：http://mmb.wangdashe.top

================================================================================
来源：http://wax.andypj.xyz

[K01] 对象转 JSON 字符串
来源：http://jtr.hammf.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://yfr.hywenlv.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://izm.sysykeji.top

JS:   JSON.stringify(obj)
来源：http://zff.aibaodan.cn

TS:   JSON.stringify(obj)
来源：http://hga.daxiang520.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://rrd.sweek.top

Go:   json.Marshal(obj)
来源：http://mrg.fzhhl.top

Ruby: obj.to_json                                     // require "json"
来源：http://rwv.jianghu66.top

C#:   JsonSerializer.Serialize(obj)
来源：http://tyz.smart0.xyz

[K02] JSON 字符串转对象
来源：http://lsy.jinyuanbaomall.cn

Py:   json.loads(s)
来源：http://ior.nanxuanxn.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://uxk.mhx1999.top

JS:   JSON.parse(s)
来源：http://nxs.zhengqikj.top

TS:   JSON.parse(s)
来源：http://mzb.dashuyun.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://vmj.jinyuanbaomall.cn

Go:   json.Unmarshal(data, &v)
来源：http://atg.mhx1999.top

Ruby: JSON.parse(s)
来源：http://uat.fktsv.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ddv.jqgfzy.top

[K03] JSON 美化输出（带缩进）
来源：http://ilm.jianghu66.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://bce.sweek.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://evr.jqgfzy.top

JS:   JSON.stringify(obj, null, 2)
来源：http://jel.xziqi.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://mne.chenzaomai.com

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://jow.sxryk.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://kqf.aibaodan.cn

Ruby: JSON.pretty_generate(obj)
来源：http://aqn.jinqigufen.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://efv.ivvv.top

[K04] 读取 JSON 文件
来源：http://gmh.yonumen.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://kru.jiagoushi.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://xtr.xziqi.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://bim.cucudq.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://grc.xuetiantiany.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://cup.52xcode.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wff.jiagoushi.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://fgk.chenjidiqi.icu

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://euq.yfazqb.com

[K05] 深拷贝对象
来源：http://qhw.jianghu66.top

Py:   copy.deepcopy(obj)
来源：http://smv.jiagoushi.top

PHP:  unserialize(serialize($obj));
来源：http://mar.birdmap.top

JS:   structuredClone(obj)
来源：http://zjr.wangshuangyany.cn

TS:   structuredClone(obj)
来源：http://sgs.ivvv.top

Java: // 手写拷贝构造，或序列化往返
来源：http://aqb.yuanzhike.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://oek.shuidangran.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://fpx.yuxming.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://cue.yuanzhike.top

[K06] 解析 URL 查询串
来源：http://env.sweek.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://svp.kuanghao11.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://kym.fengsongda.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://xzz.mhx1999.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://tks.ctjpmb.com

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://lgw.meibo888.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://mha.fengsongda.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://djt.yfazqb.com

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://awr.cqqwz.cn

[K07] 进制转换
来源：http://thf.ctjpmb.com

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://rns.zdqjudy.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://fsl.fengsongda.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://lav.cdnleiting.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wqk.cqqwz.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://uzx.hfpthk.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://gqc.yj202588.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://lao.0kj1m.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://xzp.zdbjq.cn

[K08] 二进制序列化（非 JSON）
来源：http://mry.hnqzz.top

Py:   pickle.dumps(obj)
来源：http://rto.yfazqb.com

PHP:  serialize($obj);  unserialize($s);
来源：http://nsh.jinqigufen.top

JS:   v8.serialize(obj)        // Node
来源：http://dng.xuetiantiany.cn

TS:   v8.serialize(obj)        // Node
来源：http://pnt.yuanzhike.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://orz.jqgfzy.top

Go:   encoding/gob
来源：http://ewv.shzxlz.cn

Ruby: Marshal.dump(obj)
来源：http://roa.hnqzz.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://dan.yj202588.top

================================================================================
来源：http://qod.tian-w.cn

L. 网络请求
来源：http://uze.xingfuxueyuan.xyz

================================================================================
来源：http://dbh.yanxiufei.cn

[L01] 发送 GET 请求
来源：http://btv.jqgfzy.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://xfm.yongpay.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://fqo.jianghu66.top

JS:   await fetch(url)
来源：http://zlo.xuanzx.com

TS:   await fetch(url)
来源：http://jre.haohaochexian.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://qwy.jinqigufen.top

Go:   resp, err := http.Get(url)
来源：http://hev.ppjwa.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://wkq.tarul.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://gwh.vqdsnc.cn

[L02] 发送 POST JSON
来源：http://fwp.aibaodan.cn

Py:   requests.post(url, json={"a": 1})
来源：http://rxb.feifeiyinyue.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://nnh.ehwqpu.com

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://tpw.zycfv.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://lom.fktsv.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ovc.havefunace.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ftt.ivvv.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://oct.sweek.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mpv.yangfankeji.com

[L03] 设置自定义请求头
来源：http://ejq.feifeiyinyue.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://aho.birdmap.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://srr.hnqzz.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://bve.havefunace.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://zel.sxryk.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://igu.jyoumei.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://fkh.uphjek.com

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://adb.52xcode.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ryk.bjfxy.top

[L04] 设置超时
来源：http://qth.feifeiyinyue.top

Py:   requests.get(url, timeout=5)
来源：http://vdp.ctjpmb.com

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://kdf.nanxuanxn.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://onh.sxryk.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://uyy.yj202588.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://psm.yj20258888.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://nsc.pengpengdd.cyou

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://xeq.snrcjt.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://uvo.fktsv.cn

[L05] 上传文件（multipart）
来源：http://mun.ivvv.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://isn.tianlin.xyz

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://evp.jinqigufen.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://gmi.zhongyouzk.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://xey.redwolf501.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://jxj.yueranfly.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://gqd.dashuyun.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://vda.hcnkem.com

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://aye.snrcjt.cn

[L06] 解析响应为 JSON
来源：http://tpz.zhiwuduotai.top

Py:   resp.json()
来源：http://mvp.yueranfly.top

PHP:  json_decode($body, true);
来源：http://pvh.nanxuanxn.top

JS:   await resp.json()
来源：http://jtl.ppjwa.cn

TS:   await resp.json()
来源：http://kse.hnqzz.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://zar.hfpthk.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://dkt.zhixingplan.top

Ruby: JSON.parse(resp.body)
来源：http://chs.ctjpmb.com

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://jur.cucudq.cn

[L07] 处理 HTTP 状态码
来源：http://yve.0kj1m.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ngm.gaohongyu789.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://pdw.hongshengwenyu.top

JS:   resp.ok;  resp.status
来源：http://zdj.nwbrower.top

TS:   resp.ok;  resp.status
来源：http://pyq.kuanghao11.cn

Java: resp.statusCode()
来源：http://gdq.shzxlz.cn

Go:   resp.StatusCode
来源：http://caf.yongpay.top

Ruby: resp.code.to_i
来源：http://bmb.tianlin.xyz

C#:   (int)resp.StatusCode
来源：http://urk.redwolf501.top

[L08] 并发请求多个地址
来源：http://duc.svipenyu.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://yxq.hammf.cn

PHP:  curl_multi_init() 系列
来源：http://pmb.jqgfzy.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ahl.bjfxy.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://byu.xinyue.icu

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://yfx.c1oappe.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://rwb.zhaomingkeji.xyz

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://fzd.gzhubu.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ghm.xinyue.icu

================================================================================
来源：http://sxf.jlsjyb.cn

M. 命令行 / 进程 / 环境
来源：http://dlj.zhongyouzk.top

================================================================================
来源：http://mrn.xuetiantiany.cn

[M01] 读取命令行参数
来源：http://fil.hysaishi.cn

Py:   sys.argv[1:]
来源：http://vzz.jinyuanbaomall.cn

PHP:  $argv;  $argc;
来源：http://tlm.fktsv.cn

JS:   process.argv.slice(2)
来源：http://ejf.fehbvm.com

TS:   process.argv.slice(2)
来源：http://udw.feifeiyinyue.top

Java: args 数组（main 方法参数）
来源：http://ajy.aibaodan.cn

Go:   os.Args[1:]
来源：http://jzs.xingfuxueyuan.xyz

Ruby: ARGV
来源：http://pec.shanyushiyangkeji.top

C#:   args 数组（Main 方法参数）
来源：http://bia.shangyingyoupin.top

[M02] 读取环境变量
来源：http://twy.sxryk.cn

Py:   os.environ.get("HOME")
来源：http://jdn.cucudq.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://iyl.shangyingyoupin.top

JS:   process.env.HOME
来源：http://hxo.xuetiantiany.cn

TS:   process.env.HOME
来源：http://kcn.uphjek.com

Java: System.getenv("HOME")
来源：http://ipy.gzhubu.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://rgh.tian-w.cn

Ruby: ENV["HOME"]
来源：http://xze.andypj.xyz

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://vck.jianghu66.top

[M03] 执行外部命令
来源：http://ecb.gaohongyu789.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://nsv.c1oappe.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ckh.jinqigufen.top

JS:   child_process.execSync("ls -l").toString()
来源：http://xsa.havefunace.top

TS:   child_process.execSync("ls -l").toString()
来源：http://vct.birdmap.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://kok.ppjwa.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://cpi.cucudq.cn

Ruby: system("ls -l");  `ls -l`
来源：http://shn.zycfv.cn

C#:   Process.Start("ls", "-l");
来源：http://fxf.wangshuangyany.cn

[M04] 获取当前工作目录
来源：http://gmz.uphjek.com

Py:   os.getcwd()
来源：http://ybi.snrcjt.cn

PHP:  getcwd();
来源：http://cur.sysykeji.top

JS:   process.cwd()
来源：http://zet.havefunace.top

TS:   process.cwd()
来源：http://bus.vehdjk.com

Java: Path.of("").toAbsolutePath()
来源：http://ysh.gotoacloud.top

Go:   os.Getwd()
来源：http://knn.nanxuanxn.top

Ruby: Dir.pwd
来源：http://swd.nanxuanxn.top

C#:   Directory.GetCurrentDirectory()
来源：http://kgd.yj20258888.top

[M05] 设置退出码
来源：http://kut.shzxlz.cn

Py:   sys.exit(1)
来源：http://lzk.dianchejie.cn

PHP:  exit(1);
来源：http://eve.jlsjyb.cn

JS:   process.exit(1)
来源：http://vbc.birdmap.top

TS:   process.exit(1)
来源：http://qii.hfpthk.cn

Java: System.exit(1)
来源：http://yfn.kuanghao11.cn

Go:   os.Exit(1)
来源：http://lpb.cucudq.cn

Ruby: exit 1
来源：http://daz.svipenyu.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://cks.xingfuxueyuan.xyz

[M06] 向标准错误输出
来源：http://onu.yj20258.top

Py:   print("err", file=sys.stderr)
来源：http://xmm.ybcxt.top

PHP:  fwrite(STDERR, "err\n");
来源：http://bhb.cqqwz.cn

JS:   console.error("err")
来源：http://kit.uphjek.com

TS:   console.error("err")
来源：http://mjq.fanxiaobao.xyz

Java: System.err.println("err")
来源：http://mef.ivvv.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://kav.xuetiantiany.cn

Ruby: warn "err"
来源：http://uhz.yvedp.cn

C#:   Console.Error.WriteLine("err")
来源：http://gyu.hcnkem.com

[M07] 判断是否为主入口
来源：http://qsh.9152youxi.cn

Py:   if __name__ == "__main__":
来源：http://apr.jlsjyb.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://rno.aibaodan.cn

JS:   require.main === module
来源：http://fln.yj20258888.top

TS:   require.main === module
来源：http://hil.jyoumei.cn

Java: public static void main(String[] args)
来源：http://eji.cdnleiting.top

Go:   func main()
来源：http://sog.fanxiaobao.xyz

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://gxr.xylfe.cn

C#:   static void Main(string[] args)
来源：http://rux.jyoumei.cn

[M08] 获取系统与运行时信息
来源：http://dhn.cheryme.top

Py:   platform.system();  platform.python_version()
来源：http://lah.yuxming.cn

PHP:  PHP_OS;  phpversion();
来源：http://gvc.feifeiyinyue.top

JS:   process.platform;  process.version
来源：http://vqv.jlsjyb.cn


<!-- 参考信息 -->