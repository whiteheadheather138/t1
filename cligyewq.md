代发 wailian999

J. 日期与时间
来源：http://zsr.ppjwa.cn

================================================================================
来源：http://eej.cheryme.top

[J01] 获取当前时间
来源：http://sqv.ivvv.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://mfl.tianlin.xyz

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://flz.cqqwz.cn

JS:   new Date();  Date.now()
来源：http://spi.jinghuilouyu.cn

TS:   new Date();  Date.now()
来源：http://qhu.jinqigfzy.top

Java: LocalDateTime.now();  Instant.now()
来源：http://gaa.chenlongwang.top

Go:   time.Now()
来源：http://ufq.sweek.top

Ruby: Time.now
来源：http://fty.wangshuangyany.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://wln.yongpay.top

[J02] 格式化输出
来源：http://obe.vqdsnc.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ixd.yuxming.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://qny.zhiwuduotai.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://weh.yj20258.top

TS:   d.toISOString()
来源：http://opy.zycfv.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://dff.zhiwuduotai.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://tyt.cucudq.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://pln.sysykeji.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://rpr.c1oappe.top

[J03] 字符串解析为日期
来源：http://nmc.feifeiyinyue.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://bfw.birdmap.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://jzl.guowangkeji.top

JS:   new Date("2024-01-02")
来源：http://uxr.vehdjk.com

TS:   new Date("2024-01-02")
来源：http://gbr.wangshuangyany.cn

Java: LocalDate.parse("2024-01-02")
来源：http://mev.vqdsnc.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://wdj.sweek.top

Ruby: Date.parse("2024-01-02")
来源：http://hws.hysaishi.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://oaf.yj202588.top

[J04] 时间戳与日期互转
来源：http://mdq.cdnleiting.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://dhh.yangfankeji.com

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://kdk.cucudq.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://cuq.chenlongwang.top

TS:   Math.floor(Date.now() / 1000)
来源：http://zrb.xingfuxueyuan.xyz

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://tya.ydjk.org.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ief.chenzaomai.com

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ugt.cheryme.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ucy.snrcjt.cn

[J05] 时间加减（加 7 天）
来源：http://ijo.jianghu66.top

Py:   now + timedelta(days=7)
来源：http://enn.hywenlv.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://aaf.hcnkem.com

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://alj.jinqigufen.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://fic.sufxvd.cn

Java: LocalDate.now().plusDays(7)
来源：http://yfu.fanxiaobao.xyz

Go:   time.Now().AddDate(0, 0, 7)
来源：http://vlb.gogol.net.cn

Ruby: Time.now + 7 * 86400
来源：http://nbd.ywan-chungtsiang.top

C#:   DateTime.Now.AddDays(7)
来源：http://jao.9152youxi.cn

[J06] 计算两时间之差
来源：http://xxr.fktsv.cn

Py:   (end - start).total_seconds()
来源：http://lgf.meibo888.top

PHP:  $end->diff($start)->days;
来源：http://fdg.snrcjt.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ien.fanxiaobao.xyz

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://wld.fzhhl.top

Java: Duration.between(start, end).toSeconds()
来源：http://jay.yanxiufei.cn

Go:   end.Sub(start).Hours()
来源：http://kyb.kuanghao11.cn

Ruby: end - start                 # 返回秒数
来源：http://acb.uphjek.com

C#:   (end - start).TotalSeconds
来源：http://aaw.hcnkem.com

[J07] 比较两个日期
来源：http://xvg.hnxiangtu.top

Py:   d1 < d2;  d1 == d2
来源：http://tac.zhoulong.xyz

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://zyp.yj20258.top

JS:   d1.getTime() < d2.getTime()
来源：http://wxj.zhixingplan.top

TS:   d1.getTime() < d2.getTime()
来源：http://wij.316326.xyz

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hwb.gaohongyu789.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://lpy.havefunace.top

Ruby: d1 < d2;  d1 == d2
来源：http://qiw.pengpengdd.cyou

C#:   d1 < d2;  d1 == d2
来源：http://jrd.haohaochexian.top

[J08] 提取年月日与星期
来源：http://dju.jyoumei.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://mbr.zhaomingkeji.xyz

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://sav.bjfxy.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://nji.zhixingplan.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://znd.sxryk.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://rah.redwolf501.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://bhl.epnwcf.com

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://uxm.svipenyu.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://pav.nanxuanxn.top

