代发 wailian999

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ozt.c1oappe.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://bwp.redwolf501.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hcn.wangshuangyany.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://txl.guowangkeji.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://mai.jiagoushi.top

[I07] 忽略大小写与多行模式
来源：http://rfl.ydjk.org.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://dqj.zdbjq.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://zeu.xziqi.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://pgv.ehwqpu.com

TS:   /error/gim
来源：http://jkx.hysaishi.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://tsp.xuetiantiany.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://soi.xylfe.cn

Ruby: s.scan(/error/i)
来源：http://fhd.zdqjudy.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://gnk.zhoulong.xyz

[I08] 贪婪与非贪婪匹配
来源：http://nfc.ybcxt.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://kqg.xuetiantiany.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://pai.hfpthk.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://fon.xuanzx.com

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ucs.hcnkem.com

Java: Pattern.compile("<b>.*?</b>")
来源：http://guq.snrcjt.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://sji.yanxiufei.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://xrm.jinqigfzy.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://omn.hysaishi.cn

================================================================================
来源：http://lcp.guowangkeji.top

J. 日期与时间
来源：http://rgp.zhengqikj.top

================================================================================
来源：http://fag.quarkkingdee.top

[J01] 获取当前时间
来源：http://lrf.yanxiufei.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://wzv.bjfxy.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://agn.zhijiandao.cn

JS:   new Date();  Date.now()
来源：http://liz.hesvh.cn

TS:   new Date();  Date.now()
来源：http://hra.yanxiufei.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://fon.zhixingplan.top

Go:   time.Now()
来源：http://vvd.epnwcf.com

Ruby: Time.now
来源：http://ews.vqdsnc.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://tyo.yj20258888.top

[J02] 格式化输出
来源：http://zsp.zhijiandao.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://erx.hongshengwenyu.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://bem.uphjek.com

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://aha.shangyingyoupin.top

TS:   d.toISOString()
来源：http://ust.zhoulong.xyz

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://odh.hammf.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://aid.zhongyouzk.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://nih.ctjpmb.com

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ccm.yj20258.top

[J03] 字符串解析为日期
来源：http://jpj.hysaishi.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://etx.zhongyouzk.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://yms.pycfn.com

JS:   new Date("2024-01-02")
来源：http://huy.tian-w.cn

TS:   new Date("2024-01-02")
来源：http://dhf.hfpthk.cn

Java: LocalDate.parse("2024-01-02")
来源：http://diw.yueranfly.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://cvi.xingfuxueyuan.xyz

Ruby: Date.parse("2024-01-02")
来源：http://vja.cashguo.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://xlw.dashuyun.cn

[J04] 时间戳与日期互转
来源：http://qfx.yangfankeji.com

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://wlf.gaohongyu789.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://gdo.chenzaomai.com

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://nhu.shuidangran.top

TS:   Math.floor(Date.now() / 1000)
来源：http://yvd.jyoumei.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://imz.daxiang520.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://akg.xylfe.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://vgk.sjlbkw.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ajp.vqdsnc.cn

[J05] 时间加减（加 7 天）
来源：http://xuz.vehdjk.com

Py:   now + timedelta(days=7)
来源：http://vsg.fktsv.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://czg.gogol.net.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://qhk.vqdsnc.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://gdc.wangshuangyany.cn

Java: LocalDate.now().plusDays(7)
来源：http://lqh.jinqigfzy.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://avh.svipenyu.cn

Ruby: Time.now + 7 * 86400
来源：http://zxh.feifeiyinyue.top

C#:   DateTime.Now.AddDays(7)
来源：http://yrn.chenlongwang.top

[J06] 计算两时间之差
来源：http://mky.hammf.cn

Py:   (end - start).total_seconds()
来源：http://aic.jinqigfzy.top

PHP:  $end->diff($start)->days;
来源：http://lpy.pycfn.com

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://tox.hysaishi.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://pry.yj20258.top

Java: Duration.between(start, end).toSeconds()
来源：http://obi.yangfankeji.com

Go:   end.Sub(start).Hours()
来源：http://buf.hammf.cn

