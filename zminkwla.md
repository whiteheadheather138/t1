代发 wailian999

J. 日期与时间
来源：http://cjy.iojbl.cn

================================================================================
来源：http://lzi.tianlin.xyz

[J01] 获取当前时间
来源：http://ahp.fengsongda.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://mzu.yonumen.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://cov.guowangkeji.top

JS:   new Date();  Date.now()
来源：http://odc.sxryk.cn

TS:   new Date();  Date.now()
来源：http://tgz.havefunace.top

Java: LocalDateTime.now();  Instant.now()
来源：http://mek.yangfankeji.com

Go:   time.Now()
来源：http://wia.shuidangran.top

Ruby: Time.now
来源：http://gtc.birdmap.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://iza.hesvh.cn

[J02] 格式化输出
来源：http://qxg.ybcxt.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://rln.jiagoushi.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://zvv.ydzc1.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://pmo.xuanzx.com

TS:   d.toISOString()
来源：http://vhq.pycfn.com

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://tah.vehdjk.com

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://rim.andypj.xyz

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://xse.vqdsnc.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://yhk.zhongyouzk.top

[J03] 字符串解析为日期
来源：http://kgo.guannengcc.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://dns.fehbvm.com

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://cdu.zhiwuduotai.top

JS:   new Date("2024-01-02")
来源：http://bfd.guannengcc.top

TS:   new Date("2024-01-02")
来源：http://mvp.wangshuangyany.cn

Java: LocalDate.parse("2024-01-02")
来源：http://mse.xuanzx.com

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://goy.gogol.net.cn

Ruby: Date.parse("2024-01-02")
来源：http://ypb.birdmap.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://xye.chenjidiqi.icu

[J04] 时间戳与日期互转
来源：http://rjx.vqdsnc.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hyp.bbcook.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://aut.316326.xyz

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://gxs.xinyue.icu

TS:   Math.floor(Date.now() / 1000)
来源：http://smu.jinghuilouyu.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://dnz.jyoumei.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://cti.zdbjq.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://qfj.zhoulong.xyz

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://nby.dianchejie.cn

[J05] 时间加减（加 7 天）
来源：http://ikg.hnqzz.top

Py:   now + timedelta(days=7)
来源：http://dev.hnxiangtu.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://kem.hesvh.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://vpw.birdmap.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://fnz.uphjek.com

Java: LocalDate.now().plusDays(7)
来源：http://ubp.jianghu66.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://jan.ydjk.org.cn

Ruby: Time.now + 7 * 86400
来源：http://hko.jinqigfzy.top

C#:   DateTime.Now.AddDays(7)
来源：http://ntb.yuxming.cn

[J06] 计算两时间之差
来源：http://kwa.zycfv.cn

Py:   (end - start).total_seconds()
来源：http://rzu.xuanzx.com

PHP:  $end->diff($start)->days;
来源：http://mvp.ctjpmb.com

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://gsl.xuetiantiany.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://wnd.uphjek.com

Java: Duration.between(start, end).toSeconds()
来源：http://fyq.tarul.cn

Go:   end.Sub(start).Hours()
来源：http://mhr.mhx1999.top

Ruby: end - start                 # 返回秒数
来源：http://mux.xingfuxueyuan.xyz

C#:   (end - start).TotalSeconds
来源：http://wbf.xinyue.icu

[J07] 比较两个日期
来源：http://flt.guannengcc.top

Py:   d1 < d2;  d1 == d2
来源：http://elz.shanyushiyangtech.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://siy.9152youxi.cn

JS:   d1.getTime() < d2.getTime()
来源：http://wsw.wangshuangyany.cn

TS:   d1.getTime() < d2.getTime()
来源：http://jwf.tanke756.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://xsl.chenlongwang.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://rhy.dianchejie.cn

Ruby: d1 < d2;  d1 == d2
来源：http://gxb.yuanzhike.top

C#:   d1 < d2;  d1 == d2
来源：http://bfi.uphjek.com

[J08] 提取年月日与星期
来源：http://ykw.zhaomingkeji.xyz

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://gkw.xingfuxueyuan.xyz

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://huk.yvedp.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ugv.jiagoushi.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://dqv.yj20258888.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://bao.nanxuanxn.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://lxp.guannengcc.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ukn.fktsv.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://fqa.jinyuanbaomall.cn

