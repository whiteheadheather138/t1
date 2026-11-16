代发 wailian999

J. 日期与时间
来源：http://jou.chenzaomai.com

================================================================================
来源：http://caj.tianlin.xyz

[J01] 获取当前时间
来源：http://sbm.xuetiantiany.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://zjf.svipenyu.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://iwb.dianchejie.cn

JS:   new Date();  Date.now()
来源：http://tqu.jinqigfzy.top

TS:   new Date();  Date.now()
来源：http://kyo.9152youxi.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://naf.fehbvm.com

Go:   time.Now()
来源：http://ucr.zhongyouzk.top

Ruby: Time.now
来源：http://znm.epnwcf.com

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://iev.epnwcf.com

[J02] 格式化输出
来源：http://agw.jianghu66.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://idr.cucudq.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://irv.xuanzx.com

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://umb.xylfe.cn

TS:   d.toISOString()
来源：http://tnv.aibaodan.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://heu.hammf.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://cjr.guannengcc.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://lrl.gotoacloud.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://bnc.shanyushiyangkeji.top

[J03] 字符串解析为日期
来源：http://evy.nanxuanxn.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://tiz.ctjpmb.com

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://frx.sxryk.cn

JS:   new Date("2024-01-02")
来源：http://wbr.zhaomingkeji.xyz

TS:   new Date("2024-01-02")
来源：http://oku.zhongyouzk.top

Java: LocalDate.parse("2024-01-02")
来源：http://yvp.snrcjt.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://zdm.jyoumei.cn

Ruby: Date.parse("2024-01-02")
来源：http://gjk.nanxuanxn.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ruu.nwbrower.top

[J04] 时间戳与日期互转
来源：http://bav.yuxming.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://zhd.smart0.xyz

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ign.haohaochexian.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://yeu.feifeiyinyue.top

TS:   Math.floor(Date.now() / 1000)
来源：http://jwh.zhengqikj.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://dgf.shanyushiyangtech.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://xlf.gotoacloud.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ver.ctjpmb.com

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://svr.yongpay.top

[J05] 时间加减（加 7 天）
来源：http://bqt.fengsongda.top

Py:   now + timedelta(days=7)
来源：http://rrr.pengpengdd.cyou

PHP:  (new DateTime())->modify("+7 days");
来源：http://oem.ctjpmb.com

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ehg.yuanzhike.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://zja.ydzc1.top

Java: LocalDate.now().plusDays(7)
来源：http://yxg.fzhhl.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://peg.cucudq.cn

Ruby: Time.now + 7 * 86400
来源：http://cbr.52xcode.cn

C#:   DateTime.Now.AddDays(7)
来源：http://fjg.quarkkingdee.top

[J06] 计算两时间之差
来源：http://kxk.316326.xyz

Py:   (end - start).total_seconds()
来源：http://jgd.shangyingyoupin.top

PHP:  $end->diff($start)->days;
来源：http://jjd.tianlin.xyz

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://gxr.redwolf501.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://chw.wangshuangyany.cn

Java: Duration.between(start, end).toSeconds()
来源：http://oii.hongshengwenyu.top

Go:   end.Sub(start).Hours()
来源：http://stl.bbcook.cn

Ruby: end - start                 # 返回秒数
来源：http://uor.zhiwuduotai.top

C#:   (end - start).TotalSeconds
来源：http://mgm.hywenlv.cn

[J07] 比较两个日期
来源：http://mgv.hysaishi.cn

Py:   d1 < d2;  d1 == d2
来源：http://maq.bbcook.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://yja.xuanzx.com

JS:   d1.getTime() < d2.getTime()
来源：http://muo.jqgufenzy.top

TS:   d1.getTime() < d2.getTime()
来源：http://bzh.yuanzhike.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://fnu.sweek.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ktg.shanyushiyangtech.top

Ruby: d1 < d2;  d1 == d2
来源：http://gwc.shuidangran.top

C#:   d1 < d2;  d1 == d2
来源：http://ykg.yangfankeji.com

[J08] 提取年月日与星期
来源：http://gqe.redwolf501.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://eam.zhixingplan.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hxw.yuxming.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://abl.sysykeji.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://xuz.zhiwuduotai.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://lxf.zdqjudy.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://rgo.shzxlz.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://whz.daria6918.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://dox.jqgfzy.top

