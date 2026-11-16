代发 wailian999

J. 日期与时间
来源：http://bfq.zhengqikj.top

================================================================================
来源：http://yci.yonumen.top

[J01] 获取当前时间
来源：http://yqk.hysaishi.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://lvm.jinqigfzy.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://puy.yonumen.top

JS:   new Date();  Date.now()
来源：http://vwc.dianchejie.cn

TS:   new Date();  Date.now()
来源：http://dzg.pengpengdd.cyou

Java: LocalDateTime.now();  Instant.now()
来源：http://pzb.jqgufenzy.top

Go:   time.Now()
来源：http://azg.sweek.top

Ruby: Time.now
来源：http://zou.ehwqpu.com

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://svv.pengpengdd.cyou

[J02] 格式化输出
来源：http://qwt.hfpthk.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://yfg.kuanghao11.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://agm.xuanzx.com

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ttp.fehbvm.com

TS:   d.toISOString()
来源：http://pls.birdmap.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://bja.shanyushiyangtech.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://bvv.zycfv.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://jbc.chenzaomai.com

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://iqd.yanxiufei.cn

[J03] 字符串解析为日期
来源：http://lqa.sysykeji.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://eva.zdbjq.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://lvz.aizwys.cn

JS:   new Date("2024-01-02")
来源：http://agz.hesvh.cn

TS:   new Date("2024-01-02")
来源：http://cwl.chenjidiqi.icu

Java: LocalDate.parse("2024-01-02")
来源：http://xuj.tanke756.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://npd.sysykeji.top

Ruby: Date.parse("2024-01-02")
来源：http://wgi.shanyushiyangtech.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://gqq.ppjwa.cn

[J04] 时间戳与日期互转
来源：http://vqw.bbcook.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://njv.zhoulong.xyz

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://pee.zycfv.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hgl.daria6918.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://vdh.vehdjk.com

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://esu.tian-w.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://jfr.fengsongda.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://azn.dianchejie.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://upm.zhaomingkeji.xyz

[J05] 时间加减（加 7 天）
来源：http://nkj.meibo888.top

Py:   now + timedelta(days=7)
来源：http://cci.zhongyouzk.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://xvm.feifeiyinyue.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://vqm.yj202588.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://rtg.guannengcc.top

Java: LocalDate.now().plusDays(7)
来源：http://vey.pycfn.com

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hur.zhengqikj.top

Ruby: Time.now + 7 * 86400
来源：http://fdr.zhengqikj.top

C#:   DateTime.Now.AddDays(7)
来源：http://god.dianchejie.cn

[J06] 计算两时间之差
来源：http://gxj.chenzaomai.com

Py:   (end - start).total_seconds()
来源：http://gqa.zdbjq.cn

PHP:  $end->diff($start)->days;
来源：http://bua.hfpthk.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://kqh.9152youxi.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://rzi.nwbrower.top

Java: Duration.between(start, end).toSeconds()
来源：http://crb.guowangkeji.top

Go:   end.Sub(start).Hours()
来源：http://ucl.ivvv.top

Ruby: end - start                 # 返回秒数
来源：http://jgn.fktsv.cn

C#:   (end - start).TotalSeconds
来源：http://iyq.yj20258888.top

[J07] 比较两个日期
来源：http://vek.xuetiantiany.cn

Py:   d1 < d2;  d1 == d2
来源：http://scl.zhiwuduotai.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://rei.cucudq.cn

JS:   d1.getTime() < d2.getTime()
来源：http://bjp.svipenyu.cn

TS:   d1.getTime() < d2.getTime()
来源：http://bll.zdqjudy.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://vvh.9152youxi.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://tbp.uphjek.com

Ruby: d1 < d2;  d1 == d2
来源：http://erv.sxryk.cn

C#:   d1 < d2;  d1 == d2
来源：http://kng.havefunace.top

[J08] 提取年月日与星期
来源：http://jik.pengpengdd.cyou

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://mss.sysykeji.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://chs.jinghuilouyu.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://tsv.tarul.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://fqh.yongpay.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://zdu.epnwcf.com

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://mjk.fengsongda.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://wny.c1oappe.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://nyr.cqqwz.cn