[J09] 时区处理
来源：http://vof.bjfxy.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://tmo.pycfn.com

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://gmw.ydzc1.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://lky.snrcjt.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mpy.smart0.xyz

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://jut.fengsongda.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ikq.xingfuxueyuan.xyz

Ruby: Time.now.getlocal("+08:00")
来源：http://gqs.bbcook.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://rqj.tanke756.top

[J10] 取今天 / 本月第一天
来源：http://iff.fzhhl.top

Py:   date.today();  date.today().replace(day=1)
来源：http://nms.ppjwa.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hii.ehwqpu.com

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://nii.hammf.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://fcj.jianghu66.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://tpl.316326.xyz

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://owr.yuanzhike.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://wyx.jinghuilouyu.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ums.fengsongda.top

================================================================================
来源：http://hpk.yuanzhike.top

K. JSON 与序列化
来源：http://dge.yfazqb.com

================================================================================
来源：http://gdo.feifeiyinyue.top

[K01] 对象转 JSON 字符串
来源：http://pyr.zhoulong.xyz

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://syl.yj202588.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hvf.xingfuxueyuan.xyz

JS:   JSON.stringify(obj)
来源：http://fyt.cheryme.top

TS:   JSON.stringify(obj)
来源：http://mlr.haohaochexian.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://mdy.hysaishi.cn

Go:   json.Marshal(obj)
来源：http://rxe.snrcjt.cn

Ruby: obj.to_json                                     // require "json"
来源：http://sgh.uphjek.com

C#:   JsonSerializer.Serialize(obj)
来源：http://ygl.daria6918.cn

[K02] JSON 字符串转对象
来源：http://bdk.snrcjt.cn

Py:   json.loads(s)
来源：http://kqf.zhiwuduotai.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://kem.haohaochexian.top

JS:   JSON.parse(s)
来源：http://euy.andypj.xyz

TS:   JSON.parse(s)
来源：http://zox.epnwcf.com

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://kpa.xingfuxueyuan.xyz

Go:   json.Unmarshal(data, &v)
来源：http://yfc.yvedp.cn

Ruby: JSON.parse(s)
来源：http://rgh.316326.xyz

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://vdt.pycfn.com

[K03] JSON 美化输出（带缩进）
来源：http://myf.xuanzx.com

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://sjm.birdmap.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://fbl.vqdsnc.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://utb.uphjek.com

TS:   JSON.stringify(obj, null, 2)
来源：http://zyz.zdqjudy.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hxr.birdmap.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://xye.cashguo.top

Ruby: JSON.pretty_generate(obj)
来源：http://nng.guannengcc.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://rfb.zhaomingkeji.xyz

[K04] 读取 JSON 文件
来源：http://lev.52xcode.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://kqx.haohaochexian.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://qpa.hfpthk.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://buc.xingfuxueyuan.xyz

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://lbw.ydzc1.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://xfs.gzhubu.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ptw.xuanzx.com

Ruby: JSON.parse(File.read("a.json"))
来源：http://gbt.dashuyun.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://cqr.ydzc1.top

[K05] 深拷贝对象
来源：http://idk.nwbrower.top

Py:   copy.deepcopy(obj)
来源：http://ksy.sysykeji.top

PHP:  unserialize(serialize($obj));
来源：http://jus.sweek.top

JS:   structuredClone(obj)
来源：http://dxf.shangyingyoupin.top

TS:   structuredClone(obj)
来源：http://uri.zhoulong.xyz

Java: // 手写拷贝构造，或序列化往返
来源：http://loc.bjfxy.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://xlm.ywan-chungtsiang.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://xaz.ppjwa.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://ggr.zycfv.cn

[K06] 解析 URL 查询串
来源：http://fxf.nanxinkj.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://uyw.wangdashe.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://yzl.hesvh.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://qta.wangshuangyany.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ias.jiagoushi.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wmu.yonumen.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://sqv.fktsv.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://xzv.meibo888.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://pmz.zhongyouzk.top

[K07] 进制转换
来源：http://fgm.hongshengwenyu.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://iri.mhx1999.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hfo.hywenlv.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://voc.cucudq.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://efw.zhiwuduotai.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://nbq.9152youxi.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://bsm.ydjk.org.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mio.jinqigfzy.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://svg.ctjpmb.com