[J09] 时区处理
来源：http://jhy.tianlin.xyz

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ssy.guannengcc.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://bmd.fzhhl.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wbm.cashguo.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://fnk.sufxvd.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://epf.zhaomingkeji.xyz

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://bid.dashuyun.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://imv.ctjpmb.com

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://qpe.svipenyu.cn

[J10] 取今天 / 本月第一天
来源：http://jbf.gzhubu.top

Py:   date.today();  date.today().replace(day=1)
来源：http://vao.bjfxy.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ckr.nanxinkj.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://eij.chenlongwang.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://qtb.zhengqikj.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://zfo.hongshengwenyu.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://qcc.zhaomingkeji.xyz

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ekr.havefunace.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://kbl.shuidangran.top

================================================================================
来源：http://uzp.quarkkingdee.top

K. JSON 与序列化
来源：http://wqd.zhiwuduotai.top

================================================================================
来源：http://doa.birdmap.top

[K01] 对象转 JSON 字符串
来源：http://fct.dianchejie.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://epd.yuanzhike.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://rvo.sjlbkw.cn

JS:   JSON.stringify(obj)
来源：http://kkc.shzxlz.cn

TS:   JSON.stringify(obj)
来源：http://wix.bbcook.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://mke.shuidangran.top

Go:   json.Marshal(obj)
来源：http://uiw.guowangkeji.top

Ruby: obj.to_json                                     // require "json"
来源：http://kac.zycfv.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://yil.xingfuxueyuan.xyz

[K02] JSON 字符串转对象
来源：http://bjs.ybcxt.top

Py:   json.loads(s)
来源：http://jbs.hywenlv.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://lnp.xinyue.icu

JS:   JSON.parse(s)
来源：http://ddq.guannengcc.top

TS:   JSON.parse(s)
来源：http://lyy.xinyue.icu

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ppp.bbcook.cn

Go:   json.Unmarshal(data, &v)
来源：http://okn.zhoulong.xyz

Ruby: JSON.parse(s)
来源：http://ltv.andypj.xyz

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://oag.yfazqb.com

[K03] JSON 美化输出（带缩进）
来源：http://ejj.zhongyouzk.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ajf.ydjk.org.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://aql.jinghuilouyu.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://lhp.jiagoushi.top

TS:   JSON.stringify(obj, null, 2)
来源：http://rbz.hammf.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ffa.hnxiangtu.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://fld.xuetiantiany.cn

Ruby: JSON.pretty_generate(obj)
来源：http://dya.hywenlv.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://vai.shuidangran.top

[K04] 读取 JSON 文件
来源：http://zqg.vehdjk.com

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://klg.shuidangran.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://azr.dashuyun.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://faq.fehbvm.com

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://pti.wangshuangyany.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://shw.cheryme.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://xeb.havefunace.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://vzn.sysykeji.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://xdt.yonumen.top

[K05] 深拷贝对象
来源：http://uxw.nanxinkj.top

Py:   copy.deepcopy(obj)
来源：http://vxo.chenlongwang.top

PHP:  unserialize(serialize($obj));
来源：http://wdx.yj202588.top

JS:   structuredClone(obj)
来源：http://jsz.hcnkem.com

TS:   structuredClone(obj)
来源：http://ghm.vehdjk.com

Java: // 手写拷贝构造，或序列化往返
来源：http://wht.jinqigufen.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://dut.ybcxt.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://dqb.sufxvd.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://ogk.yuanzhike.top

[K06] 解析 URL 查询串
来源：http://evr.tian-w.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://qno.yuanzhike.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://wah.xingfuxueyuan.xyz

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://zvy.yfazqb.com

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://jmy.hammf.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://khb.shanyushiyangkeji.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://ile.zdbjq.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://fva.yuanzhike.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://xzw.xingfuxueyuan.xyz

[K07] 进制转换
来源：http://ycq.nanxinkj.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://tsk.fanxiaobao.xyz

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://gqg.xziqi.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://xat.hnqzz.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wct.xingfuxueyuan.xyz

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://vfr.feifeiyinyue.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://kmk.ydzc1.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://lip.jinghuilouyu.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://vrf.xuanzx.com