[J09] 时区处理
来源：http://irl.xinyue.icu

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://sha.9152youxi.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://kry.ehwqpu.com

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://avq.xingfuxueyuan.xyz

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://dwt.yonumen.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://xfs.cdnleiting.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://owp.9152youxi.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://ewi.zdbjq.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://fup.gzhubu.top

[J10] 取今天 / 本月第一天
来源：http://ydo.zhijiandao.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://exl.meibo888.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://srx.uphjek.com

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://xhg.yj20258888.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://dri.snrcjt.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://nco.cdnleiting.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://vsn.zhiwuduotai.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://gdh.gogol.net.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://pjc.daria6918.cn

================================================================================
来源：http://eqj.sufxvd.cn

K. JSON 与序列化
来源：http://egm.uphjek.com

================================================================================
来源：http://yie.zdbjq.cn

[K01] 对象转 JSON 字符串
来源：http://znb.sweek.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://lkh.yonumen.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://wrs.shzxlz.cn

JS:   JSON.stringify(obj)
来源：http://smn.fengsongda.top

TS:   JSON.stringify(obj)
来源：http://jsp.jlsjyb.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://nfm.ivvv.top

Go:   json.Marshal(obj)
来源：http://axj.yonumen.top

Ruby: obj.to_json                                     // require "json"
来源：http://jky.bbcook.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://rve.sufxvd.cn

[K02] JSON 字符串转对象
来源：http://sro.dashuyun.cn

Py:   json.loads(s)
来源：http://gva.jyoumei.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://tcl.fehbvm.com

JS:   JSON.parse(s)
来源：http://jlo.yj20258888.top

TS:   JSON.parse(s)
来源：http://xow.hesvh.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://fgc.hnxiangtu.top

Go:   json.Unmarshal(data, &v)
来源：http://lim.dashuyun.cn

Ruby: JSON.parse(s)
来源：http://ohr.yuxming.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://rnw.yj202588.top

[K03] JSON 美化输出（带缩进）
来源：http://zdy.tianlin.xyz

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://zrf.zhoulong.xyz

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://sjt.zhixingplan.top

JS:   JSON.stringify(obj, null, 2)
来源：http://bnp.tanke756.top

TS:   JSON.stringify(obj, null, 2)
来源：http://llx.zhengqikj.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://gkp.xingfuxueyuan.xyz

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ros.andypj.xyz

Ruby: JSON.pretty_generate(obj)
来源：http://nov.tian-w.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://dyi.kuanghao11.cn

[K04] 读取 JSON 文件
来源：http://ulu.zycfv.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://jgk.cdnleiting.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hud.chenzaomai.com

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://cdr.yanxiufei.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://tea.hfpthk.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hhd.fzhhl.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://xyb.shuidangran.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://lld.feifeiyinyue.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://xhm.zhaomingkeji.xyz

[K05] 深拷贝对象
来源：http://qnt.xingfuxueyuan.xyz

Py:   copy.deepcopy(obj)
来源：http://xos.hcnkem.com

PHP:  unserialize(serialize($obj));
来源：http://vpl.xuetiantiany.cn

JS:   structuredClone(obj)
来源：http://xlj.hcnkem.com

TS:   structuredClone(obj)
来源：http://vml.jinqigufen.top

Java: // 手写拷贝构造，或序列化往返
来源：http://ema.guowangkeji.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://klp.yvedp.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://lbx.chenlongwang.top

C#:   // 序列化往返，或自定义 Clone
来源：http://fwe.mhx1999.top

[K06] 解析 URL 查询串
来源：http://djt.tarul.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://evr.hnqzz.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://pdj.wangshuangyany.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://uzm.zhaomingkeji.xyz

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://zjo.tanke756.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://adu.yonumen.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://hcr.snrcjt.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://bpx.pycfn.com

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://iju.cucudq.cn

[K07] 进制转换
来源：http://spe.xylfe.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://jxb.yanxiufei.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://svx.yfazqb.com

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://zty.jianghu66.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://xfs.xinyue.icu

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://qhu.hesvh.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://xlg.yvedp.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://xsp.yonumen.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://kdi.shanyushiyangtech.top

[K08] 二进制序列化（非 JSON）
来源：http://dat.xingfuxueyuan.xyz

