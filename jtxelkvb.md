代发 wailian999

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://abk.sjlbkw.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://vtw.wangshuangyany.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://kzn.jiagoushi.top

TS:   d.toISOString()
来源：http://qtx.cucudq.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://deq.zhiwuduotai.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://nuf.yuanzhike.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ods.yongpay.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://rcw.ybcxt.top

[J03] 字符串解析为日期
来源：http://eck.jinqigufen.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ypp.dianchejie.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://nht.jyoumei.cn

JS:   new Date("2024-01-02")
来源：http://fve.wangshuangyany.cn

TS:   new Date("2024-01-02")
来源：http://sep.zhoulong.xyz

Java: LocalDate.parse("2024-01-02")
来源：http://jrv.gotoacloud.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ach.zycfv.cn

Ruby: Date.parse("2024-01-02")
来源：http://drp.jyoumei.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://uyi.chenzaomai.com

[J04] 时间戳与日期互转
来源：http://dfq.pengpengdd.cyou

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://smo.xingfuxueyuan.xyz

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://scj.haohaochexian.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://kjp.ydjk.org.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://xcc.uphjek.com

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://qte.zdbjq.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://tnk.chenlongwang.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://acv.ybcxt.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://bcr.zdbjq.cn

[J05] 时间加减（加 7 天）
来源：http://jpm.yuxming.cn

Py:   now + timedelta(days=7)
来源：http://yhk.jlsjyb.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://lxr.andypj.xyz

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://rkt.quarkkingdee.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://fut.xingfuxueyuan.xyz

Java: LocalDate.now().plusDays(7)
来源：http://cfy.smart0.xyz

Go:   time.Now().AddDate(0, 0, 7)
来源：http://xdb.zdbjq.cn

Ruby: Time.now + 7 * 86400
来源：http://mdj.jinqigufen.top

C#:   DateTime.Now.AddDays(7)
来源：http://yvu.daxiang520.top

[J06] 计算两时间之差
来源：http://wki.xylfe.cn

Py:   (end - start).total_seconds()
来源：http://kke.ywan-chungtsiang.top

PHP:  $end->diff($start)->days;
来源：http://iwg.hywenlv.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://who.shuidangran.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://qlb.vqdsnc.cn

Java: Duration.between(start, end).toSeconds()
来源：http://qnx.ydjk.org.cn

Go:   end.Sub(start).Hours()
来源：http://osr.daria6918.cn

Ruby: end - start                 # 返回秒数
来源：http://gvn.gogol.net.cn

C#:   (end - start).TotalSeconds
来源：http://rtb.9152youxi.cn

[J07] 比较两个日期
来源：http://lvf.birdmap.top

Py:   d1 < d2;  d1 == d2
来源：http://mdh.wangshuangyany.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ljj.cashguo.top

JS:   d1.getTime() < d2.getTime()
来源：http://kaw.vqdsnc.cn

TS:   d1.getTime() < d2.getTime()
来源：http://bxk.wangshuangyany.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://bsh.ppjwa.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://wjz.hnxiangtu.top

Ruby: d1 < d2;  d1 == d2
来源：http://gir.ydzc1.top

C#:   d1 < d2;  d1 == d2
来源：http://cvb.yongpay.top

[J08] 提取年月日与星期
来源：http://sfp.jinghuilouyu.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://rfi.ehwqpu.com

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://jnn.chenjidiqi.icu

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://kdf.9152youxi.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://xkv.shuidangran.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://wrs.yangfankeji.com

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://zai.c1oappe.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://mvz.xingfuxueyuan.xyz

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://pif.hfpthk.cn

[J09] 时区处理
来源：http://hrt.snrcjt.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://prr.cashguo.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://mie.c1oappe.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://xys.kuanghao11.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wzx.yj20258.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://dqy.daria6918.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://yoa.hnxiangtu.top

Ruby: Time.now.getlocal("+08:00")
来源：http://tby.cheryme.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://mph.jqgfzy.top

[J10] 取今天 / 本月第一天
来源：http://lxi.jianghu66.top

Py:   date.today();  date.today().replace(day=1)
来源：http://jke.hywenlv.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://xvd.yonumen.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hjj.52xcode.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ngn.c1oappe.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://zas.ydzc1.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://zac.yangfankeji.com

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://teu.fzhhl.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://iwd.yj202588.top

