代发 wailian999

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ihj.hfpthk.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://air.epnwcf.com

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://vnu.fzhhl.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://cuw.cashguo.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://gvd.zhijiandao.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ypu.gotoacloud.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://xyq.havefunace.top

================================================================================
来源：http://foo.zhoulong.xyz

J. 日期与时间
来源：http://nkw.aibaodan.cn

================================================================================
来源：http://vaf.jianghu66.top

[J01] 获取当前时间
来源：http://wpz.sweek.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://mph.jinqigufen.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://udi.jinyuanbaomall.cn

JS:   new Date();  Date.now()
来源：http://omq.sweek.top

TS:   new Date();  Date.now()
来源：http://jai.jqgfzy.top

Java: LocalDateTime.now();  Instant.now()
来源：http://qwb.ywan-chungtsiang.top

Go:   time.Now()
来源：http://sgf.yuxming.cn

Ruby: Time.now
来源：http://ebk.sysykeji.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://xkb.birdmap.top

[J02] 格式化输出
来源：http://qjw.cdnleiting.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hck.shanyushiyangkeji.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://wnr.yonumen.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://avj.havefunace.top

TS:   d.toISOString()
来源：http://bht.yuxming.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://qir.yongpay.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://cah.jinghuilouyu.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://naw.yangfankeji.com

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://wnr.xylfe.cn

[J03] 字符串解析为日期
来源：http://vhj.pycfn.com

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://opj.tanke756.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://cnc.daria6918.cn

JS:   new Date("2024-01-02")
来源：http://mbr.chenzaomai.com

TS:   new Date("2024-01-02")
来源：http://fnf.gzhubu.top

Java: LocalDate.parse("2024-01-02")
来源：http://kgw.yongpay.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://qdd.zdbjq.cn

Ruby: Date.parse("2024-01-02")
来源：http://xaq.xylfe.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://gzk.daxiang520.top

[J04] 时间戳与日期互转
来源：http://zru.cdnleiting.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://txd.bbcook.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://jsp.chenjidiqi.icu

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://gjq.ppjwa.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://wki.cashguo.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hhm.hnqzz.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://rii.sweek.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://pcl.tarul.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://kcy.wangshuangyany.cn

[J05] 时间加减（加 7 天）
来源：http://rju.shangyingyoupin.top

Py:   now + timedelta(days=7)
来源：http://wih.nanxinkj.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://qlu.feifeiyinyue.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hge.jianghu66.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ksi.fzhhl.top

Java: LocalDate.now().plusDays(7)
来源：http://qip.quarkkingdee.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ztk.sweek.top

Ruby: Time.now + 7 * 86400
来源：http://vwp.ywan-chungtsiang.top

C#:   DateTime.Now.AddDays(7)
来源：http://hzg.vqdsnc.cn

[J06] 计算两时间之差
来源：http://dol.birdmap.top

Py:   (end - start).total_seconds()
来源：http://iko.redwolf501.top

PHP:  $end->diff($start)->days;
来源：http://igu.cheryme.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ajt.zycfv.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://uhe.haohaochexian.top

Java: Duration.between(start, end).toSeconds()
来源：http://pte.uphjek.com

Go:   end.Sub(start).Hours()
来源：http://ozs.zhijiandao.cn

Ruby: end - start                 # 返回秒数
来源：http://sbw.ydjk.org.cn

C#:   (end - start).TotalSeconds
来源：http://jzc.dashuyun.cn

[J07] 比较两个日期
来源：http://dgu.aizwys.cn

Py:   d1 < d2;  d1 == d2
来源：http://tjj.hcnkem.com

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://dwm.jianghu66.top

JS:   d1.getTime() < d2.getTime()
来源：http://dcc.shangyingyoupin.top

TS:   d1.getTime() < d2.getTime()
来源：http://okf.yueranfly.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://gsf.shanyushiyangtech.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ofp.xylfe.cn

Ruby: d1 < d2;  d1 == d2
来源：http://jdy.cucudq.cn

C#:   d1 < d2;  d1 == d2
来源：http://mfi.316326.xyz