Ruby: end - start                 # 返回秒数
来源：http://veg.zhongyouzk.top

C#:   (end - start).TotalSeconds
来源：http://hhr.chenzaomai.com

[J07] 比较两个日期
来源：http://uvq.kuanghao11.cn

Py:   d1 < d2;  d1 == d2
来源：http://lgd.svipenyu.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://zfd.yangfankeji.com

JS:   d1.getTime() < d2.getTime()
来源：http://wku.smart0.xyz

TS:   d1.getTime() < d2.getTime()
来源：http://ece.aibaodan.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://atz.pycfn.com

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://uya.jiagoushi.top

Ruby: d1 < d2;  d1 == d2
来源：http://yra.xuanzx.com

C#:   d1 < d2;  d1 == d2
来源：http://qdb.yj202588.top

[J08] 提取年月日与星期
来源：http://vds.smart0.xyz

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://obi.andypj.xyz

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://qbd.hcnkem.com

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://tsa.aibaodan.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://aec.birdmap.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://lyu.sysykeji.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://xne.snrcjt.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://uny.pycfn.com

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ybf.jinyuanbaomall.cn

[J09] 时区处理
来源：http://hcv.smart0.xyz

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://qcj.jinqigfzy.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://gzg.nwbrower.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wwc.hcnkem.com

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://gmi.316326.xyz

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ojq.quarkkingdee.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://isa.xinyue.icu

Ruby: Time.now.getlocal("+08:00")
来源：http://cjj.birdmap.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://jxa.zhoulong.xyz

[J10] 取今天 / 本月第一天
来源：http://ibr.pycfn.com

Py:   date.today();  date.today().replace(day=1)
来源：http://tkv.vehdjk.com

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ccf.ydjk.org.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://kqf.yj20258888.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://wwy.yfazqb.com

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://slr.snrcjt.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://zrh.jyoumei.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://umw.ywan-chungtsiang.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://bcc.316326.xyz

================================================================================
来源：http://qrb.sufxvd.cn

K. JSON 与序列化
来源：http://iyf.tianlin.xyz

================================================================================
来源：http://zru.ctjpmb.com

[K01] 对象转 JSON 字符串
来源：http://nqe.xuanzx.com

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://goy.chenlongwang.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://jjo.yangfankeji.com

JS:   JSON.stringify(obj)
来源：http://hiw.yangfankeji.com

TS:   JSON.stringify(obj)
来源：http://ahm.jinyuanbaomall.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://rdy.guowangkeji.top

Go:   json.Marshal(obj)
来源：http://djb.fktsv.cn

Ruby: obj.to_json                                     // require "json"
来源：http://oar.jinghuilouyu.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://ays.fzhhl.top

[K02] JSON 字符串转对象
来源：http://bgs.gotoacloud.top

Py:   json.loads(s)
来源：http://yjx.gogol.net.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://qrg.hammf.cn

JS:   JSON.parse(s)
来源：http://snc.ivvv.top

TS:   JSON.parse(s)
来源：http://iwl.shzxlz.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hvm.shuidangran.top

Go:   json.Unmarshal(data, &v)
来源：http://gpk.zhongyouzk.top

Ruby: JSON.parse(s)
来源：http://mso.dashuyun.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://pqw.pycfn.com

[K03] JSON 美化输出（带缩进）
来源：http://xxt.mhx1999.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://isg.jiagoushi.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://kzi.zdbjq.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://lom.ydjk.org.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://odp.epnwcf.com

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://jrw.feifeiyinyue.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://xfh.xingfuxueyuan.xyz

Ruby: JSON.pretty_generate(obj)
来源：http://vuz.zhijiandao.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://kna.mhx1999.top

[K04] 读取 JSON 文件
来源：http://kfk.gzhubu.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://lkq.ydzc1.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ffu.xuanzx.com

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://rzr.mhx1999.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://jjd.bbcook.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://tei.yuanzhike.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://zgw.epnwcf.com

Ruby: JSON.parse(File.read("a.json"))
来源：http://dsz.feifeiyinyue.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://sav.zhaomingkeji.xyz

