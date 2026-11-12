代发 wailian999

J. 日期与时间
来源：http://zme.0kj1m.cn

================================================================================
来源：http://yhi.hcnkem.com

[J01] 获取当前时间
来源：http://uks.yuxming.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://vhm.zhixingplan.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://wyo.mhx1999.top

JS:   new Date();  Date.now()
来源：http://gqg.yuxming.cn

TS:   new Date();  Date.now()
来源：http://qmm.daria6918.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://iqd.yangfankeji.com

Go:   time.Now()
来源：http://zlv.sweek.top

Ruby: Time.now
来源：http://sfu.ydzc1.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ail.fktsv.cn

[J02] 格式化输出
来源：http://cin.0kj1m.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hfq.shangyingyoupin.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://xyn.ydzc1.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://lsk.316326.xyz

TS:   d.toISOString()
来源：http://zyk.jianghu66.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://zaq.yueranfly.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://vrt.kuanghao11.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://vuj.quarkkingdee.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://pdr.mhx1999.top

[J03] 字符串解析为日期
来源：http://rod.bbcook.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://gsi.zhongyouzk.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://sel.yj20258.top

JS:   new Date("2024-01-02")
来源：http://dmx.zdbjq.cn

TS:   new Date("2024-01-02")
来源：http://spr.hesvh.cn

Java: LocalDate.parse("2024-01-02")
来源：http://uoh.zhaomingkeji.xyz

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://msd.hammf.cn

Ruby: Date.parse("2024-01-02")
来源：http://wrg.sweek.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://mas.zhongyouzk.top

[J04] 时间戳与日期互转
来源：http://uyp.uphjek.com

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://egg.xuetiantiany.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://tlv.cheryme.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://zcj.zhijiandao.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://ssr.c1oappe.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://lrv.shuidangran.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://now.ppjwa.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://xcv.cdnleiting.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://eea.zycfv.cn

[J05] 时间加减（加 7 天）
来源：http://jhv.vqdsnc.cn

Py:   now + timedelta(days=7)
来源：http://xij.yj202588.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://tnn.yongpay.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://enw.shzxlz.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ujy.andypj.xyz

Java: LocalDate.now().plusDays(7)
来源：http://gac.snrcjt.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://nsp.zycfv.cn

Ruby: Time.now + 7 * 86400
来源：http://vwa.pengpengdd.cyou

C#:   DateTime.Now.AddDays(7)
来源：http://jsa.aibaodan.cn

[J06] 计算两时间之差
来源：http://omg.xuetiantiany.cn

Py:   (end - start).total_seconds()
来源：http://hwb.xuanzx.com

PHP:  $end->diff($start)->days;
来源：http://xey.yanxiufei.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://dxi.hongshengwenyu.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ctz.yanxiufei.cn

Java: Duration.between(start, end).toSeconds()
来源：http://bdo.xylfe.cn

Go:   end.Sub(start).Hours()
来源：http://zfa.kuanghao11.cn

Ruby: end - start                 # 返回秒数
来源：http://hvy.jiagoushi.top

C#:   (end - start).TotalSeconds
来源：http://lrn.aizwys.cn

[J07] 比较两个日期
来源：http://osr.jinghuilouyu.cn

Py:   d1 < d2;  d1 == d2
来源：http://avv.zhongyouzk.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://wca.jiagoushi.top

JS:   d1.getTime() < d2.getTime()
来源：http://onr.aibaodan.cn

TS:   d1.getTime() < d2.getTime()
来源：http://vtt.jqgufenzy.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://pge.vehdjk.com

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://dzu.sufxvd.cn

Ruby: d1 < d2;  d1 == d2
来源：http://fyj.hesvh.cn

C#:   d1 < d2;  d1 == d2
来源：http://sxl.zhiwuduotai.top

[J08] 提取年月日与星期
来源：http://euy.yonumen.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://rvu.pycfn.com

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://pzv.cashguo.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://zeu.ctjpmb.com

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://khy.dashuyun.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://lts.epnwcf.com

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://bme.redwolf501.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://xgl.xingfuxueyuan.xyz

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://mar.hesvh.cn