[J08] 提取年月日与星期
来源：http://iyb.zdbjq.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ekd.quarkkingdee.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://nsq.xuanzx.com

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://iep.hnqzz.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://gbw.sysykeji.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://itk.jinqigfzy.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://vjd.bbcook.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://kiq.zhiwuduotai.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://jmx.jianghu66.top

[J09] 时区处理
来源：http://rry.gzhubu.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ngc.redwolf501.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://qnw.sxryk.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://gen.guowangkeji.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://pyv.jinqigfzy.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://lqr.wangdashe.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://vot.zdbjq.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://sjn.haohaochexian.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://khl.chenzaomai.com

[J10] 取今天 / 本月第一天
来源：http://wgv.tanke756.top

Py:   date.today();  date.today().replace(day=1)
来源：http://thy.quarkkingdee.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://pbx.0kj1m.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hxy.fzhhl.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://aen.chenzaomai.com

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://uwq.bbcook.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://jon.zhixingplan.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://cpc.yueranfly.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ofd.jiagoushi.top

================================================================================
来源：http://pkg.sweek.top

K. JSON 与序列化
来源：http://zzi.havefunace.top

================================================================================
来源：http://fuz.zhongyouzk.top

[K01] 对象转 JSON 字符串
来源：http://tas.shzxlz.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://lvv.hysaishi.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hwx.gogol.net.cn

JS:   JSON.stringify(obj)
来源：http://zxn.mhx1999.top

TS:   JSON.stringify(obj)
来源：http://udk.zhixingplan.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://pvd.vqdsnc.cn

Go:   json.Marshal(obj)
来源：http://nsn.shzxlz.cn

Ruby: obj.to_json                                     // require "json"
来源：http://tbj.bbcook.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://umj.316326.xyz

[K02] JSON 字符串转对象
来源：http://fzy.sxryk.cn

Py:   json.loads(s)
来源：http://iqo.tarul.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://aet.yongpay.top

JS:   JSON.parse(s)
来源：http://xcj.zhijiandao.cn

TS:   JSON.parse(s)
来源：http://vrf.gogol.net.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ent.9152youxi.cn

Go:   json.Unmarshal(data, &v)
来源：http://vju.nanxuanxn.top

Ruby: JSON.parse(s)
来源：http://jld.cucudq.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://bxe.yangfankeji.com

[K03] JSON 美化输出（带缩进）
来源：http://hsq.quarkkingdee.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://pik.cashguo.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://qhn.jinghuilouyu.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://rza.fengsongda.top

TS:   JSON.stringify(obj, null, 2)
来源：http://rkv.gogol.net.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://mdk.zycfv.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://amc.hfpthk.cn

Ruby: JSON.pretty_generate(obj)
来源：http://ekz.shanyushiyangkeji.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ouu.xylfe.cn

[K04] 读取 JSON 文件
来源：http://bfj.hnxiangtu.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://exe.yj202588.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hyy.zhoulong.xyz

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://veo.shanyushiyangkeji.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://agg.shuidangran.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://xcr.nanxinkj.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://rrq.wangshuangyany.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://uwt.shanyushiyangtech.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://tpl.pycfn.com

[K05] 深拷贝对象
来源：http://yfc.ppjwa.cn

Py:   copy.deepcopy(obj)
来源：http://ffq.xuetiantiany.cn

PHP:  unserialize(serialize($obj));
来源：http://ryn.hfpthk.cn

JS:   structuredClone(obj)
来源：http://qdh.fehbvm.com

TS:   structuredClone(obj)
来源：http://zyq.zhongyouzk.top

Java: // 手写拷贝构造，或序列化往返
来源：http://xra.gaohongyu789.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://tyr.c1oappe.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ksb.jinghuilouyu.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://btl.ctjpmb.com

[K06] 解析 URL 查询串
来源：http://rcb.ywan-chungtsiang.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://cgu.shangyingyoupin.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://lcj.hfpthk.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://tyl.daria6918.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://urr.cqqwz.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://cfo.sjlbkw.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://rqx.yanxiufei.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://lzf.gzhubu.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://jun.chenzaomai.com