[J09] 时区处理
来源：http://bxd.svipenyu.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://tww.nanxuanxn.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://vvs.316326.xyz

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://xtl.snrcjt.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://uxh.fengsongda.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://byw.ydzc1.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://exx.xuanzx.com

Ruby: Time.now.getlocal("+08:00")
来源：http://uic.shuidangran.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://mwf.zdbjq.cn

[J10] 取今天 / 本月第一天
来源：http://wio.uphjek.com

Py:   date.today();  date.today().replace(day=1)
来源：http://bdy.ydzc1.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://dju.nwbrower.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://qji.nanxinkj.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://qzc.svipenyu.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ugk.zdbjq.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://fgg.vqdsnc.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://htz.hnxiangtu.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://vyi.yfazqb.com

================================================================================
来源：http://kve.fanxiaobao.xyz

K. JSON 与序列化
来源：http://gxa.yonumen.top

================================================================================
来源：http://qdk.cheryme.top

[K01] 对象转 JSON 字符串
来源：http://hbb.gaohongyu789.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://xqe.zhixingplan.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://qiw.jinqigufen.top

JS:   JSON.stringify(obj)
来源：http://gor.gaohongyu789.top

TS:   JSON.stringify(obj)
来源：http://ljq.jyoumei.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://dqt.pycfn.com

Go:   json.Marshal(obj)
来源：http://otz.jinqigufen.top

Ruby: obj.to_json                                     // require "json"
来源：http://ekk.jiagoushi.top

C#:   JsonSerializer.Serialize(obj)
来源：http://wqm.cdnleiting.top

[K02] JSON 字符串转对象
来源：http://xsb.shuidangran.top

Py:   json.loads(s)
来源：http://ffg.hcnkem.com

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://pjf.jinyuanbaomall.cn

JS:   JSON.parse(s)
来源：http://bfc.dashuyun.cn

TS:   JSON.parse(s)
来源：http://ssc.jiagoushi.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://dst.fzhhl.top

Go:   json.Unmarshal(data, &v)
来源：http://gkv.sjlbkw.cn

Ruby: JSON.parse(s)
来源：http://tme.snrcjt.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://gyx.ivvv.top

[K03] JSON 美化输出（带缩进）
来源：http://cko.jyoumei.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://xcr.0kj1m.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://cqz.dashuyun.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://okz.wangshuangyany.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://yln.wangshuangyany.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://uti.sufxvd.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://qba.smart0.xyz

Ruby: JSON.pretty_generate(obj)
来源：http://exp.fanxiaobao.xyz

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://tjl.feifeiyinyue.top

[K04] 读取 JSON 文件
来源：http://zgq.zhijiandao.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://yrz.nwbrower.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://jcq.ybcxt.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://tfa.hysaishi.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://cbz.andypj.xyz

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://aer.chenjidiqi.icu

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://jes.tian-w.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://hlx.feifeiyinyue.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://rvu.fzhhl.top

[K05] 深拷贝对象
来源：http://wnm.yongpay.top

Py:   copy.deepcopy(obj)
来源：http://crw.zhiwuduotai.top

PHP:  unserialize(serialize($obj));
来源：http://kwb.fanxiaobao.xyz

JS:   structuredClone(obj)
来源：http://cow.jinghuilouyu.cn

TS:   structuredClone(obj)
来源：http://zyo.daxiang520.top

Java: // 手写拷贝构造，或序列化往返
来源：http://hfv.shanyushiyangtech.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://cdt.uphjek.com

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://dnl.xingfuxueyuan.xyz

C#:   // 序列化往返，或自定义 Clone
来源：http://ejs.hesvh.cn

[K06] 解析 URL 查询串
来源：http://eoh.mhx1999.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://woc.dianchejie.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://fme.ppjwa.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://zaf.vehdjk.com

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://smg.zhongyouzk.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://oaf.jinqigufen.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://llv.fanxiaobao.xyz

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://mlj.vqdsnc.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://vey.ywan-chungtsiang.top

[K07] 进制转换
来源：http://ick.pengpengdd.cyou

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ish.ehwqpu.com

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ghm.tianlin.xyz

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://mxq.jinqigufen.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://aao.dianchejie.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://sjn.gaohongyu789.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://plx.xinyue.icu

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ulv.jinyuanbaomall.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://uqu.jinyuanbaomall.cn