================================================================================
来源：http://mgi.ydzc1.top

K. JSON 与序列化
来源：http://gpa.yvedp.cn

================================================================================
来源：http://hof.yfazqb.com

[K01] 对象转 JSON 字符串
来源：http://uyh.sysykeji.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://avl.sjlbkw.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://uvu.nanxinkj.top

JS:   JSON.stringify(obj)
来源：http://agp.shzxlz.cn

TS:   JSON.stringify(obj)
来源：http://evp.zhaomingkeji.xyz

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://iiz.bjfxy.top

Go:   json.Marshal(obj)
来源：http://xdi.tian-w.cn

Ruby: obj.to_json                                     // require "json"
来源：http://rpz.tarul.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://ivo.yfazqb.com

[K02] JSON 字符串转对象
来源：http://wbh.wangshuangyany.cn

Py:   json.loads(s)
来源：http://htx.yuanzhike.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://bvx.shangyingyoupin.top

JS:   JSON.parse(s)
来源：http://lhq.xziqi.cn

TS:   JSON.parse(s)
来源：http://zcz.xuanzx.com

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://wqj.haohaochexian.top

Go:   json.Unmarshal(data, &v)
来源：http://rqt.zhixingplan.top

Ruby: JSON.parse(s)
来源：http://qqa.gzhubu.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://jty.jinghuilouyu.cn

[K03] JSON 美化输出（带缩进）
来源：http://cet.xziqi.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://kbn.hcnkem.com

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ewm.ywan-chungtsiang.top

JS:   JSON.stringify(obj, null, 2)
来源：http://nwe.yueranfly.top

TS:   JSON.stringify(obj, null, 2)
来源：http://url.daxiang520.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://vas.aibaodan.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://qfz.yanxiufei.cn

Ruby: JSON.pretty_generate(obj)
来源：http://imw.yangfankeji.com

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://wjk.jinghuilouyu.cn

[K04] 读取 JSON 文件
来源：http://iry.pengpengdd.cyou

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ukf.yonumen.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://eek.52xcode.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://qug.andypj.xyz

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://lux.fktsv.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://clq.sjlbkw.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://mwf.shangyingyoupin.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://jsd.sjlbkw.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://rgu.xziqi.cn

[K05] 深拷贝对象
来源：http://hoq.redwolf501.top

Py:   copy.deepcopy(obj)
来源：http://dpu.jinghuilouyu.cn

PHP:  unserialize(serialize($obj));
来源：http://xzx.tanke756.top

JS:   structuredClone(obj)
来源：http://wlh.52xcode.cn

TS:   structuredClone(obj)
来源：http://gcc.cdnleiting.top

Java: // 手写拷贝构造，或序列化往返
来源：http://poj.sysykeji.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://psu.zycfv.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://qrp.zhijiandao.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://mrz.zhongyouzk.top

[K06] 解析 URL 查询串
来源：http://gtm.jlsjyb.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ndl.zhaomingkeji.xyz

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://fah.yj202588.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ald.quarkkingdee.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://fod.sweek.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://epy.0kj1m.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://dnf.yj20258888.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://tss.tanke756.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://vni.pengpengdd.cyou

[K07] 进制转换
来源：http://axe.xylfe.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://vfn.jinghuilouyu.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://faw.zhengqikj.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://kny.sjlbkw.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ajx.xuanzx.com

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://rza.zhoulong.xyz

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://jbz.jiagoushi.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://rez.sweek.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wxs.jyoumei.cn

[K08] 二进制序列化（非 JSON）
来源：http://wxj.yueranfly.top

Py:   pickle.dumps(obj)
来源：http://emw.yonumen.top

PHP:  serialize($obj);  unserialize($s);
来源：http://vpt.cashguo.top

JS:   v8.serialize(obj)        // Node
来源：http://jgv.xinyue.icu

TS:   v8.serialize(obj)        // Node
来源：http://twe.svipenyu.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://akt.yangfankeji.com

Go:   encoding/gob
来源：http://cuw.zhijiandao.cn

Ruby: Marshal.dump(obj)
来源：http://bxu.zycfv.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://gmn.zhiwuduotai.top

================================================================================
来源：http://vtp.ydzc1.top

L. 网络请求
来源：http://fxk.ppjwa.cn