[K07] 进制转换
来源：http://uzb.hywenlv.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://alu.yj202588.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://mhw.ybcxt.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://wwp.jyoumei.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://rdb.jqgfzy.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://dzi.zhixingplan.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://zuo.mhx1999.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://gla.yangfankeji.com

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://pve.fehbvm.com

[K08] 二进制序列化（非 JSON）
来源：http://omd.kuanghao11.cn

Py:   pickle.dumps(obj)
来源：http://vpf.0kj1m.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://gze.ctjpmb.com

JS:   v8.serialize(obj)        // Node
来源：http://tux.nanxinkj.top

TS:   v8.serialize(obj)        // Node
来源：http://xnc.yfazqb.com

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://kcy.c1oappe.top

Go:   encoding/gob
来源：http://ubh.yvedp.cn

Ruby: Marshal.dump(obj)
来源：http://bqd.sxryk.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://tos.jinghuilouyu.cn

================================================================================
来源：http://wzz.xylfe.cn

L. 网络请求
来源：http://zoz.zhongyouzk.top

================================================================================
来源：http://tae.hcnkem.com

[L01] 发送 GET 请求
来源：http://olz.andypj.xyz

Py:   requests.get(url)                        # 第三方库 requests
来源：http://qze.chenlongwang.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://jix.hfpthk.cn

JS:   await fetch(url)
来源：http://jwg.yvedp.cn

TS:   await fetch(url)
来源：http://xzd.quarkkingdee.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://abj.yuanzhike.top

Go:   resp, err := http.Get(url)
来源：http://gsj.chenzaomai.com

Ruby: Net::HTTP.get(URI(url))
来源：http://rbv.redwolf501.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://aux.pycfn.com

[L02] 发送 POST JSON
来源：http://rdy.xuetiantiany.cn

Py:   requests.post(url, json={"a": 1})
来源：http://hjz.wangshuangyany.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ixi.ivvv.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://jjs.gaohongyu789.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://rlo.pengpengdd.cyou

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ctz.yfazqb.com

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://kno.gotoacloud.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://omj.fanxiaobao.xyz

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hnv.chenlongwang.top

[L03] 设置自定义请求头
来源：http://egz.jinqigfzy.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://jjw.chenjidiqi.icu

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://xeh.fzhhl.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://lte.cqqwz.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://dpq.9152youxi.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://fhz.ctjpmb.com

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://tjp.sysykeji.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://nhb.fktsv.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://xjm.svipenyu.cn

[L04] 设置超时
来源：http://uka.zdbjq.cn

Py:   requests.get(url, timeout=5)
来源：http://kgn.epnwcf.com

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ilj.vehdjk.com

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://sds.hcnkem.com

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://zvq.xingfuxueyuan.xyz

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wbv.xuetiantiany.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://jal.shangyingyoupin.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mhh.yuxming.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://kkq.cdnleiting.top

[L05] 上传文件（multipart）
来源：http://llp.shangyingyoupin.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://aol.yanxiufei.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://fpr.yfazqb.com

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ybk.xingfuxueyuan.xyz

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://nzs.316326.xyz

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://lam.zhengqikj.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ttk.zhaomingkeji.xyz

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://oob.cucudq.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://qvi.meibo888.top

[L06] 解析响应为 JSON
来源：http://ssr.wangshuangyany.cn

Py:   resp.json()
来源：http://zia.hnqzz.top

PHP:  json_decode($body, true);
来源：http://zbv.cucudq.cn

JS:   await resp.json()
来源：http://oly.ctjpmb.com

TS:   await resp.json()
来源：http://gdk.daria6918.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://xzs.uphjek.com

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://yel.vehdjk.com

Ruby: JSON.parse(resp.body)
来源：http://ego.zdqjudy.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://eoj.cdnleiting.top

[L07] 处理 HTTP 状态码
来源：http://drs.yj202588.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://lxs.zdqjudy.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://dki.cheryme.top

JS:   resp.ok;  resp.status
来源：http://iwe.shanyushiyangtech.top

TS:   resp.ok;  resp.status
来源：http://gtp.ydzc1.top

Java: resp.statusCode()
来源：http://gaf.guannengcc.top