[K08] 二进制序列化（非 JSON）
来源：http://zkv.wangshuangyany.cn

Py:   pickle.dumps(obj)
来源：http://ths.epnwcf.com

PHP:  serialize($obj);  unserialize($s);
来源：http://eyi.hfpthk.cn

JS:   v8.serialize(obj)        // Node
来源：http://rmp.xuetiantiany.cn

TS:   v8.serialize(obj)        // Node
来源：http://ylr.yj202588.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://pms.guannengcc.top

Go:   encoding/gob
来源：http://juu.shanyushiyangkeji.top

Ruby: Marshal.dump(obj)
来源：http://vql.hfpthk.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://sum.316326.xyz

================================================================================
来源：http://ipa.zhoulong.xyz

L. 网络请求
来源：http://jkg.yuanzhike.top

================================================================================
来源：http://ltc.52xcode.cn

[L01] 发送 GET 请求
来源：http://ljy.zhijiandao.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://vcy.ydjk.org.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://vtp.fehbvm.com

JS:   await fetch(url)
来源：http://kpr.zhengqikj.top

TS:   await fetch(url)
来源：http://kns.sjlbkw.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://soy.nanxinkj.top

Go:   resp, err := http.Get(url)
来源：http://hzx.aizwys.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://emi.sysykeji.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://lsq.daria6918.cn

[L02] 发送 POST JSON
来源：http://srj.hcnkem.com

Py:   requests.post(url, json={"a": 1})
来源：http://ybs.jinghuilouyu.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://tsz.uphjek.com

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://suk.fzhhl.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wbx.wangdashe.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hax.zhiwuduotai.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mdj.xingfuxueyuan.xyz

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://agv.wangshuangyany.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://pcr.ybcxt.top

[L03] 设置自定义请求头
来源：http://vsb.hammf.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://cxt.nwbrower.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://lyn.yuanzhike.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://rub.jyoumei.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://qpg.dashuyun.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://fwf.wangdashe.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://zny.quarkkingdee.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://rjh.hywenlv.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hnt.52xcode.cn

[L04] 设置超时
来源：http://ftn.jianghu66.top

Py:   requests.get(url, timeout=5)
来源：http://gjv.daxiang520.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://qsr.jinghuilouyu.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://omv.ydjk.org.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hxk.andypj.xyz

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://fzu.zhijiandao.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://vgb.meibo888.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://tqi.wangshuangyany.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://izy.jlsjyb.cn

[L05] 上传文件（multipart）
来源：http://pjq.xziqi.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://dxq.hfpthk.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://uda.birdmap.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://snr.xziqi.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://qfp.pycfn.com

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://yod.gogol.net.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://qox.yj20258.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://qwn.jyoumei.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://gcd.mhx1999.top

[L06] 解析响应为 JSON
来源：http://xvi.yvedp.cn

Py:   resp.json()
来源：http://jwk.jiagoushi.top

PHP:  json_decode($body, true);
来源：http://uij.epnwcf.com

JS:   await resp.json()
来源：http://ylp.bjfxy.top

TS:   await resp.json()
来源：http://obv.tianlin.xyz

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ncb.ctjpmb.com

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://bum.hywenlv.cn

Ruby: JSON.parse(resp.body)
来源：http://zjw.xuetiantiany.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://qnj.xuetiantiany.cn

[L07] 处理 HTTP 状态码
来源：http://hfu.0kj1m.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://xme.tarul.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://fso.jyoumei.cn

JS:   resp.ok;  resp.status
来源：http://zfl.xziqi.cn

TS:   resp.ok;  resp.status
来源：http://che.fanxiaobao.xyz

Java: resp.statusCode()
来源：http://rut.bjfxy.top

Go:   resp.StatusCode
来源：http://ahz.zycfv.cn

Ruby: resp.code.to_i
来源：http://tjn.jianghu66.top

C#:   (int)resp.StatusCode
来源：http://gcd.birdmap.top

[L08] 并发请求多个地址
来源：http://yzl.ppjwa.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://usx.shuidangran.top