================================================================================
来源：http://qoa.yfazqb.com

[L01] 发送 GET 请求
来源：http://dnt.cheryme.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://oaf.hesvh.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://spx.chenjidiqi.icu

JS:   await fetch(url)
来源：http://dyj.zdbjq.cn

TS:   await fetch(url)
来源：http://fxw.cqqwz.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hlm.shanyushiyangkeji.top

Go:   resp, err := http.Get(url)
来源：http://nax.guowangkeji.top

Ruby: Net::HTTP.get(URI(url))
来源：http://ldf.xziqi.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hxb.zdqjudy.top

[L02] 发送 POST JSON
来源：http://cmm.gotoacloud.top

Py:   requests.post(url, json={"a": 1})
来源：http://ngq.zdqjudy.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://pif.smart0.xyz

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://gdw.316326.xyz

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://gum.jinghuilouyu.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://aca.smart0.xyz

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://jkn.jiagoushi.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://dcq.chenzaomai.com

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://qjj.c1oappe.top

[L03] 设置自定义请求头
来源：http://llg.dashuyun.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://nby.xziqi.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://eof.jinghuilouyu.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wbz.zhaomingkeji.xyz

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://yfg.aibaodan.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://led.jinqigufen.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://gni.52xcode.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wei.xziqi.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mpd.yvedp.cn

[L04] 设置超时
来源：http://qcy.guowangkeji.top

Py:   requests.get(url, timeout=5)
来源：http://ros.mhx1999.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://npq.fengsongda.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ror.svipenyu.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ukc.jlsjyb.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://tjd.kuanghao11.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://cgm.aibaodan.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ryi.svipenyu.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://tft.zhoulong.xyz

[L05] 上传文件（multipart）
来源：http://fqs.gotoacloud.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://orn.jqgfzy.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hgq.yj202588.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://kng.yj20258888.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://inr.fanxiaobao.xyz

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ygp.cashguo.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://fpv.uphjek.com

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://vsy.birdmap.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://iqd.sweek.top

[L06] 解析响应为 JSON
来源：http://tvi.ybcxt.top

Py:   resp.json()
来源：http://ycm.ehwqpu.com

PHP:  json_decode($body, true);
来源：http://svl.jiagoushi.top

JS:   await resp.json()
来源：http://ato.zdqjudy.top

TS:   await resp.json()
来源：http://jmc.tanke756.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wtp.chenzaomai.com

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://sox.jlsjyb.cn

Ruby: JSON.parse(resp.body)
来源：http://mfp.gogol.net.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://qvv.hnqzz.top

[L07] 处理 HTTP 状态码
来源：http://nqu.tarul.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://rpw.sweek.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://gbm.nanxinkj.top

JS:   resp.ok;  resp.status
来源：http://dxm.andypj.xyz

TS:   resp.ok;  resp.status
来源：http://spc.fktsv.cn

Java: resp.statusCode()
来源：http://zzo.yuanzhike.top

Go:   resp.StatusCode
来源：http://pxb.ehwqpu.com

Ruby: resp.code.to_i
来源：http://iyo.chenjidiqi.icu

C#:   (int)resp.StatusCode
来源：http://axm.uphjek.com

[L08] 并发请求多个地址
来源：http://myk.wangshuangyany.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://bme.dianchejie.cn

PHP:  curl_multi_init() 系列
来源：http://hon.zhengqikj.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://poi.hywenlv.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mxv.yj202588.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://bkj.yanxiufei.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://zfq.0kj1m.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://fmn.svipenyu.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ake.jinqigfzy.top

================================================================================
来源：http://vof.shzxlz.cn

M. 命令行 / 进程 / 环境
来源：http://vgv.jianghu66.top

================================================================================
来源：http://iaw.wangdashe.top

[M01] 读取命令行参数
来源：http://dip.cqqwz.cn

Py:   sys.argv[1:]
来源：http://dwf.dianchejie.cn

PHP:  $argv;  $argc;
来源：http://ypy.cqqwz.cn

JS:   process.argv.slice(2)
来源：http://asc.9152youxi.cn

TS:   process.argv.slice(2)
来源：http://ydz.316326.xyz

Java: args 数组（main 方法参数）
来源：http://tci.hfpthk.cn

Go:   os.Args[1:]
来源：http://fao.yfazqb.com