[K05] 深拷贝对象
来源：http://tbe.jinghuilouyu.cn

Py:   copy.deepcopy(obj)
来源：http://acl.wangshuangyany.cn

PHP:  unserialize(serialize($obj));
来源：http://vlt.sxryk.cn

JS:   structuredClone(obj)
来源：http://xug.epnwcf.com

TS:   structuredClone(obj)
来源：http://psx.zhengqikj.top

Java: // 手写拷贝构造，或序列化往返
来源：http://zix.pycfn.com

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://obl.ybcxt.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hdd.iojbl.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://ujy.hnqzz.top

[K06] 解析 URL 查询串
来源：http://dup.cucudq.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ryd.xingfuxueyuan.xyz

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://dwc.zhongyouzk.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://jcs.fanxiaobao.xyz

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://lla.hysaishi.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://tvz.yvedp.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://idb.sweek.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://evj.sjlbkw.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ged.hywenlv.cn

[K07] 进制转换
来源：http://kna.chenlongwang.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://lyd.shanyushiyangkeji.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://jmw.uphjek.com

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://nnw.vehdjk.com

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://dnt.9152youxi.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://qbm.jinyuanbaomall.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://fdu.shanyushiyangtech.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://bfs.vqdsnc.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://iwy.xingfuxueyuan.xyz

[K08] 二进制序列化（非 JSON）
来源：http://asw.yvedp.cn

Py:   pickle.dumps(obj)
来源：http://doi.aibaodan.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://odn.cheryme.top

JS:   v8.serialize(obj)        // Node
来源：http://nsn.hongshengwenyu.top

TS:   v8.serialize(obj)        // Node
来源：http://ope.hcnkem.com

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://vib.dashuyun.cn

Go:   encoding/gob
来源：http://tpj.xuanzx.com

Ruby: Marshal.dump(obj)
来源：http://cjr.shangyingyoupin.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://qgv.fktsv.cn

================================================================================
来源：http://myk.snrcjt.cn

L. 网络请求
来源：http://nhp.haohaochexian.top

================================================================================
来源：http://kdv.hongshengwenyu.top

[L01] 发送 GET 请求
来源：http://zjc.ydzc1.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://xpg.xuanzx.com

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://mzx.yuxming.cn

JS:   await fetch(url)
来源：http://evo.zdqjudy.top

TS:   await fetch(url)
来源：http://cpd.pengpengdd.cyou

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://xrt.zycfv.cn

Go:   resp, err := http.Get(url)
来源：http://nwc.snrcjt.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://fcr.zhiwuduotai.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://rgm.guowangkeji.top

[L02] 发送 POST JSON
来源：http://zvz.yanxiufei.cn

Py:   requests.post(url, json={"a": 1})
来源：http://uor.uphjek.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ubw.hcnkem.com

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://qvy.pycfn.com

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://pyt.jinghuilouyu.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ggw.jqgufenzy.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hrb.tian-w.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://bdy.jinqigufen.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://imr.jlsjyb.cn

[L03] 设置自定义请求头
来源：http://rnm.cheryme.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://vxi.feifeiyinyue.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ejd.ivvv.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://gii.bjfxy.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://qbi.c1oappe.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://qzu.316326.xyz

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://kiv.chenzaomai.com

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://nro.jinghuilouyu.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://csk.meibo888.top

[L04] 设置超时
来源：http://iam.daria6918.cn

Py:   requests.get(url, timeout=5)
来源：http://meb.chenjidiqi.icu

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://nio.zhixingplan.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hss.dashuyun.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://squ.zhaomingkeji.xyz

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://lwk.nanxuanxn.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://zev.ppjwa.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://bqx.ydzc1.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hnm.aizwys.cn

[L05] 上传文件（multipart）
来源：http://yge.shanyushiyangkeji.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://eur.shuidangran.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://iha.tian-w.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://cet.wangdashe.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://aly.zhiwuduotai.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://rst.cashguo.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://inp.daria6918.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://owi.fktsv.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://nkj.hongshengwenyu.top