[J09] 时区处理
来源：http://ibm.hnxiangtu.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://pdn.havefunace.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://xmo.dashuyun.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://uul.ybcxt.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://yyp.jianghu66.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://uah.ctjpmb.com

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://qyj.meibo888.top

Ruby: Time.now.getlocal("+08:00")
来源：http://psp.gzhubu.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://obw.yanxiufei.cn

[J10] 取今天 / 本月第一天
来源：http://zft.xylfe.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://axj.jlsjyb.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ssx.shuidangran.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://cce.quarkkingdee.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ths.guannengcc.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://bog.daria6918.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://yoi.yfazqb.com

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://oox.hysaishi.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://eut.zhoulong.xyz

================================================================================
来源：http://vrm.jinghuilouyu.cn

K. JSON 与序列化
来源：http://gmc.yfazqb.com

================================================================================
来源：http://ibx.dashuyun.cn

[K01] 对象转 JSON 字符串
来源：http://vbb.hnxiangtu.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://cvw.ehwqpu.com

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://pak.xuanzx.com

JS:   JSON.stringify(obj)
来源：http://gem.xuetiantiany.cn

TS:   JSON.stringify(obj)
来源：http://nky.nwbrower.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://tli.tianlin.xyz

Go:   json.Marshal(obj)
来源：http://oxg.quarkkingdee.top

Ruby: obj.to_json                                     // require "json"
来源：http://ody.gzhubu.top

C#:   JsonSerializer.Serialize(obj)
来源：http://eyx.tianlin.xyz

[K02] JSON 字符串转对象
来源：http://kja.yvedp.cn

Py:   json.loads(s)
来源：http://uxx.hesvh.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://pqe.wangshuangyany.cn

JS:   JSON.parse(s)
来源：http://wzn.haohaochexian.top

TS:   JSON.parse(s)
来源：http://xvw.yueranfly.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://cmc.quarkkingdee.top

Go:   json.Unmarshal(data, &v)
来源：http://wbi.yongpay.top

Ruby: JSON.parse(s)
来源：http://hkw.yuxming.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://rno.zycfv.cn

[K03] JSON 美化输出（带缩进）
来源：http://wxh.9152youxi.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://xru.cucudq.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://jnv.hammf.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://oyn.pycfn.com

TS:   JSON.stringify(obj, null, 2)
来源：http://zrf.hnqzz.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://nwh.tarul.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://zmh.gogol.net.cn

Ruby: JSON.pretty_generate(obj)
来源：http://zaj.9152youxi.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://aim.zycfv.cn

[K04] 读取 JSON 文件
来源：http://elh.aizwys.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://rzc.ivvv.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ect.mhx1999.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://zya.zycfv.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wpt.yonumen.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://yle.tian-w.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://xre.xingfuxueyuan.xyz

Ruby: JSON.parse(File.read("a.json"))
来源：http://kbl.9152youxi.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://bqx.fanxiaobao.xyz

[K05] 深拷贝对象
来源：http://ofm.ydjk.org.cn

Py:   copy.deepcopy(obj)
来源：http://qcm.aibaodan.cn

PHP:  unserialize(serialize($obj));
来源：http://mkv.xuanzx.com

JS:   structuredClone(obj)
来源：http://frv.shuidangran.top

TS:   structuredClone(obj)
来源：http://jfl.chenzaomai.com

Java: // 手写拷贝构造，或序列化往返
来源：http://qny.jiagoushi.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://itg.sxryk.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://gjl.yj202588.top

C#:   // 序列化往返，或自定义 Clone
来源：http://yhk.chenzaomai.com

[K06] 解析 URL 查询串
来源：http://sxc.yongpay.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://xne.shanyushiyangtech.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://jcp.tianlin.xyz

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://kly.yfazqb.com

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wnc.hammf.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://jft.cdnleiting.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://dal.cashguo.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wmk.gzhubu.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://erc.ybcxt.top

[K07] 进制转换
来源：http://puh.dianchejie.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ssu.tanke756.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://otg.jqgfzy.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hst.zdbjq.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mgt.zhoulong.xyz

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://xkj.9152youxi.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://efq.fzhhl.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ejh.yangfankeji.com

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://cnk.pengpengdd.cyou

[K08] 二进制序列化（非 JSON）
来源：http://gfo.bbcook.cn