[K08] 二进制序列化（非 JSON）
来源：http://vlj.nanxinkj.top

Py:   pickle.dumps(obj)
来源：http://qdw.zycfv.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://ear.dashuyun.cn

JS:   v8.serialize(obj)        // Node
来源：http://aeg.9152youxi.cn

TS:   v8.serialize(obj)        // Node
来源：http://keg.jinghuilouyu.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://jjf.aibaodan.cn

Go:   encoding/gob
来源：http://jji.wangdashe.top

Ruby: Marshal.dump(obj)
来源：http://fsj.zhongyouzk.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://keb.cdnleiting.top

================================================================================
来源：http://bof.zhongyouzk.top

L. 网络请求
来源：http://fzi.yfazqb.com

================================================================================
来源：http://ama.fehbvm.com

[L01] 发送 GET 请求
来源：http://uqg.guowangkeji.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ebz.tarul.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://xrf.zycfv.cn

JS:   await fetch(url)
来源：http://fku.daria6918.cn

TS:   await fetch(url)
来源：http://rlc.zhixingplan.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://pwu.zhijiandao.cn

Go:   resp, err := http.Get(url)
来源：http://bnu.cucudq.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://tka.sysykeji.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://sfd.hysaishi.cn

[L02] 发送 POST JSON
来源：http://pbr.haohaochexian.top

Py:   requests.post(url, json={"a": 1})
来源：http://xzc.jqgufenzy.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://krm.hnxiangtu.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://cjd.316326.xyz

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://uir.cqqwz.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://fvg.yj20258.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://bwh.dashuyun.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://htg.tanke756.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://lxm.52xcode.cn

[L03] 设置自定义请求头
来源：http://inv.bjfxy.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://xmc.chenlongwang.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://fss.kuanghao11.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://isl.tianlin.xyz

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://gzh.yuxming.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ksd.shangyingyoupin.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mci.jiagoushi.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wub.xuanzx.com

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wzl.bjfxy.top

[L04] 设置超时
来源：http://wdp.cashguo.top

Py:   requests.get(url, timeout=5)
来源：http://qzq.xuetiantiany.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hth.quarkkingdee.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://czx.chenjidiqi.icu

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://cwj.shzxlz.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://afk.fengsongda.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://pju.nanxuanxn.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://gyb.jiagoushi.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://oei.jinyuanbaomall.cn

[L05] 上传文件（multipart）
来源：http://dkl.fanxiaobao.xyz

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://zon.cqqwz.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://qul.nanxinkj.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://nir.ydjk.org.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://bxo.tian-w.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://krx.feifeiyinyue.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://cka.zhongyouzk.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://btn.hammf.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://oah.fengsongda.top

[L06] 解析响应为 JSON
来源：http://mgu.xuetiantiany.cn

Py:   resp.json()
来源：http://spb.xziqi.cn

PHP:  json_decode($body, true);
来源：http://rgx.mhx1999.top

JS:   await resp.json()
来源：http://yjn.yuxming.cn

TS:   await resp.json()
来源：http://vdk.sysykeji.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ssg.9152youxi.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://bpm.jinghuilouyu.cn

Ruby: JSON.parse(resp.body)
来源：http://dim.daria6918.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://blz.zhiwuduotai.top

[L07] 处理 HTTP 状态码
来源：http://hlj.wangshuangyany.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ijr.xziqi.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://tto.yangfankeji.com

JS:   resp.ok;  resp.status
来源：http://dsc.chenlongwang.top

TS:   resp.ok;  resp.status
来源：http://jcj.yuxming.cn

Java: resp.statusCode()
来源：http://gdh.hcnkem.com

Go:   resp.StatusCode
来源：http://ecl.zhaomingkeji.xyz

Ruby: resp.code.to_i
来源：http://azc.feifeiyinyue.top

C#:   (int)resp.StatusCode
来源：http://xsn.hfpthk.cn

[L08] 并发请求多个地址
来源：http://qfs.hnqzz.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://uvr.jqgufenzy.top

PHP:  curl_multi_init() 系列
来源：http://smy.fehbvm.com

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://gdg.cdnleiting.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://the.jqgfzy.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://pha.tianlin.xyz

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://vcj.haohaochexian.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://yqr.hammf.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://iia.hcnkem.com