[K08] 二进制序列化（非 JSON）
来源：http://rpz.yj202588.top

Py:   pickle.dumps(obj)
来源：http://asg.hfpthk.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://umc.shzxlz.cn

JS:   v8.serialize(obj)        // Node
来源：http://emm.xingfuxueyuan.xyz

TS:   v8.serialize(obj)        // Node
来源：http://inp.jyoumei.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://tqt.jinghuilouyu.cn

Go:   encoding/gob
来源：http://msf.yuanzhike.top

Ruby: Marshal.dump(obj)
来源：http://lwm.yangfankeji.com

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://zls.smart0.xyz

================================================================================
来源：http://ixq.andypj.xyz

L. 网络请求
来源：http://inj.birdmap.top

================================================================================
来源：http://ylb.wangdashe.top

[L01] 发送 GET 请求
来源：http://oqq.zhijiandao.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://rcj.yj20258888.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://izp.tianlin.xyz

JS:   await fetch(url)
来源：http://jbk.yanxiufei.cn

TS:   await fetch(url)
来源：http://rem.vqdsnc.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://bvq.gogol.net.cn

Go:   resp, err := http.Get(url)
来源：http://wgd.chenjidiqi.icu

Ruby: Net::HTTP.get(URI(url))
来源：http://xgt.havefunace.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://yrf.sufxvd.cn

[L02] 发送 POST JSON
来源：http://udd.guannengcc.top

Py:   requests.post(url, json={"a": 1})
来源：http://ecn.gzhubu.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mrm.zhaomingkeji.xyz

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://vqj.wangshuangyany.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://okz.hywenlv.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://fyi.jianghu66.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mcr.xinyue.icu

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://bnv.epnwcf.com

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wug.hammf.cn

[L03] 设置自定义请求头
来源：http://yli.hysaishi.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ivb.hywenlv.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://tyb.ivvv.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://qva.zhengqikj.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://fax.ydjk.org.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://eyc.jinyuanbaomall.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ikw.ivvv.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://aos.yonumen.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wvf.jqgfzy.top

[L04] 设置超时
来源：http://wfw.cdnleiting.top

Py:   requests.get(url, timeout=5)
来源：http://eqy.ywan-chungtsiang.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ozk.snrcjt.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://fzp.hongshengwenyu.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://bwc.dashuyun.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mgw.yueranfly.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://atg.pengpengdd.cyou

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hsv.yj20258.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://uhk.bjfxy.top

[L05] 上传文件（multipart）
来源：http://xhg.havefunace.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://gyi.shanyushiyangtech.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ruh.52xcode.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://vih.guannengcc.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://pkh.zhiwuduotai.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://gvt.shanyushiyangkeji.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://dfn.shangyingyoupin.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://cjh.zhoulong.xyz

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://iru.xziqi.cn

[L06] 解析响应为 JSON
来源：http://rmm.zhongyouzk.top

Py:   resp.json()
来源：http://fvu.hammf.cn

PHP:  json_decode($body, true);
来源：http://gqp.cdnleiting.top

JS:   await resp.json()
来源：http://gct.cashguo.top

TS:   await resp.json()
来源：http://eyc.tian-w.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://paw.bbcook.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://jsm.gzhubu.top

Ruby: JSON.parse(resp.body)
来源：http://obc.tian-w.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ckv.zdbjq.cn

[L07] 处理 HTTP 状态码
来源：http://dmn.yongpay.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://osp.yj20258.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://qoa.fktsv.cn

JS:   resp.ok;  resp.status
来源：http://dqv.smart0.xyz

TS:   resp.ok;  resp.status
来源：http://duk.epnwcf.com

Java: resp.statusCode()
来源：http://nkr.andypj.xyz

Go:   resp.StatusCode
来源：http://hnt.hywenlv.cn

Ruby: resp.code.to_i
来源：http://qwd.0kj1m.cn

C#:   (int)resp.StatusCode
来源：http://gmx.shanyushiyangkeji.top

[L08] 并发请求多个地址
来源：http://vhj.pengpengdd.cyou

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://xli.shanyushiyangtech.top