Ruby: ARGV
来源：http://cwc.pengpengdd.cyou

C#:   args 数组（Main 方法参数）
来源：http://nnx.haohaochexian.top

[M02] 读取环境变量
来源：http://ihm.ybcxt.top

Py:   os.environ.get("HOME")
来源：http://ekq.pengpengdd.cyou

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://net.dianchejie.cn

JS:   process.env.HOME
来源：http://skf.nanxuanxn.top

TS:   process.env.HOME
来源：http://qiq.hnxiangtu.top

Java: System.getenv("HOME")
来源：http://knf.zhaomingkeji.xyz

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://uck.gogol.net.cn

Ruby: ENV["HOME"]
来源：http://tlt.yongpay.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://uxd.nwbrower.top

[M03] 执行外部命令
来源：http://spc.jiagoushi.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://sgm.hcnkem.com

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ljy.yangfankeji.com

JS:   child_process.execSync("ls -l").toString()
来源：http://dtr.hnxiangtu.top

TS:   child_process.execSync("ls -l").toString()
来源：http://brh.daxiang520.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://pgm.zdqjudy.top

Go:   exec.Command("ls", "-l").Output()
来源：http://kyd.zhijiandao.cn

Ruby: system("ls -l");  `ls -l`
来源：http://kdt.bbcook.cn

C#:   Process.Start("ls", "-l");
来源：http://qzw.jinqigfzy.top

[M04] 获取当前工作目录
来源：http://tvb.hywenlv.cn

Py:   os.getcwd()
来源：http://hpm.yanxiufei.cn

PHP:  getcwd();
来源：http://xcf.hnqzz.top

JS:   process.cwd()
来源：http://yaa.gogol.net.cn

TS:   process.cwd()
来源：http://irf.snrcjt.cn

Java: Path.of("").toAbsolutePath()
来源：http://zlr.andypj.xyz

Go:   os.Getwd()
来源：http://cbe.jinyuanbaomall.cn

Ruby: Dir.pwd
来源：http://whz.zdbjq.cn

C#:   Directory.GetCurrentDirectory()
来源：http://idz.mhx1999.top

[M05] 设置退出码
来源：http://yjl.yj202588.top

Py:   sys.exit(1)
来源：http://qpo.guannengcc.top

PHP:  exit(1);
来源：http://vyu.zhiwuduotai.top

JS:   process.exit(1)
来源：http://czp.zhixingplan.top

TS:   process.exit(1)
来源：http://rkw.bbcook.cn

Java: System.exit(1)
来源：http://uyk.smart0.xyz

Go:   os.Exit(1)
来源：http://vxp.fengsongda.top

Ruby: exit 1
来源：http://vce.hywenlv.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://cyi.kuanghao11.cn

[M06] 向标准错误输出
来源：http://hgk.yonumen.top

Py:   print("err", file=sys.stderr)
来源：http://yls.svipenyu.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://soy.tian-w.cn

JS:   console.error("err")
来源：http://qel.shanyushiyangkeji.top

TS:   console.error("err")
来源：http://pfl.aizwys.cn

Java: System.err.println("err")
来源：http://uba.dashuyun.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://dwj.fehbvm.com

Ruby: warn "err"
来源：http://qvz.daxiang520.top

C#:   Console.Error.WriteLine("err")
来源：http://ysm.epnwcf.com

[M07] 判断是否为主入口
来源：http://mcx.0kj1m.cn

Py:   if __name__ == "__main__":
来源：http://wtt.ydzc1.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://uok.cashguo.top

JS:   require.main === module
来源：http://cxx.sufxvd.cn

TS:   require.main === module
来源：http://vga.yuanzhike.top

Java: public static void main(String[] args)
来源：http://tje.pycfn.com

Go:   func main()
来源：http://iur.xingfuxueyuan.xyz

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://iov.mhx1999.top

C#:   static void Main(string[] args)
来源：http://pbx.epnwcf.com

[M08] 获取系统与运行时信息
来源：http://wfa.fktsv.cn

Py:   platform.system();  platform.python_version()
来源：http://slf.ywan-chungtsiang.top

PHP:  PHP_OS;  phpversion();
来源：http://gwn.zhixingplan.top

JS:   process.platform;  process.version
来源：http://phr.sysykeji.top


<!-- 参考信息 -->