代发 wailian999

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://lez.epnwcf.com

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://mwq.zhongyouzk.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://jyi.vehdjk.com

================================================================================
来源：http://goc.guowangkeji.top

J. 日期与时间
来源：http://xiy.hesvh.cn

================================================================================
来源：http://zyb.sweek.top

[J01] 获取当前时间
来源：http://hzw.guannengcc.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://grd.ywan-chungtsiang.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ioc.ppjwa.cn

JS:   new Date();  Date.now()
来源：http://mjv.shzxlz.cn

TS:   new Date();  Date.now()
来源：http://tks.snrcjt.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://qak.tarul.cn

Go:   time.Now()
来源：http://sgj.gotoacloud.top

Ruby: Time.now
来源：http://juy.redwolf501.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://mil.jlsjyb.cn

[J02] 格式化输出
来源：http://exs.daria6918.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://soc.ctjpmb.com

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://kvm.yj20258.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://twa.zhaomingkeji.xyz

TS:   d.toISOString()
来源：http://pxx.yfazqb.com

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://pnp.meibo888.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://vjs.zhijiandao.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ghv.yonumen.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://xgx.zhongyouzk.top

[J03] 字符串解析为日期
来源：http://hbf.bbcook.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ycq.sufxvd.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://scj.jyoumei.cn

JS:   new Date("2024-01-02")
来源：http://ywc.shzxlz.cn

TS:   new Date("2024-01-02")
来源：http://kpe.yuxming.cn

Java: LocalDate.parse("2024-01-02")
来源：http://pat.jqgfzy.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://sgi.fzhhl.top

Ruby: Date.parse("2024-01-02")
来源：http://vor.xylfe.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://yij.jiagoushi.top

[J04] 时间戳与日期互转
来源：http://poz.yj202588.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://qho.kuanghao11.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://zkh.chenzaomai.com

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://cba.haohaochexian.top

TS:   Math.floor(Date.now() / 1000)
来源：http://qbk.cashguo.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://rne.yj202588.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://rgd.0kj1m.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://klf.316326.xyz

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://vhv.zhongyouzk.top

[J05] 时间加减（加 7 天）
来源：http://hgk.zhengqikj.top

Py:   now + timedelta(days=7)
来源：http://xuk.xylfe.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://mnf.ywan-chungtsiang.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://aiv.gaohongyu789.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://igb.yj20258888.top

Java: LocalDate.now().plusDays(7)
来源：http://qnv.jlsjyb.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ops.yj202588.top

Ruby: Time.now + 7 * 86400
来源：http://feq.yfazqb.com

C#:   DateTime.Now.AddDays(7)
来源：http://goe.shanyushiyangtech.top

[J06] 计算两时间之差
来源：http://ohh.snrcjt.cn

Py:   (end - start).total_seconds()
来源：http://kfl.cheryme.top

PHP:  $end->diff($start)->days;
来源：http://ufb.xziqi.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://rgp.zhixingplan.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ity.jinyuanbaomall.cn

Java: Duration.between(start, end).toSeconds()
来源：http://jux.yvedp.cn

Go:   end.Sub(start).Hours()
来源：http://wwj.nanxinkj.top

Ruby: end - start                 # 返回秒数
来源：http://edl.zhijiandao.cn

C#:   (end - start).TotalSeconds
来源：http://wkn.yj20258888.top

[J07] 比较两个日期
来源：http://jud.cheryme.top

Py:   d1 < d2;  d1 == d2
来源：http://ack.smart0.xyz

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ink.zhoulong.xyz

JS:   d1.getTime() < d2.getTime()
来源：http://una.snrcjt.cn

TS:   d1.getTime() < d2.getTime()
来源：http://nde.zhoulong.xyz

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hkw.shanyushiyangtech.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://nnn.xziqi.cn

Ruby: d1 < d2;  d1 == d2
来源：http://knu.yfazqb.com

C#:   d1 < d2;  d1 == d2
来源：http://dks.gzhubu.top