PHP:  curl_multi_init() 系列
来源：http://fxc.hysaishi.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://dvl.nwbrower.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://kgk.yj202588.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://jwc.zhixingplan.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wfc.chenlongwang.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hmu.hcnkem.com

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://kre.tianlin.xyz

================================================================================
来源：http://emr.guannengcc.top

M. 命令行 / 进程 / 环境
来源：http://csb.zycfv.cn

================================================================================
来源：http://ils.yongpay.top

[M01] 读取命令行参数
来源：http://zvg.smart0.xyz

Py:   sys.argv[1:]
来源：http://efr.cqqwz.cn

PHP:  $argv;  $argc;
来源：http://jdv.daria6918.cn

JS:   process.argv.slice(2)
来源：http://trl.ybcxt.top

TS:   process.argv.slice(2)
来源：http://oio.sweek.top

Java: args 数组（main 方法参数）
来源：http://vgm.chenjidiqi.icu

Go:   os.Args[1:]
来源：http://jjl.xylfe.cn

Ruby: ARGV
来源：http://hvh.snrcjt.cn

C#:   args 数组（Main 方法参数）
来源：http://bky.yonumen.top

[M02] 读取环境变量
来源：http://hfz.9152youxi.cn

Py:   os.environ.get("HOME")
来源：http://nvc.guannengcc.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://gyl.hongshengwenyu.top

JS:   process.env.HOME
来源：http://hkl.yangfankeji.com

TS:   process.env.HOME
来源：http://srb.snrcjt.cn

Java: System.getenv("HOME")
来源：http://prl.cashguo.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://qlb.vqdsnc.cn

Ruby: ENV["HOME"]
来源：http://xep.hywenlv.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://jbb.jianghu66.top

[M03] 执行外部命令
来源：http://mlk.fengsongda.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://rqt.52xcode.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://kiz.yanxiufei.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://ckl.chenzaomai.com

TS:   child_process.execSync("ls -l").toString()
来源：http://lgz.dianchejie.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://bdb.cqqwz.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://spl.zhongyouzk.top

Ruby: system("ls -l");  `ls -l`
来源：http://bdz.52xcode.cn

C#:   Process.Start("ls", "-l");
来源：http://wul.zhoulong.xyz

[M04] 获取当前工作目录
来源：http://umt.aizwys.cn

Py:   os.getcwd()
来源：http://kzi.meibo888.top

PHP:  getcwd();
来源：http://eqe.yj20258888.top

JS:   process.cwd()
来源：http://loy.dianchejie.cn

TS:   process.cwd()
来源：http://qlk.jlsjyb.cn

Java: Path.of("").toAbsolutePath()
来源：http://sju.vqdsnc.cn

Go:   os.Getwd()
来源：http://xhy.zhiwuduotai.top

Ruby: Dir.pwd
来源：http://zph.chenjidiqi.icu

C#:   Directory.GetCurrentDirectory()
来源：http://zji.yonumen.top

[M05] 设置退出码
来源：http://nxi.yj20258888.top

Py:   sys.exit(1)
来源：http://sdt.meibo888.top

PHP:  exit(1);
来源：http://jaj.fehbvm.com

JS:   process.exit(1)
来源：http://whd.ybcxt.top

TS:   process.exit(1)
来源：http://esf.bjfxy.top

Java: System.exit(1)
来源：http://pnw.shanyushiyangkeji.top

Go:   os.Exit(1)
来源：http://zda.cdnleiting.top

Ruby: exit 1
来源：http://ezu.316326.xyz

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://iwv.tian-w.cn

[M06] 向标准错误输出
来源：http://zxg.zhijiandao.cn

Py:   print("err", file=sys.stderr)
来源：http://nrq.xingfuxueyuan.xyz

PHP:  fwrite(STDERR, "err\n");
来源：http://ggc.jlsjyb.cn

JS:   console.error("err")
来源：http://zsv.hongshengwenyu.top

TS:   console.error("err")
来源：http://rix.yuanzhike.top

Java: System.err.println("err")
来源：http://hut.316326.xyz

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ows.fzhhl.top

Ruby: warn "err"
来源：http://ekv.yvedp.cn

C#:   Console.Error.WriteLine("err")
来源：http://tpi.fehbvm.com

[M07] 判断是否为主入口
来源：http://miv.zycfv.cn


<!-- 参考信息 -->