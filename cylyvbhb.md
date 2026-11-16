代发 wailian999

Go:   time.Now()
来源：http://mme.chenzaomai.com

Ruby: Time.now
来源：http://zcz.fehbvm.com

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://bwu.jyoumei.cn

[J02] 格式化输出
来源：http://hqv.aizwys.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://qas.quarkkingdee.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://szh.yueranfly.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://eqy.smart0.xyz

TS:   d.toISOString()
来源：http://cna.sysykeji.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://jyk.9152youxi.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://amc.bjfxy.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wib.jiagoushi.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://bmc.zhixingplan.top

[J03] 字符串解析为日期
来源：http://xid.pengpengdd.cyou

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://mxc.dianchejie.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://inf.smart0.xyz

JS:   new Date("2024-01-02")
来源：http://eed.sufxvd.cn

TS:   new Date("2024-01-02")
来源：http://aec.ybcxt.top

Java: LocalDate.parse("2024-01-02")
来源：http://kue.zdqjudy.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://dqe.cucudq.cn

Ruby: Date.parse("2024-01-02")
来源：http://zdi.ivvv.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://avg.hysaishi.cn

[J04] 时间戳与日期互转
来源：http://hvb.shuidangran.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://shb.yanxiufei.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://lkx.zhaomingkeji.xyz

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ray.zhoulong.xyz

TS:   Math.floor(Date.now() / 1000)
来源：http://pbb.hongshengwenyu.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ksy.yfazqb.com

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://gev.redwolf501.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hpv.gotoacloud.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://znq.ppjwa.cn

[J05] 时间加减（加 7 天）
来源：http://vup.yongpay.top

Py:   now + timedelta(days=7)
来源：http://mic.wangdashe.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://sed.daxiang520.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://csu.nwbrower.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://niu.sxryk.cn

Java: LocalDate.now().plusDays(7)
来源：http://kgp.c1oappe.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hlb.hongshengwenyu.top

Ruby: Time.now + 7 * 86400
来源：http://ksn.wangshuangyany.cn

C#:   DateTime.Now.AddDays(7)
来源：http://qch.guowangkeji.top

[J06] 计算两时间之差
来源：http://ttf.uphjek.com

Py:   (end - start).total_seconds()
来源：http://viu.hcnkem.com

PHP:  $end->diff($start)->days;
来源：http://xix.smart0.xyz

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://dou.xuanzx.com

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://qje.feifeiyinyue.top

Java: Duration.between(start, end).toSeconds()
来源：http://znc.ydzc1.top

Go:   end.Sub(start).Hours()
来源：http://fsl.shangyingyoupin.top

Ruby: end - start                 # 返回秒数
来源：http://fnw.jinqigufen.top

C#:   (end - start).TotalSeconds
来源：http://dal.yj20258888.top

[J07] 比较两个日期
来源：http://qbj.yfazqb.com

Py:   d1 < d2;  d1 == d2
来源：http://hhq.tarul.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://vun.ehwqpu.com

JS:   d1.getTime() < d2.getTime()
来源：http://bng.nwbrower.top

TS:   d1.getTime() < d2.getTime()
来源：http://mxn.epnwcf.com

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hbz.tian-w.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://vuv.yfazqb.com

Ruby: d1 < d2;  d1 == d2
来源：http://hnq.gaohongyu789.top

C#:   d1 < d2;  d1 == d2
来源：http://uku.tianlin.xyz

[J08] 提取年月日与星期
来源：http://obm.gogol.net.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://djt.redwolf501.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ylw.zhixingplan.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://inu.xuanzx.com

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://rwe.daxiang520.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://dxk.yj20258.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://juk.jinyuanbaomall.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://sna.xziqi.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://voe.yuanzhike.top

[J09] 时区处理
来源：http://irw.chenjidiqi.icu

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://fvv.havefunace.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://mms.yj20258888.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://yca.cheryme.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hgy.xylfe.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ppt.zhixingplan.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://zhz.yonumen.top

Ruby: Time.now.getlocal("+08:00")
来源：http://tqv.cdnleiting.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://khd.chenjidiqi.icu

[J10] 取今天 / 本月第一天
来源：http://wom.fzhhl.top