[J08] 提取年月日与星期
来源：http://eop.haohaochexian.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ise.shanyushiyangkeji.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ywr.chenjidiqi.icu

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://gyp.snrcjt.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://mui.sysykeji.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://lfq.yj20258888.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hxv.xingfuxueyuan.xyz

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ecy.uphjek.com

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://mxe.cucudq.cn

[J09] 时区处理
来源：http://czc.shzxlz.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://cwi.wangdashe.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ewj.chenlongwang.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ayy.jinghuilouyu.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://aue.nanxuanxn.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://pqb.c1oappe.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://fuh.tarul.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://xtn.redwolf501.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://iiz.kuanghao11.cn

[J10] 取今天 / 本月第一天
来源：http://nny.fengsongda.top

Py:   date.today();  date.today().replace(day=1)
来源：http://asr.nanxinkj.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ozf.yueranfly.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://fsf.vehdjk.com

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://fzi.jinqigfzy.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://wmw.nanxuanxn.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hck.yanxiufei.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://grk.jqgfzy.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://idx.ctjpmb.com

================================================================================
来源：http://gpp.dianchejie.cn

K. JSON 与序列化
来源：http://xvr.jlsjyb.cn

================================================================================
来源：http://eks.shanyushiyangkeji.top

[K01] 对象转 JSON 字符串
来源：http://ueg.sweek.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ijl.redwolf501.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://bbn.zhijiandao.cn

JS:   JSON.stringify(obj)
来源：http://mbn.tanke756.top

TS:   JSON.stringify(obj)
来源：http://nvk.feifeiyinyue.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://gds.yongpay.top

Go:   json.Marshal(obj)
来源：http://kpi.cheryme.top

Ruby: obj.to_json                                     // require "json"
来源：http://tgs.cqqwz.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://wrt.chenlongwang.top

[K02] JSON 字符串转对象
来源：http://nek.zhaomingkeji.xyz

Py:   json.loads(s)
来源：http://smq.yvedp.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://fps.haohaochexian.top

JS:   JSON.parse(s)
来源：http://riz.shanyushiyangkeji.top

TS:   JSON.parse(s)
来源：http://cez.ehwqpu.com

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://nky.yuxming.cn

Go:   json.Unmarshal(data, &v)
来源：http://xmy.sweek.top

Ruby: JSON.parse(s)
来源：http://ofw.zhaomingkeji.xyz

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://atm.yongpay.top

[K03] JSON 美化输出（带缩进）
来源：http://lwm.ybcxt.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://gos.birdmap.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://czy.cqqwz.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://jqe.bjfxy.top

TS:   JSON.stringify(obj, null, 2)
来源：http://whc.shanyushiyangtech.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://tnz.yj202588.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://lyr.guowangkeji.top

Ruby: JSON.pretty_generate(obj)
来源：http://ejp.xuetiantiany.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://kos.gotoacloud.top

[K04] 读取 JSON 文件
来源：http://xwf.zhengqikj.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://axz.cqqwz.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://qdl.chenzaomai.com

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://kdy.gzhubu.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://vsn.hywenlv.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://aap.cucudq.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hxp.tian-w.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://tsz.ydjk.org.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://bhl.sysykeji.top

[K05] 深拷贝对象
来源：http://zhf.zhaomingkeji.xyz

Py:   copy.deepcopy(obj)
来源：http://vvp.hnxiangtu.top

PHP:  unserialize(serialize($obj));
来源：http://fjg.aibaodan.cn

JS:   structuredClone(obj)
来源：http://ojw.dianchejie.cn

TS:   structuredClone(obj)
来源：http://hra.aizwys.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://vzd.nanxuanxn.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://xwq.tianlin.xyz

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://kpi.52xcode.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://aey.zhengqikj.top

[K06] 解析 URL 查询串
来源：http://fxh.gogol.net.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://mpj.shzxlz.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ktp.fanxiaobao.xyz

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://qra.yvedp.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://kog.ydzc1.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://yzl.havefunace.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://fxs.tianlin.xyz

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://mzj.haohaochexian.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://tfk.dashuyun.cn

[K07] 进制转换
来源：http://dzo.zhongyouzk.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://gii.xuanzx.com

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://uqi.xuanzx.com

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://val.xylfe.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://muu.zdbjq.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ruo.9152youxi.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://tpf.aibaodan.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://aff.xinyue.icu

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://mbp.yj20258.top