Py:   pickle.dumps(obj)
来源：http://jib.epnwcf.com

PHP:  serialize($obj);  unserialize($s);
来源：http://ufm.fktsv.cn

JS:   v8.serialize(obj)        // Node
来源：http://npb.chenjidiqi.icu

TS:   v8.serialize(obj)        // Node
来源：http://sow.vqdsnc.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://vbx.jqgufenzy.top

Go:   encoding/gob
来源：http://otz.redwolf501.top

Ruby: Marshal.dump(obj)
来源：http://gpb.vqdsnc.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ghj.daxiang520.top

================================================================================
来源：http://gku.shanyushiyangkeji.top

L. 网络请求
来源：http://vwu.ivvv.top

================================================================================
来源：http://byo.jinqigufen.top

[L01] 发送 GET 请求
来源：http://ygs.jqgfzy.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://qbo.vqdsnc.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://xab.xuanzx.com

JS:   await fetch(url)
来源：http://nbg.dianchejie.cn

TS:   await fetch(url)
来源：http://hsv.cheryme.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://tox.tarul.cn

Go:   resp, err := http.Get(url)
来源：http://fgy.yfazqb.com

Ruby: Net::HTTP.get(URI(url))
来源：http://kpv.tarul.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://fba.vehdjk.com

[L02] 发送 POST JSON
来源：http://smk.dianchejie.cn

Py:   requests.post(url, json={"a": 1})
来源：http://iaz.zdbjq.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wwm.hfpthk.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://khw.jlsjyb.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ukj.316326.xyz

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://jbk.svipenyu.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://nuc.jinghuilouyu.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://dev.yonumen.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://opq.zdbjq.cn

[L03] 设置自定义请求头
来源：http://jty.zhiwuduotai.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ejz.hongshengwenyu.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://vpr.fehbvm.com

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ayu.ywan-chungtsiang.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://kmk.meibo888.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://eck.tianlin.xyz

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://jkt.uphjek.com

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://fbz.uphjek.com

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ezd.uphjek.com

[L04] 设置超时
来源：http://khm.dianchejie.cn

Py:   requests.get(url, timeout=5)
来源：http://htn.daria6918.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://myq.chenjidiqi.icu

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://veu.ybcxt.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://cnj.hnqzz.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ydl.yueranfly.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://xtx.yj202588.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://bey.xziqi.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://kzb.guowangkeji.top

[L05] 上传文件（multipart）
来源：http://zru.hcnkem.com

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wbo.jyoumei.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ehy.fehbvm.com

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ucq.fanxiaobao.xyz

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://tfn.kuanghao11.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://zil.jinghuilouyu.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://tye.tanke756.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://qso.tanke756.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mdf.zhijiandao.cn

[L06] 解析响应为 JSON
来源：http://ahu.xingfuxueyuan.xyz

Py:   resp.json()
来源：http://ges.ybcxt.top

PHP:  json_decode($body, true);
来源：http://ayb.bbcook.cn

JS:   await resp.json()
来源：http://pzw.daxiang520.top

TS:   await resp.json()
来源：http://ifn.pycfn.com

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://anl.cqqwz.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://gsf.xingfuxueyuan.xyz

Ruby: JSON.parse(resp.body)
来源：http://ynq.fengsongda.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://bna.hysaishi.cn

[L07] 处理 HTTP 状态码
来源：http://red.chenzaomai.com

Py:   resp.status_code;  resp.raise_for_status()
来源：http://syd.jqgfzy.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ujp.xziqi.cn

JS:   resp.ok;  resp.status
来源：http://uxr.zhengqikj.top

TS:   resp.ok;  resp.status
来源：http://whj.yvedp.cn

Java: resp.statusCode()
来源：http://smn.yfazqb.com

Go:   resp.StatusCode
来源：http://puf.andypj.xyz

Ruby: resp.code.to_i
来源：http://wee.shanyushiyangkeji.top

C#:   (int)resp.StatusCode
来源：http://qsh.chenlongwang.top

[L08] 并发请求多个地址
来源：http://zkv.sxryk.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://pyw.uphjek.com