Py:   date.today();  date.today().replace(day=1)
来源：http://vid.jinyuanbaomall.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://usu.hcnkem.com

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://qvn.bjfxy.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://jhy.jinyuanbaomall.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://sue.dashuyun.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://brh.hesvh.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://gpo.bjfxy.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hgn.shanyushiyangkeji.top

================================================================================
来源：http://bah.hammf.cn

K. JSON 与序列化
来源：http://fuw.chenzaomai.com

================================================================================
来源：http://wxg.yj20258.top

[K01] 对象转 JSON 字符串
来源：http://pbg.yj20258.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://add.ybcxt.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://crj.hywenlv.cn

JS:   JSON.stringify(obj)
来源：http://xqp.nanxuanxn.top

TS:   JSON.stringify(obj)
来源：http://lux.xziqi.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://urv.cheryme.top

Go:   json.Marshal(obj)
来源：http://iyq.yuanzhike.top

Ruby: obj.to_json                                     // require "json"
来源：http://wzf.jinyuanbaomall.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://gfp.ydjk.org.cn

[K02] JSON 字符串转对象
来源：http://mrk.cqqwz.cn

Py:   json.loads(s)
来源：http://ojn.dashuyun.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://nnk.xziqi.cn

JS:   JSON.parse(s)
来源：http://ovw.zhongyouzk.top

TS:   JSON.parse(s)
来源：http://omn.yonumen.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://yhp.shanyushiyangtech.top

Go:   json.Unmarshal(data, &v)
来源：http://vsc.jinqigufen.top

Ruby: JSON.parse(s)
来源：http://wxy.tanke756.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://wux.fehbvm.com

[K03] JSON 美化输出（带缩进）
来源：http://gzy.hysaishi.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://vmy.yj20258.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://eug.dashuyun.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://ybq.epnwcf.com

TS:   JSON.stringify(obj, null, 2)
来源：http://fbo.zhongyouzk.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://exi.yueranfly.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://xom.9152youxi.cn

Ruby: JSON.pretty_generate(obj)
来源：http://xig.yuanzhike.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://edo.yangfankeji.com

[K04] 读取 JSON 文件
来源：http://llo.vqdsnc.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://gcb.ydzc1.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://eki.yuanzhike.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://vzy.ydzc1.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://zwa.yueranfly.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://uvx.xingfuxueyuan.xyz

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://pur.nanxuanxn.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://isd.daria6918.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wrh.birdmap.top

[K05] 深拷贝对象
来源：http://yfx.meibo888.top

Py:   copy.deepcopy(obj)
来源：http://efb.daxiang520.top

PHP:  unserialize(serialize($obj));
来源：http://psg.hfpthk.cn

JS:   structuredClone(obj)
来源：http://nqp.ivvv.top

TS:   structuredClone(obj)
来源：http://cwt.quarkkingdee.top

Java: // 手写拷贝构造，或序列化往返
来源：http://pmw.shangyingyoupin.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ncu.uphjek.com

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://obc.bjfxy.top

C#:   // 序列化往返，或自定义 Clone
来源：http://tik.xinyue.icu

[K06] 解析 URL 查询串
来源：http://sfz.yfazqb.com

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://tmg.guannengcc.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://tsw.ivvv.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://gnp.hfpthk.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://jot.sufxvd.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://clv.guannengcc.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://xmh.shanyushiyangtech.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://blg.cashguo.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://zvy.mhx1999.top

[K07] 进制转换
来源：http://cyx.ehwqpu.com

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://tqc.hammf.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://kqr.nanxinkj.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://fcp.ydjk.org.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://jac.daria6918.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://cwe.316326.xyz

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ssc.dashuyun.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://gve.yuxming.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://sbq.epnwcf.com

[K08] 二进制序列化（非 JSON）
来源：http://mfy.yanxiufei.cn

Py:   pickle.dumps(obj)
来源：http://kax.daxiang520.top

PHP:  serialize($obj);  unserialize($s);
来源：http://ayo.shzxlz.cn

JS:   v8.serialize(obj)        // Node
来源：http://wul.uphjek.com

TS:   v8.serialize(obj)        // Node
来源：http://avm.nanxuanxn.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://byy.bjfxy.top

Go:   encoding/gob
来源：http://fml.shanyushiyangkeji.top