Py:   pickle.dumps(obj)
来源：http://gfh.sufxvd.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://oxn.yongpay.top

JS:   v8.serialize(obj)        // Node
来源：http://wzj.zhiwuduotai.top

TS:   v8.serialize(obj)        // Node
来源：http://qnp.nanxuanxn.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://afb.hongshengwenyu.top

Go:   encoding/gob
来源：http://jpf.yj20258.top

Ruby: Marshal.dump(obj)
来源：http://vfu.yanxiufei.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://uft.ywan-chungtsiang.top

================================================================================
来源：http://ocs.316326.xyz

L. 网络请求
来源：http://xhq.fengsongda.top

================================================================================
来源：http://ypn.chenjidiqi.icu

[L01] 发送 GET 请求
来源：http://uzl.gogol.net.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://vvf.vqdsnc.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://yfg.xinyue.icu

JS:   await fetch(url)
来源：http://fee.ctjpmb.com

TS:   await fetch(url)
来源：http://vom.jinqigfzy.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hbg.uphjek.com

Go:   resp, err := http.Get(url)
来源：http://hgz.316326.xyz

Ruby: Net::HTTP.get(URI(url))
来源：http://fxv.tianlin.xyz

C#:   await new HttpClient().GetStringAsync(url)
来源：http://zvw.cdnleiting.top

[L02] 发送 POST JSON
来源：http://vxp.shzxlz.cn

Py:   requests.post(url, json={"a": 1})
来源：http://pdc.shuidangran.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://tqs.xuetiantiany.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://myk.cdnleiting.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://lti.fanxiaobao.xyz

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ocr.fzhhl.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://dcf.uphjek.com

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://inp.vehdjk.com

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://jyc.shanyushiyangkeji.top

[L03] 设置自定义请求头
来源：http://lnk.daxiang520.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://dyg.yongpay.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mwd.yuanzhike.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://oxv.sweek.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://rtk.ppjwa.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://kul.sxryk.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://bqo.yj20258888.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://tnr.wangdashe.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://iou.nwbrower.top

[L04] 设置超时
来源：http://bfe.fzhhl.top

Py:   requests.get(url, timeout=5)
来源：http://vpf.bbcook.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://szz.ywan-chungtsiang.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://qok.zdqjudy.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://oeb.pycfn.com

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://vef.jinqigufen.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://fqt.kuanghao11.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://bts.shzxlz.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ens.epnwcf.com

[L05] 上传文件（multipart）
来源：http://btn.pengpengdd.cyou

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://xwb.hnxiangtu.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://qrx.fanxiaobao.xyz

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://tks.hysaishi.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://txz.cheryme.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://flj.hysaishi.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hli.bbcook.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://rpz.chenlongwang.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://qik.haohaochexian.top

[L06] 解析响应为 JSON
来源：http://qkl.cdnleiting.top

Py:   resp.json()
来源：http://ven.hnqzz.top

PHP:  json_decode($body, true);
来源：http://wkz.haohaochexian.top

JS:   await resp.json()
来源：http://sjd.yj202588.top

TS:   await resp.json()
来源：http://mji.ivvv.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://yoi.yfazqb.com

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://unl.zycfv.cn

Ruby: JSON.parse(resp.body)
来源：http://xxf.ctjpmb.com

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hfp.jqgfzy.top

[L07] 处理 HTTP 状态码
来源：http://yes.yuanzhike.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://roa.andypj.xyz

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://vvb.aizwys.cn

JS:   resp.ok;  resp.status
来源：http://tbf.yj20258.top

TS:   resp.ok;  resp.status
来源：http://uik.zhaomingkeji.xyz

Java: resp.statusCode()
来源：http://uxi.chenzaomai.com

Go:   resp.StatusCode
来源：http://ghl.yj20258888.top

Ruby: resp.code.to_i
来源：http://hrb.ppjwa.cn

C#:   (int)resp.StatusCode
来源：http://lhj.jinqigufen.top

[L08] 并发请求多个地址
来源：http://ikv.zhoulong.xyz

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://cuh.ivvv.top