PHP:  curl_multi_init() 系列
来源：http://ent.birdmap.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://jgw.vqdsnc.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://qie.hfpthk.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://qah.redwolf501.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ymo.nanxuanxn.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://efx.fzhhl.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://xou.hfpthk.cn

================================================================================
来源：http://ivk.jiagoushi.top

M. 命令行 / 进程 / 环境
来源：http://vai.fengsongda.top

================================================================================
来源：http://wqs.aibaodan.cn

[M01] 读取命令行参数
来源：http://xio.cheryme.top

Py:   sys.argv[1:]
来源：http://enf.sysykeji.top

PHP:  $argv;  $argc;
来源：http://ryq.aizwys.cn

JS:   process.argv.slice(2)
来源：http://cmv.feifeiyinyue.top

TS:   process.argv.slice(2)
来源：http://huw.jyoumei.cn

Java: args 数组（main 方法参数）
来源：http://opy.yvedp.cn

Go:   os.Args[1:]
来源：http://ows.daxiang520.top

Ruby: ARGV
来源：http://yke.316326.xyz

C#:   args 数组（Main 方法参数）
来源：http://fpt.cqqwz.cn

[M02] 读取环境变量
来源：http://kya.jqgfzy.top

Py:   os.environ.get("HOME")
来源：http://klv.ppjwa.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://thd.0kj1m.cn

JS:   process.env.HOME
来源：http://scv.fktsv.cn

TS:   process.env.HOME
来源：http://ibb.tarul.cn

Java: System.getenv("HOME")
来源：http://cbj.iojbl.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ded.gogol.net.cn

Ruby: ENV["HOME"]
来源：http://jiy.vqdsnc.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://onu.guowangkeji.top

[M03] 执行外部命令
来源：http://izw.vqdsnc.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://rig.zdqjudy.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://zvr.fehbvm.com

JS:   child_process.execSync("ls -l").toString()
来源：http://cxe.zhiwuduotai.top

TS:   child_process.execSync("ls -l").toString()
来源：http://ibv.nanxinkj.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://itf.hysaishi.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://glh.tarul.cn

Ruby: system("ls -l");  `ls -l`
来源：http://bpu.shanyushiyangkeji.top

C#:   Process.Start("ls", "-l");
来源：http://qno.guowangkeji.top

[M04] 获取当前工作目录
来源：http://fsq.yj202588.top

Py:   os.getcwd()
来源：http://ofr.9152youxi.cn

PHP:  getcwd();
来源：http://fxh.yangfankeji.com

JS:   process.cwd()
来源：http://stc.shangyingyoupin.top

TS:   process.cwd()
来源：http://wyn.jyoumei.cn

Java: Path.of("").toAbsolutePath()
来源：http://wua.chenzaomai.com

Go:   os.Getwd()
来源：http://jse.daxiang520.top

Ruby: Dir.pwd
来源：http://vas.xuanzx.com

C#:   Directory.GetCurrentDirectory()
来源：http://qik.0kj1m.cn

[M05] 设置退出码
来源：http://ybe.hysaishi.cn

Py:   sys.exit(1)
来源：http://yeo.jinqigfzy.top

PHP:  exit(1);
来源：http://xrs.tianlin.xyz

JS:   process.exit(1)
来源：http://wux.tianlin.xyz

TS:   process.exit(1)
来源：http://std.yueranfly.top

Java: System.exit(1)
来源：http://wga.wangdashe.top

Go:   os.Exit(1)
来源：http://kds.hfpthk.cn

Ruby: exit 1
来源：http://szo.snrcjt.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mlg.mhx1999.top

[M06] 向标准错误输出
来源：http://tur.epnwcf.com

Py:   print("err", file=sys.stderr)
来源：http://kfx.zycfv.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://lev.tianlin.xyz

JS:   console.error("err")
来源：http://pvm.quarkkingdee.top

TS:   console.error("err")
来源：http://xol.zhengqikj.top

Java: System.err.println("err")
来源：http://ame.iojbl.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hns.aizwys.cn

Ruby: warn "err"
来源：http://ots.jqgfzy.top

C#:   Console.Error.WriteLine("err")
来源：http://xwf.ydzc1.top

[M07] 判断是否为主入口
来源：http://nim.daria6918.cn


<!-- 参考信息 -->