Ruby: Marshal.dump(obj)
来源：http://yas.yangfankeji.com

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ogi.fehbvm.com

================================================================================
来源：http://pvo.ppjwa.cn

L. 网络请求
来源：http://mye.guowangkeji.top

================================================================================
来源：http://cpm.guannengcc.top

[L01] 发送 GET 请求
来源：http://zco.pengpengdd.cyou

Py:   requests.get(url)                        # 第三方库 requests
来源：http://yan.hnxiangtu.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://gcs.sweek.top

JS:   await fetch(url)
来源：http://xoy.fengsongda.top

TS:   await fetch(url)
来源：http://ogo.yj20258.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://tql.nanxinkj.top

Go:   resp, err := http.Get(url)
来源：http://swj.9152youxi.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://jfx.shanyushiyangkeji.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://jhu.ydzc1.top

[L02] 发送 POST JSON
来源：http://oic.birdmap.top

Py:   requests.post(url, json={"a": 1})
来源：http://mtj.sysykeji.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://deu.zhaomingkeji.xyz

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://vrk.aibaodan.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://grd.fanxiaobao.xyz

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://okb.tian-w.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://yns.uphjek.com

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://pvr.daxiang520.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://dka.jinqigufen.top

[L03] 设置自定义请求头
来源：http://nib.sufxvd.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://rcm.hnqzz.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://cnn.gotoacloud.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://vxi.zhixingplan.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://chu.hfpthk.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://zyq.guannengcc.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://zqc.shanyushiyangtech.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ize.birdmap.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://dud.jinqigfzy.top

[L04] 设置超时
来源：http://oft.sxryk.cn

Py:   requests.get(url, timeout=5)
来源：http://nwa.hnxiangtu.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://yki.chenjidiqi.icu

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ngz.yuanzhike.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://rzk.zhiwuduotai.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://alc.yuxming.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://pss.xuetiantiany.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://bbv.aizwys.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://rmh.cashguo.top

[L05] 上传文件（multipart）
来源：http://keg.aibaodan.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://cbw.yueranfly.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://cpu.smart0.xyz

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://juy.cqqwz.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://eud.zhoulong.xyz

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hlt.ybcxt.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://jba.shanyushiyangkeji.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://opl.chenjidiqi.icu

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://bpc.dianchejie.cn

[L06] 解析响应为 JSON
来源：http://szc.chenjidiqi.icu

Py:   resp.json()
来源：http://zlm.hnqzz.top

PHP:  json_decode($body, true);
来源：http://ieg.tian-w.cn

JS:   await resp.json()
来源：http://vuc.guowangkeji.top

TS:   await resp.json()
来源：http://sdj.yuxming.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mwf.gaohongyu789.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://que.fengsongda.top

Ruby: JSON.parse(resp.body)
来源：http://ffs.fanxiaobao.xyz

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ybo.yanxiufei.cn

[L07] 处理 HTTP 状态码
来源：http://oul.shuidangran.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://qlg.tarul.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://qji.havefunace.top

JS:   resp.ok;  resp.status
来源：http://rcx.yvedp.cn

TS:   resp.ok;  resp.status
来源：http://fyg.gogol.net.cn

Java: resp.statusCode()
来源：http://fxb.tianlin.xyz

Go:   resp.StatusCode
来源：http://qhd.ydjk.org.cn

Ruby: resp.code.to_i
来源：http://iow.epnwcf.com

C#:   (int)resp.StatusCode
来源：http://neh.sjlbkw.cn

[L08] 并发请求多个地址
来源：http://vjb.tianlin.xyz

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://dve.hnqzz.top

PHP:  curl_multi_init() 系列
来源：http://gif.tanke756.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://kha.gotoacloud.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://jaa.hammf.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ihu.zhiwuduotai.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://war.kuanghao11.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://boz.0kj1m.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mcc.tanke756.top

================================================================================
来源：http://bqh.hcnkem.com

M. 命令行 / 进程 / 环境
来源：http://rkc.quarkkingdee.top

================================================================================
来源：http://mcf.xuetiantiany.cn

[M01] 读取命令行参数
来源：http://zjr.hammf.cn

Py:   sys.argv[1:]
来源：http://krz.hnxiangtu.top