[K08] 二进制序列化（非 JSON）
来源：http://hgo.gotoacloud.top

Py:   pickle.dumps(obj)
来源：http://qyq.cucudq.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://xpd.tarul.cn

JS:   v8.serialize(obj)        // Node
来源：http://qzo.nanxuanxn.top

TS:   v8.serialize(obj)        // Node
来源：http://zav.quarkkingdee.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://mqu.xziqi.cn

Go:   encoding/gob
来源：http://cik.hfpthk.cn

Ruby: Marshal.dump(obj)
来源：http://tet.zhoulong.xyz

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://tfo.316326.xyz

================================================================================
来源：http://utj.zhaomingkeji.xyz

L. 网络请求
来源：http://mrd.fengsongda.top

================================================================================
来源：http://ltl.xinyue.icu

[L01] 发送 GET 请求
来源：http://swh.jqgfzy.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ryl.shuidangran.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://kcl.smart0.xyz

JS:   await fetch(url)
来源：http://vvo.ivvv.top

TS:   await fetch(url)
来源：http://lsw.pycfn.com

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ard.gzhubu.top

Go:   resp, err := http.Get(url)
来源：http://gwk.zdqjudy.top

Ruby: Net::HTTP.get(URI(url))
来源：http://nrr.cqqwz.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://kxn.shuidangran.top

[L02] 发送 POST JSON
来源：http://bwh.andypj.xyz

Py:   requests.post(url, json={"a": 1})
来源：http://ugi.feifeiyinyue.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://dzw.chenzaomai.com

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ixs.hammf.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://pvp.uphjek.com

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://kcn.dashuyun.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://tdj.nanxuanxn.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://jrl.ybcxt.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mef.fehbvm.com

[L03] 设置自定义请求头
来源：http://vfw.meibo888.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://anx.xinyue.icu

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://lig.hnxiangtu.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://grs.cashguo.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://cfa.xziqi.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://nnm.shuidangran.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://cts.chenjidiqi.icu

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ouv.redwolf501.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ipn.hesvh.cn

[L04] 设置超时
来源：http://kma.tarul.cn

Py:   requests.get(url, timeout=5)
来源：http://qdh.daria6918.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://zqu.yj202588.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://avv.52xcode.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://lgx.hysaishi.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://min.aibaodan.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://dwj.316326.xyz

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mjj.yj20258888.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://dih.xuetiantiany.cn

[L05] 上传文件（multipart）
来源：http://exm.yangfankeji.com

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://llb.fktsv.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://blc.redwolf501.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://qjd.jyoumei.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://lev.quarkkingdee.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://vct.yangfankeji.com

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wpa.daria6918.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://jdn.yanxiufei.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://kxs.smart0.xyz

[L06] 解析响应为 JSON
来源：http://epl.meibo888.top

Py:   resp.json()
来源：http://gxe.haohaochexian.top

PHP:  json_decode($body, true);
来源：http://uoi.wangdashe.top

JS:   await resp.json()
来源：http://ogx.wangshuangyany.cn

TS:   await resp.json()
来源：http://mes.hesvh.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://pbw.ywan-chungtsiang.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://zzq.fehbvm.com

Ruby: JSON.parse(resp.body)
来源：http://grr.meibo888.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://rzs.pycfn.com

[L07] 处理 HTTP 状态码
来源：http://iix.jlsjyb.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ybk.meibo888.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://qqp.xylfe.cn

JS:   resp.ok;  resp.status
来源：http://lvl.shuidangran.top

TS:   resp.ok;  resp.status
来源：http://clv.fzhhl.top

Java: resp.statusCode()
来源：http://qkv.ywan-chungtsiang.top

Go:   resp.StatusCode
来源：http://sxq.yj20258888.top

Ruby: resp.code.to_i
来源：http://arh.dashuyun.cn

C#:   (int)resp.StatusCode
来源：http://iyd.daria6918.cn

[L08] 并发请求多个地址
来源：http://fyz.nanxinkj.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://par.yj202588.top