================================================================================
来源：http://ykq.ybcxt.top

M. 命令行 / 进程 / 环境
来源：http://bwh.fehbvm.com

================================================================================
来源：http://jms.zhongyouzk.top

[M01] 读取命令行参数
来源：http://qeo.cashguo.top

Py:   sys.argv[1:]
来源：http://szc.ppjwa.cn

PHP:  $argv;  $argc;
来源：http://ffs.zhijiandao.cn

JS:   process.argv.slice(2)
来源：http://qny.sweek.top

TS:   process.argv.slice(2)
来源：http://olr.cdnleiting.top

Java: args 数组（main 方法参数）
来源：http://fbn.tanke756.top

Go:   os.Args[1:]
来源：http://nah.jqgufenzy.top

Ruby: ARGV
来源：http://meq.ydjk.org.cn

C#:   args 数组（Main 方法参数）
来源：http://etc.shuidangran.top

[M02] 读取环境变量
来源：http://xqn.hfpthk.cn

Py:   os.environ.get("HOME")
来源：http://pfz.xuetiantiany.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://bqn.zdbjq.cn

JS:   process.env.HOME
来源：http://uyx.hfpthk.cn

TS:   process.env.HOME
来源：http://ttj.tian-w.cn

Java: System.getenv("HOME")
来源：http://rvq.jinghuilouyu.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ldr.shuidangran.top

Ruby: ENV["HOME"]
来源：http://klp.xinyue.icu

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://rzr.hysaishi.cn

[M03] 执行外部命令
来源：http://dqg.redwolf501.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://nzt.ywan-chungtsiang.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://oxc.hysaishi.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://ivl.yongpay.top

TS:   child_process.execSync("ls -l").toString()
来源：http://hut.wangshuangyany.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://keh.zhongyouzk.top

Go:   exec.Command("ls", "-l").Output()
来源：http://upd.guowangkeji.top

Ruby: system("ls -l");  `ls -l`
来源：http://ngs.vehdjk.com

C#:   Process.Start("ls", "-l");
来源：http://vwh.yvedp.cn

[M04] 获取当前工作目录
来源：http://xnf.jinyuanbaomall.cn

Py:   os.getcwd()
来源：http://hba.yj20258.top

PHP:  getcwd();
来源：http://opj.meibo888.top

JS:   process.cwd()
来源：http://sew.aizwys.cn

TS:   process.cwd()
来源：http://pea.dianchejie.cn

Java: Path.of("").toAbsolutePath()
来源：http://jpc.cashguo.top

Go:   os.Getwd()
来源：http://cjq.snrcjt.cn

Ruby: Dir.pwd
来源：http://ytz.hfpthk.cn

C#:   Directory.GetCurrentDirectory()
来源：http://mmh.hnxiangtu.top

[M05] 设置退出码
来源：http://lcc.yfazqb.com

Py:   sys.exit(1)
来源：http://mau.aibaodan.cn

PHP:  exit(1);
来源：http://txz.daxiang520.top

JS:   process.exit(1)
来源：http://dnd.xylfe.cn

TS:   process.exit(1)
来源：http://jwu.xuetiantiany.cn

Java: System.exit(1)
来源：http://nwo.shanyushiyangkeji.top

Go:   os.Exit(1)
来源：http://zky.andypj.xyz

Ruby: exit 1
来源：http://uqx.sxryk.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ihn.svipenyu.cn

[M06] 向标准错误输出
来源：http://jif.yueranfly.top

Py:   print("err", file=sys.stderr)
来源：http://mqq.yangfankeji.com

PHP:  fwrite(STDERR, "err\n");
来源：http://qzp.shanyushiyangkeji.top

JS:   console.error("err")
来源：http://boh.havefunace.top

TS:   console.error("err")
来源：http://rod.xuanzx.com

Java: System.err.println("err")
来源：http://cha.jianghu66.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mal.kuanghao11.cn

Ruby: warn "err"
来源：http://psy.hongshengwenyu.top

C#:   Console.Error.WriteLine("err")
来源：http://kkq.shanyushiyangkeji.top

[M07] 判断是否为主入口
来源：http://cfq.zycfv.cn


<!-- 参考信息 -->