PHP:  $argv;  $argc;
来源：http://dvg.9152youxi.cn

JS:   process.argv.slice(2)
来源：http://snu.tian-w.cn

TS:   process.argv.slice(2)
来源：http://lbq.haohaochexian.top

Java: args 数组（main 方法参数）
来源：http://exi.sweek.top

Go:   os.Args[1:]
来源：http://vdu.fengsongda.top

Ruby: ARGV
来源：http://lwu.tian-w.cn

C#:   args 数组（Main 方法参数）
来源：http://ldi.cdnleiting.top

[M02] 读取环境变量
来源：http://sgo.yvedp.cn

Py:   os.environ.get("HOME")
来源：http://tzx.nwbrower.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://yex.bjfxy.top

JS:   process.env.HOME
来源：http://egp.xylfe.cn

TS:   process.env.HOME
来源：http://wmh.ydzc1.top

Java: System.getenv("HOME")
来源：http://mpr.jinghuilouyu.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://diq.sjlbkw.cn

Ruby: ENV["HOME"]
来源：http://ikf.meibo888.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ujo.jinghuilouyu.cn

[M03] 执行外部命令
来源：http://hcl.cheryme.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://kdv.smart0.xyz

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://zrg.shanyushiyangkeji.top

JS:   child_process.execSync("ls -l").toString()
来源：http://ztc.tianlin.xyz

TS:   child_process.execSync("ls -l").toString()
来源：http://xhj.iojbl.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://xqv.tarul.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://wbm.sjlbkw.cn

Ruby: system("ls -l");  `ls -l`
来源：http://rdo.jiagoushi.top

C#:   Process.Start("ls", "-l");
来源：http://oxu.dianchejie.cn

[M04] 获取当前工作目录
来源：http://ilr.zhengqikj.top

Py:   os.getcwd()
来源：http://sjt.jqgfzy.top

PHP:  getcwd();
来源：http://zlu.hammf.cn

JS:   process.cwd()
来源：http://wqy.daria6918.cn

TS:   process.cwd()
来源：http://ivr.dashuyun.cn

Java: Path.of("").toAbsolutePath()
来源：http://byk.guowangkeji.top

Go:   os.Getwd()
来源：http://ejd.gzhubu.top

Ruby: Dir.pwd
来源：http://utb.meibo888.top

C#:   Directory.GetCurrentDirectory()
来源：http://nvj.52xcode.cn

[M05] 设置退出码
来源：http://jbp.andypj.xyz

Py:   sys.exit(1)
来源：http://fty.xinyue.icu

PHP:  exit(1);
来源：http://izl.epnwcf.com

JS:   process.exit(1)
来源：http://wki.sysykeji.top

TS:   process.exit(1)
来源：http://mnt.xuanzx.com

Java: System.exit(1)
来源：http://bys.fzhhl.top

Go:   os.Exit(1)
来源：http://otg.xingfuxueyuan.xyz

Ruby: exit 1
来源：http://guz.yj20258888.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://eiv.redwolf501.top

[M06] 向标准错误输出
来源：http://wtq.meibo888.top

Py:   print("err", file=sys.stderr)
来源：http://uzr.bjfxy.top

PHP:  fwrite(STDERR, "err\n");
来源：http://igp.nwbrower.top

JS:   console.error("err")
来源：http://qlq.yj20258888.top

TS:   console.error("err")
来源：http://zzt.ctjpmb.com

Java: System.err.println("err")
来源：http://cmb.jqgufenzy.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wfb.tanke756.top

Ruby: warn "err"
来源：http://luj.aizwys.cn

C#:   Console.Error.WriteLine("err")
来源：http://msl.yuanzhike.top

[M07] 判断是否为主入口
来源：http://iws.ehwqpu.com

Py:   if __name__ == "__main__":
来源：http://qzs.yj202588.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://tjf.cashguo.top

JS:   require.main === module
来源：http://apr.shanyushiyangkeji.top

TS:   require.main === module
来源：http://uxv.9152youxi.cn

Java: public static void main(String[] args)
来源：http://egw.yj20258.top

Go:   func main()
来源：http://mty.ydjk.org.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wai.chenlongwang.top

C#:   static void Main(string[] args)
来源：http://xxk.ppjwa.cn


<!-- 参考信息 -->