PHP:  curl_multi_init() 系列
来源：http://zcb.zhengqikj.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://vqy.jinghuilouyu.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://qes.sjlbkw.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://nwr.yanxiufei.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://yvy.yangfankeji.com

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://uce.pycfn.com

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://oim.jyoumei.cn

================================================================================
来源：http://ebo.jinqigfzy.top

M. 命令行 / 进程 / 环境
来源：http://xxl.hysaishi.cn

================================================================================
来源：http://qve.cdnleiting.top

[M01] 读取命令行参数
来源：http://dad.svipenyu.cn

Py:   sys.argv[1:]
来源：http://dku.gotoacloud.top

PHP:  $argv;  $argc;
来源：http://cbo.tanke756.top

JS:   process.argv.slice(2)
来源：http://vxb.yfazqb.com

TS:   process.argv.slice(2)
来源：http://slv.sjlbkw.cn

Java: args 数组（main 方法参数）
来源：http://pym.hcnkem.com

Go:   os.Args[1:]
来源：http://lta.ydzc1.top

Ruby: ARGV
来源：http://ouu.wangdashe.top

C#:   args 数组（Main 方法参数）
来源：http://xpy.yueranfly.top

[M02] 读取环境变量
来源：http://bbj.ydjk.org.cn

Py:   os.environ.get("HOME")
来源：http://fou.jinyuanbaomall.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wma.hysaishi.cn

JS:   process.env.HOME
来源：http://ypb.zdbjq.cn

TS:   process.env.HOME
来源：http://ifs.ybcxt.top

Java: System.getenv("HOME")
来源：http://sdc.sxryk.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://sfs.shangyingyoupin.top

Ruby: ENV["HOME"]
来源：http://fik.nanxuanxn.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://unf.jinghuilouyu.cn

[M03] 执行外部命令
来源：http://yci.hnqzz.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://svs.nanxuanxn.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://dnx.wangdashe.top

JS:   child_process.execSync("ls -l").toString()
来源：http://nrd.cqqwz.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://tsi.feifeiyinyue.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://pzf.nanxuanxn.top

Go:   exec.Command("ls", "-l").Output()
来源：http://fcj.aizwys.cn

Ruby: system("ls -l");  `ls -l`
来源：http://bbs.hysaishi.cn

C#:   Process.Start("ls", "-l");
来源：http://cqd.yongpay.top

[M04] 获取当前工作目录
来源：http://zbv.xylfe.cn

Py:   os.getcwd()
来源：http://mej.sysykeji.top

PHP:  getcwd();
来源：http://gxf.chenjidiqi.icu

JS:   process.cwd()
来源：http://rfq.nanxuanxn.top

TS:   process.cwd()
来源：http://gss.epnwcf.com

Java: Path.of("").toAbsolutePath()
来源：http://akd.jyoumei.cn

Go:   os.Getwd()
来源：http://jji.guowangkeji.top

Ruby: Dir.pwd
来源：http://efq.jqgfzy.top

C#:   Directory.GetCurrentDirectory()
来源：http://cpd.tarul.cn

[M05] 设置退出码
来源：http://shi.iojbl.cn

Py:   sys.exit(1)
来源：http://rna.snrcjt.cn

PHP:  exit(1);
来源：http://she.wangshuangyany.cn

JS:   process.exit(1)
来源：http://gob.shanyushiyangkeji.top

TS:   process.exit(1)
来源：http://ksq.havefunace.top

Java: System.exit(1)
来源：http://aby.hammf.cn

Go:   os.Exit(1)
来源：http://ihq.mhx1999.top

Ruby: exit 1
来源：http://nqa.sxryk.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://kji.fengsongda.top

[M06] 向标准错误输出
来源：http://prn.cdnleiting.top

Py:   print("err", file=sys.stderr)
来源：http://ksl.dashuyun.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://ovp.jinyuanbaomall.cn

JS:   console.error("err")
来源：http://qha.nanxinkj.top

TS:   console.error("err")
来源：http://vrs.nanxinkj.top

Java: System.err.println("err")
来源：http://zmi.dashuyun.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://cdc.hesvh.cn

Ruby: warn "err"
来源：http://wsr.zhaomingkeji.xyz

C#:   Console.Error.WriteLine("err")
来源：http://dar.gogol.net.cn

[M07] 判断是否为主入口
来源：http://twd.sweek.top


<!-- 参考信息 -->