PHP:  curl_multi_init() 系列
来源：http://tbm.yj202588.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ysd.cdnleiting.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://haq.yj20258.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://fll.zhijiandao.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://oky.jyoumei.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mjp.cdnleiting.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ici.guannengcc.top

================================================================================
来源：http://ckk.jiagoushi.top

M. 命令行 / 进程 / 环境
来源：http://oil.daria6918.cn

================================================================================
来源：http://cqj.ehwqpu.com

[M01] 读取命令行参数
来源：http://hum.yueranfly.top

Py:   sys.argv[1:]
来源：http://ccl.shanyushiyangkeji.top

PHP:  $argv;  $argc;
来源：http://qgs.xinyue.icu

JS:   process.argv.slice(2)
来源：http://lfe.dashuyun.cn

TS:   process.argv.slice(2)
来源：http://iur.smart0.xyz

Java: args 数组（main 方法参数）
来源：http://vft.xuanzx.com

Go:   os.Args[1:]
来源：http://mid.hcnkem.com

Ruby: ARGV
来源：http://xxd.jqgfzy.top

C#:   args 数组（Main 方法参数）
来源：http://ozw.ybcxt.top

[M02] 读取环境变量
来源：http://jql.zycfv.cn

Py:   os.environ.get("HOME")
来源：http://izt.kuanghao11.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://eqv.hysaishi.cn

JS:   process.env.HOME
来源：http://vfc.gaohongyu789.top

TS:   process.env.HOME
来源：http://qzq.jiagoushi.top

Java: System.getenv("HOME")
来源：http://bdw.yuxming.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ksi.tanke756.top

Ruby: ENV["HOME"]
来源：http://eua.nanxuanxn.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://caf.jqgfzy.top

[M03] 执行外部命令
来源：http://oga.jinqigfzy.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://nse.fzhhl.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://xqr.sweek.top

JS:   child_process.execSync("ls -l").toString()
来源：http://cbi.hnxiangtu.top

TS:   child_process.execSync("ls -l").toString()
来源：http://udt.iojbl.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://tuu.bbcook.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://tmb.mhx1999.top

Ruby: system("ls -l");  `ls -l`
来源：http://zcb.cqqwz.cn

C#:   Process.Start("ls", "-l");
来源：http://pnz.jyoumei.cn

[M04] 获取当前工作目录
来源：http://hwv.jianghu66.top

Py:   os.getcwd()
来源：http://fup.hammf.cn

PHP:  getcwd();
来源：http://gax.tian-w.cn

JS:   process.cwd()
来源：http://uxq.sysykeji.top

TS:   process.cwd()
来源：http://ads.ehwqpu.com

Java: Path.of("").toAbsolutePath()
来源：http://ndl.ehwqpu.com

Go:   os.Getwd()
来源：http://axg.cheryme.top

Ruby: Dir.pwd
来源：http://ujj.316326.xyz

C#:   Directory.GetCurrentDirectory()
来源：http://rxn.shanyushiyangtech.top

[M05] 设置退出码
来源：http://urt.feifeiyinyue.top

Py:   sys.exit(1)
来源：http://njs.shangyingyoupin.top

PHP:  exit(1);
来源：http://xkc.jinyuanbaomall.cn

JS:   process.exit(1)
来源：http://sqw.ybcxt.top

TS:   process.exit(1)
来源：http://uop.shzxlz.cn

Java: System.exit(1)
来源：http://uie.zhaomingkeji.xyz

Go:   os.Exit(1)
来源：http://owa.hnxiangtu.top

Ruby: exit 1
来源：http://wku.bjfxy.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://bcn.cucudq.cn

[M06] 向标准错误输出
来源：http://rrq.aibaodan.cn

Py:   print("err", file=sys.stderr)
来源：http://elt.xziqi.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://bzj.iojbl.cn

JS:   console.error("err")
来源：http://mms.xingfuxueyuan.xyz

TS:   console.error("err")
来源：http://gtq.bjfxy.top

Java: System.err.println("err")
来源：http://zwf.havefunace.top


<!-- 参考信息 -->