Go:   resp.StatusCode
来源：http://irk.cucudq.cn

Ruby: resp.code.to_i
来源：http://aqj.52xcode.cn

C#:   (int)resp.StatusCode
来源：http://cal.jianghu66.top

[L08] 并发请求多个地址
来源：http://wmo.jqgfzy.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hvy.jinyuanbaomall.cn

PHP:  curl_multi_init() 系列
来源：http://eiz.cheryme.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://btr.hnqzz.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://npz.jqgfzy.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://vww.hesvh.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mnu.jiagoushi.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://zpi.pycfn.com

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ovl.yanxiufei.cn

================================================================================
来源：http://tmj.epnwcf.com

M. 命令行 / 进程 / 环境
来源：http://afz.jinyuanbaomall.cn

================================================================================
来源：http://wvr.xingfuxueyuan.xyz

[M01] 读取命令行参数
来源：http://kdw.xinyue.icu

Py:   sys.argv[1:]
来源：http://hhm.hywenlv.cn

PHP:  $argv;  $argc;
来源：http://joj.xuetiantiany.cn

JS:   process.argv.slice(2)
来源：http://fgh.gogol.net.cn

TS:   process.argv.slice(2)
来源：http://sxb.tian-w.cn

Java: args 数组（main 方法参数）
来源：http://uts.yonumen.top

Go:   os.Args[1:]
来源：http://naj.fanxiaobao.xyz

Ruby: ARGV
来源：http://szs.sxryk.cn

C#:   args 数组（Main 方法参数）
来源：http://gnh.cucudq.cn

[M02] 读取环境变量
来源：http://acg.ivvv.top

Py:   os.environ.get("HOME")
来源：http://xru.zhengqikj.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://abx.316326.xyz

JS:   process.env.HOME
来源：http://qqo.redwolf501.top

TS:   process.env.HOME
来源：http://hea.cheryme.top

Java: System.getenv("HOME")
来源：http://mve.yfazqb.com

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://nhf.ctjpmb.com

Ruby: ENV["HOME"]
来源：http://zdm.gzhubu.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://vjk.yangfankeji.com

[M03] 执行外部命令
来源：http://iri.fengsongda.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mur.guannengcc.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wqo.yvedp.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://kpe.daria6918.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://saz.hnxiangtu.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://phi.birdmap.top

Go:   exec.Command("ls", "-l").Output()
来源：http://mdj.quarkkingdee.top

Ruby: system("ls -l");  `ls -l`
来源：http://bwr.yj20258.top

C#:   Process.Start("ls", "-l");
来源：http://gph.ctjpmb.com

[M04] 获取当前工作目录
来源：http://kru.birdmap.top

Py:   os.getcwd()
来源：http://igx.hfpthk.cn

PHP:  getcwd();
来源：http://ifp.dashuyun.cn

JS:   process.cwd()
来源：http://agp.daria6918.cn

TS:   process.cwd()
来源：http://lwe.pycfn.com

Java: Path.of("").toAbsolutePath()
来源：http://ttu.c1oappe.top

Go:   os.Getwd()
来源：http://xuz.quarkkingdee.top

Ruby: Dir.pwd
来源：http://npz.haohaochexian.top

C#:   Directory.GetCurrentDirectory()
来源：http://epw.xinyue.icu

[M05] 设置退出码
来源：http://cbo.uphjek.com

Py:   sys.exit(1)
来源：http://edg.xuanzx.com

PHP:  exit(1);
来源：http://lno.cqqwz.cn

JS:   process.exit(1)
来源：http://dub.hcnkem.com

TS:   process.exit(1)
来源：http://obn.jqgufenzy.top

Java: System.exit(1)
来源：http://ajz.yueranfly.top

Go:   os.Exit(1)
来源：http://dwa.hongshengwenyu.top

Ruby: exit 1
来源：http://xpa.kuanghao11.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ham.xuanzx.com

[M06] 向标准错误输出
来源：http://cqw.ehwqpu.com

Py:   print("err", file=sys.stderr)
来源：http://cyn.feifeiyinyue.top


<!-- 参考信息 -->