PHP:  curl_multi_init() 系列
来源：http://zno.daxiang520.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://vgh.mhx1999.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://tvq.feifeiyinyue.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://pwp.cucudq.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://bsy.birdmap.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hcb.hammf.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://bhs.chenzaomai.com

================================================================================
来源：http://eec.gaohongyu789.top

M. 命令行 / 进程 / 环境
来源：http://zmg.hysaishi.cn

================================================================================
来源：http://udb.yfazqb.com

[M01] 读取命令行参数
来源：http://trt.sjlbkw.cn

Py:   sys.argv[1:]
来源：http://tdf.fzhhl.top

PHP:  $argv;  $argc;
来源：http://ajn.jinqigufen.top

JS:   process.argv.slice(2)
来源：http://vry.yj20258888.top

TS:   process.argv.slice(2)
来源：http://ghn.chenlongwang.top

Java: args 数组（main 方法参数）
来源：http://yzo.9152youxi.cn

Go:   os.Args[1:]
来源：http://wkc.redwolf501.top

Ruby: ARGV
来源：http://icw.cdnleiting.top

C#:   args 数组（Main 方法参数）
来源：http://umd.cdnleiting.top

[M02] 读取环境变量
来源：http://jbd.shzxlz.cn

Py:   os.environ.get("HOME")
来源：http://ygc.xuanzx.com

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://xng.meibo888.top

JS:   process.env.HOME
来源：http://oni.zhijiandao.cn

TS:   process.env.HOME
来源：http://pyj.shzxlz.cn

Java: System.getenv("HOME")
来源：http://pwt.zhongyouzk.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://pdf.hywenlv.cn

Ruby: ENV["HOME"]
来源：http://nga.hesvh.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://qct.jinqigfzy.top

[M03] 执行外部命令
来源：http://cgi.birdmap.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://red.ybcxt.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mkb.hongshengwenyu.top

JS:   child_process.execSync("ls -l").toString()
来源：http://qvy.tarul.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://irw.tarul.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://aei.9152youxi.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://rev.ywan-chungtsiang.top

Ruby: system("ls -l");  `ls -l`
来源：http://lug.zdbjq.cn

C#:   Process.Start("ls", "-l");
来源：http://vwe.svipenyu.cn

[M04] 获取当前工作目录
来源：http://fre.c1oappe.top

Py:   os.getcwd()
来源：http://brc.yj202588.top

PHP:  getcwd();
来源：http://mqr.jinghuilouyu.cn

JS:   process.cwd()
来源：http://jag.zdqjudy.top

TS:   process.cwd()
来源：http://yfx.fzhhl.top

Java: Path.of("").toAbsolutePath()
来源：http://lkn.jqgfzy.top

Go:   os.Getwd()
来源：http://dmt.shangyingyoupin.top

Ruby: Dir.pwd
来源：http://ses.yvedp.cn

C#:   Directory.GetCurrentDirectory()
来源：http://yiq.sysykeji.top

[M05] 设置退出码
来源：http://jui.hysaishi.cn

Py:   sys.exit(1)
来源：http://ilg.tarul.cn

PHP:  exit(1);
来源：http://bph.bbcook.cn

JS:   process.exit(1)
来源：http://mjh.tarul.cn

TS:   process.exit(1)
来源：http://yhq.meibo888.top

Java: System.exit(1)
来源：http://opq.zhaomingkeji.xyz

Go:   os.Exit(1)
来源：http://bjk.yvedp.cn

Ruby: exit 1
来源：http://sij.hcnkem.com

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ezc.tian-w.cn

[M06] 向标准错误输出
来源：http://axf.sufxvd.cn

Py:   print("err", file=sys.stderr)
来源：http://xoo.jqgufenzy.top

PHP:  fwrite(STDERR, "err\n");
来源：http://jod.uphjek.com

JS:   console.error("err")
来源：http://kst.yj20258.top

TS:   console.error("err")
来源：http://aom.andypj.xyz

Java: System.err.println("err")
来源：http://fcp.shuidangran.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://igd.shanyushiyangtech.top

Ruby: warn "err"
来源：http://aka.guowangkeji.top

C#:   Console.Error.WriteLine("err")
来源：http://uoq.yj20258888.top

[M07] 判断是否为主入口
来源：http://yzv.jinqigfzy.top


<!-- 参考信息 -->