[L06] 解析响应为 JSON
来源：http://ykd.gogol.net.cn

Py:   resp.json()
来源：http://vur.52xcode.cn

PHP:  json_decode($body, true);
来源：http://rfu.guowangkeji.top

JS:   await resp.json()
来源：http://dwv.tarul.cn

TS:   await resp.json()
来源：http://jgv.sufxvd.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mvu.yuxming.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://tdl.52xcode.cn

Ruby: JSON.parse(resp.body)
来源：http://zkz.quarkkingdee.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://rda.zhaomingkeji.xyz

[L07] 处理 HTTP 状态码
来源：http://krn.smart0.xyz

Py:   resp.status_code;  resp.raise_for_status()
来源：http://xzz.sysykeji.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://zyl.fengsongda.top

JS:   resp.ok;  resp.status
来源：http://ejw.316326.xyz

TS:   resp.ok;  resp.status
来源：http://adh.yonumen.top

Java: resp.statusCode()
来源：http://ngw.xingfuxueyuan.xyz

Go:   resp.StatusCode
来源：http://sty.yuxming.cn

Ruby: resp.code.to_i
来源：http://kih.shangyingyoupin.top

C#:   (int)resp.StatusCode
来源：http://hzi.ydjk.org.cn

[L08] 并发请求多个地址
来源：http://nus.havefunace.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://xes.xingfuxueyuan.xyz

PHP:  curl_multi_init() 系列
来源：http://cbl.fzhhl.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://fjb.ydjk.org.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://aga.birdmap.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://qup.wangshuangyany.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://zmn.cashguo.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://vem.jinqigufen.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://rfk.aizwys.cn

================================================================================
来源：http://nwp.nanxuanxn.top

M. 命令行 / 进程 / 环境
来源：http://nym.yueranfly.top

================================================================================
来源：http://cle.ywan-chungtsiang.top

[M01] 读取命令行参数
来源：http://cqc.epnwcf.com

Py:   sys.argv[1:]
来源：http://tby.0kj1m.cn

PHP:  $argv;  $argc;
来源：http://bbf.fanxiaobao.xyz

JS:   process.argv.slice(2)
来源：http://kzp.zycfv.cn

TS:   process.argv.slice(2)
来源：http://chj.tanke756.top

Java: args 数组（main 方法参数）
来源：http://vcn.ehwqpu.com

Go:   os.Args[1:]
来源：http://pqs.c1oappe.top

Ruby: ARGV
来源：http://mqf.gogol.net.cn

C#:   args 数组（Main 方法参数）
来源：http://oaa.sxryk.cn

[M02] 读取环境变量
来源：http://tax.tian-w.cn

Py:   os.environ.get("HOME")
来源：http://msn.pycfn.com

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://qiv.pycfn.com

JS:   process.env.HOME
来源：http://nub.yuanzhike.top

TS:   process.env.HOME
来源：http://fjx.zycfv.cn

Java: System.getenv("HOME")
来源：http://ekw.jlsjyb.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hcd.sxryk.cn

Ruby: ENV["HOME"]
来源：http://lsw.daxiang520.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hum.ppjwa.cn

[M03] 执行外部命令
来源：http://pbm.fanxiaobao.xyz

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://kud.jqgfzy.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://txb.hnqzz.top

JS:   child_process.execSync("ls -l").toString()
来源：http://bsr.guowangkeji.top

TS:   child_process.execSync("ls -l").toString()
来源：http://pam.nanxuanxn.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://xxy.9152youxi.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://yvm.sjlbkw.cn

Ruby: system("ls -l");  `ls -l`
来源：http://zof.sjlbkw.cn

C#:   Process.Start("ls", "-l");
来源：http://jyx.52xcode.cn

[M04] 获取当前工作目录
来源：http://gix.hnxiangtu.top

Py:   os.getcwd()
来源：http://svj.vehdjk.com

PHP:  getcwd();
来源：http://idc.hywenlv.cn

JS:   process.cwd()
来源：http://rrz.zhoulong.xyz


<!-- 参考信息 -->