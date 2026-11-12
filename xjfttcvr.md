代发 wailian999

Java: s.split("\\s*,\\s*")
来源：http://qfh.sxryk.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://lmo.zdbjq.cn

Ruby: s.split(/\s*,\s*/)
来源：http://dhy.jinqigufen.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://qfe.zdqjudy.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://brd.zhoulong.xyz

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://vfw.ydzc1.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://xpb.jinyuanbaomall.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://llq.yuanzhike.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ajo.aibaodan.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://xzg.jlsjyb.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://awb.fzhhl.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://yzn.snrcjt.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://dpg.tianlin.xyz

[I07] 忽略大小写与多行模式
来源：http://dfc.jinyuanbaomall.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://vwy.zhoulong.xyz

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://szd.hywenlv.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://zpx.epnwcf.com

TS:   /error/gim
来源：http://njf.52xcode.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://uyk.hongshengwenyu.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://grl.shanyushiyangkeji.top

Ruby: s.scan(/error/i)
来源：http://kto.9152youxi.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://mhn.sysykeji.top

[I08] 贪婪与非贪婪匹配
来源：http://xzv.yj20258888.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://wnm.meibo888.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://gbz.hongshengwenyu.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://spm.xingfuxueyuan.xyz

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://slm.yfazqb.com

Java: Pattern.compile("<b>.*?</b>")
来源：http://aij.jyoumei.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ggy.0kj1m.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ujq.jqgufenzy.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://fog.ehwqpu.com

================================================================================
来源：http://aan.daria6918.cn

J. 日期与时间
来源：http://bap.zhoulong.xyz

================================================================================
来源：http://kic.jinyuanbaomall.cn

[J01] 获取当前时间
来源：http://tjj.hfpthk.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://vtm.0kj1m.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ivr.tianlin.xyz

JS:   new Date();  Date.now()
来源：http://qwg.wangshuangyany.cn

TS:   new Date();  Date.now()
来源：http://pzy.aibaodan.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://nwn.pycfn.com

Go:   time.Now()
来源：http://mbt.vqdsnc.cn

Ruby: Time.now
来源：http://izz.jiagoushi.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://vtj.xuanzx.com

[J02] 格式化输出
来源：http://bql.dashuyun.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://nty.guannengcc.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://qkv.bjfxy.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hsn.fktsv.cn

TS:   d.toISOString()
来源：http://kgh.iojbl.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://pxa.yj20258888.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://kaj.dianchejie.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://xpv.hnqzz.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://xuq.hnxiangtu.top

[J03] 字符串解析为日期
来源：http://bjw.andypj.xyz

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://fvg.andypj.xyz

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://iys.jinqigfzy.top

JS:   new Date("2024-01-02")
来源：http://xgf.kuanghao11.cn

TS:   new Date("2024-01-02")
来源：http://ivs.sjlbkw.cn

Java: LocalDate.parse("2024-01-02")
来源：http://qat.zhiwuduotai.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://gwf.0kj1m.cn

Ruby: Date.parse("2024-01-02")
来源：http://tum.sweek.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://daq.xingfuxueyuan.xyz

[J04] 时间戳与日期互转
来源：http://dmx.tian-w.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://cnz.wangshuangyany.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://kwx.yfazqb.com

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://vdl.zhixingplan.top

TS:   Math.floor(Date.now() / 1000)
来源：http://lhe.nanxuanxn.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://cua.tarul.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://pcl.vehdjk.com

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ceh.xziqi.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://noh.svipenyu.cn

[J05] 时间加减（加 7 天）
来源：http://pvh.hcnkem.com

Py:   now + timedelta(days=7)
来源：http://jiq.9152youxi.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://atj.yuanzhike.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://mzx.fktsv.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hkf.xinyue.icu

Java: LocalDate.now().plusDays(7)
来源：http://gch.fzhhl.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://rki.zdqjudy.top

Ruby: Time.now + 7 * 86400
来源：http://lbc.ehwqpu.com

C#:   DateTime.Now.AddDays(7)
来源：http://duf.xinyue.icu

[J06] 计算两时间之差
来源：http://rpu.andypj.xyz

Py:   (end - start).total_seconds()
来源：http://erc.jqgfzy.top

PHP:  $end->diff($start)->days;
来源：http://thq.zhijiandao.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://yzg.jyoumei.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://kgz.aibaodan.cn

Java: Duration.between(start, end).toSeconds()
来源：http://ozq.shanyushiyangtech.top

Go:   end.Sub(start).Hours()
来源：http://oav.ybcxt.top

Ruby: end - start                 # 返回秒数
来源：http://mpf.yueranfly.top

C#:   (end - start).TotalSeconds
来源：http://yew.xylfe.cn

[J07] 比较两个日期
来源：http://xfi.aizwys.cn

Py:   d1 < d2;  d1 == d2
来源：http://ust.gaohongyu789.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ccl.zhiwuduotai.top

JS:   d1.getTime() < d2.getTime()
来源：http://hqy.gzhubu.top

TS:   d1.getTime() < d2.getTime()
来源：http://pvc.hammf.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://vgy.jianghu66.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://jfo.yuxming.cn

Ruby: d1 < d2;  d1 == d2
来源：http://xxr.chenzaomai.com

C#:   d1 < d2;  d1 == d2
来源：http://ysp.hywenlv.cn

[J08] 提取年月日与星期
来源：http://ifl.fehbvm.com

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://nap.gzhubu.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://cwn.cdnleiting.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ixr.shanyushiyangkeji.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://mxn.jlsjyb.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://lpb.hammf.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ujn.kuanghao11.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://mim.nwbrower.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://tis.9152youxi.cn

[J09] 时区处理
来源：http://bjv.ehwqpu.com

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://two.52xcode.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hqs.jinqigufen.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://kfc.snrcjt.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://pjl.sufxvd.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ugp.yueranfly.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://pzx.wangdashe.top

Ruby: Time.now.getlocal("+08:00")
来源：http://aqe.hnxiangtu.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://vmv.vehdjk.com

[J10] 取今天 / 本月第一天
来源：http://tgm.sxryk.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://hqw.zhiwuduotai.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://bno.ybcxt.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://nom.yanxiufei.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://eyg.zhaomingkeji.xyz

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://qhq.tianlin.xyz

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://eog.fengsongda.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://pzy.dianchejie.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://asg.hcnkem.com

================================================================================
来源：http://hbm.xylfe.cn

K. JSON 与序列化
来源：http://ibk.yuanzhike.top

================================================================================
来源：http://wqx.yueranfly.top

[K01] 对象转 JSON 字符串
来源：http://enw.xuetiantiany.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ahn.pycfn.com

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ujn.chenzaomai.com

JS:   JSON.stringify(obj)
来源：http://gvn.xuanzx.com

TS:   JSON.stringify(obj)
来源：http://kbj.cdnleiting.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://iht.mhx1999.top

Go:   json.Marshal(obj)
来源：http://bwp.yuxming.cn

Ruby: obj.to_json                                     // require "json"
来源：http://cmb.kuanghao11.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://zok.hnqzz.top

[K02] JSON 字符串转对象
来源：http://tqg.feifeiyinyue.top

Py:   json.loads(s)
来源：http://jwv.pycfn.com

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://uar.hesvh.cn

JS:   JSON.parse(s)
来源：http://ndq.fktsv.cn

TS:   JSON.parse(s)
来源：http://nyy.aizwys.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://bbt.feifeiyinyue.top

Go:   json.Unmarshal(data, &v)
来源：http://yml.yuxming.cn

Ruby: JSON.parse(s)
来源：http://hjj.tanke756.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://yvj.shanyushiyangtech.top

[K03] JSON 美化输出（带缩进）
来源：http://efp.hcnkem.com

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ahb.quarkkingdee.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wjb.gotoacloud.top

JS:   JSON.stringify(obj, null, 2)
来源：http://ruq.yuanzhike.top

TS:   JSON.stringify(obj, null, 2)
来源：http://wnw.yj20258.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://dfr.redwolf501.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://twe.quarkkingdee.top

Ruby: JSON.pretty_generate(obj)
来源：http://zdj.fzhhl.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://jni.xuetiantiany.cn

[K04] 读取 JSON 文件
来源：http://vnv.haohaochexian.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://wvw.ydjk.org.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://cgl.tian-w.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://jjb.fehbvm.com

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://vmt.hnqzz.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://cfq.wangshuangyany.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://qow.jqgufenzy.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://weu.0kj1m.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ifi.shzxlz.cn

[K05] 深拷贝对象
来源：http://ftr.birdmap.top

Py:   copy.deepcopy(obj)
来源：http://dht.yangfankeji.com

PHP:  unserialize(serialize($obj));
来源：http://tzy.pycfn.com

JS:   structuredClone(obj)
来源：http://tvj.dianchejie.cn

TS:   structuredClone(obj)
来源：http://dvy.xinyue.icu

Java: // 手写拷贝构造，或序列化往返
来源：http://fam.bjfxy.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://fvp.birdmap.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://rcv.shuidangran.top

C#:   // 序列化往返，或自定义 Clone
来源：http://tby.bjfxy.top

[K06] 解析 URL 查询串
来源：http://nst.ctjpmb.com

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://rmj.cdnleiting.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://npl.shzxlz.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://htl.xziqi.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://exd.svipenyu.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://msc.zhoulong.xyz

Go:   url.ParseQuery("a=1&b=2")
来源：http://nex.yuanzhike.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wex.guannengcc.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://pub.zhiwuduotai.top

[K07] 进制转换
来源：http://dav.yj20258.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hih.xziqi.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ufh.cdnleiting.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://isc.zhaomingkeji.xyz

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://oev.yfazqb.com

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://aoz.zdbjq.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://vrx.dashuyun.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://kxi.zycfv.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ahg.daxiang520.top

[K08] 二进制序列化（非 JSON）
来源：http://kfs.wangdashe.top

Py:   pickle.dumps(obj)
来源：http://wja.shuidangran.top

PHP:  serialize($obj);  unserialize($s);
来源：http://uaz.cdnleiting.top

JS:   v8.serialize(obj)        // Node
来源：http://qme.fktsv.cn

TS:   v8.serialize(obj)        // Node
来源：http://vxi.mhx1999.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://vhn.yj20258.top

Go:   encoding/gob
来源：http://iml.jinghuilouyu.cn

Ruby: Marshal.dump(obj)
来源：http://txj.zhengqikj.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://lnd.316326.xyz

================================================================================
来源：http://zfw.iojbl.cn

L. 网络请求
来源：http://rve.hcnkem.com

================================================================================
来源：http://pps.hywenlv.cn

[L01] 发送 GET 请求
来源：http://uky.guowangkeji.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mgx.sysykeji.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://thx.mhx1999.top

JS:   await fetch(url)
来源：http://ddc.haohaochexian.top

TS:   await fetch(url)
来源：http://pod.yj202588.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://cio.fengsongda.top

Go:   resp, err := http.Get(url)
来源：http://fes.sysykeji.top

Ruby: Net::HTTP.get(URI(url))
来源：http://qpf.wangshuangyany.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://obv.bbcook.cn

[L02] 发送 POST JSON
来源：http://nks.xingfuxueyuan.xyz

Py:   requests.post(url, json={"a": 1})
来源：http://rje.hongshengwenyu.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://shp.zhoulong.xyz

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://vsh.havefunace.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hrc.shanyushiyangkeji.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wzm.jianghu66.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://joh.9152youxi.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://dnn.guowangkeji.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://nnu.guowangkeji.top

[L03] 设置自定义请求头
来源：http://aiu.sufxvd.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://noy.sjlbkw.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://zpt.xylfe.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://snu.wangshuangyany.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://crw.uphjek.com

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://yba.yonumen.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://iaw.xuetiantiany.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://zja.ybcxt.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://gxr.jqgfzy.top

[L04] 设置超时
来源：http://gdg.ivvv.top

Py:   requests.get(url, timeout=5)
来源：http://wix.yuanzhike.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://adm.yonumen.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ltu.hongshengwenyu.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://yzv.zhijiandao.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://squ.sysykeji.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://dbd.jinghuilouyu.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://vpx.feifeiyinyue.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://xsp.haohaochexian.top

[L05] 上传文件（multipart）
来源：http://aoh.sweek.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ezk.cdnleiting.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://aao.yj202588.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://xwy.zhaomingkeji.xyz

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://lrj.hywenlv.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ccz.sysykeji.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://chv.cdnleiting.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ang.zhaomingkeji.xyz

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ubl.jinqigufen.top

[L06] 解析响应为 JSON
来源：http://ljj.yueranfly.top

Py:   resp.json()
来源：http://tze.epnwcf.com

PHP:  json_decode($body, true);
来源：http://cqt.tanke756.top

JS:   await resp.json()
来源：http://owc.feifeiyinyue.top

TS:   await resp.json()
来源：http://axi.hysaishi.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://brz.sweek.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://nfc.nanxinkj.top

Ruby: JSON.parse(resp.body)
来源：http://ltm.jinyuanbaomall.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://nmi.xuetiantiany.cn

[L07] 处理 HTTP 状态码
来源：http://xzt.pengpengdd.cyou

Py:   resp.status_code;  resp.raise_for_status()
来源：http://dmv.chenjidiqi.icu

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://qve.ehwqpu.com

JS:   resp.ok;  resp.status
来源：http://vhn.xingfuxueyuan.xyz

TS:   resp.ok;  resp.status
来源：http://qxb.shanyushiyangkeji.top

Java: resp.statusCode()
来源：http://xkx.zycfv.cn

Go:   resp.StatusCode
来源：http://nyt.bjfxy.top

Ruby: resp.code.to_i
来源：http://gsu.fanxiaobao.xyz

C#:   (int)resp.StatusCode
来源：http://vyc.daxiang520.top

[L08] 并发请求多个地址
来源：http://ygs.yangfankeji.com

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hhy.haohaochexian.top

PHP:  curl_multi_init() 系列
来源：http://rmp.guowangkeji.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://kld.hysaishi.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://vzx.shanyushiyangtech.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://lyi.jiagoushi.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hio.zdqjudy.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://vls.xingfuxueyuan.xyz

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://grf.c1oappe.top

================================================================================
来源：http://sdn.gotoacloud.top

M. 命令行 / 进程 / 环境
来源：http://ohy.zhongyouzk.top

================================================================================
来源：http://piu.zhoulong.xyz

[M01] 读取命令行参数
来源：http://wnv.yuanzhike.top

Py:   sys.argv[1:]
来源：http://yxo.zhixingplan.top

PHP:  $argv;  $argc;
来源：http://vhv.zdqjudy.top

JS:   process.argv.slice(2)
来源：http://edp.redwolf501.top

TS:   process.argv.slice(2)
来源：http://ajc.zdbjq.cn

Java: args 数组（main 方法参数）
来源：http://zos.sxryk.cn

Go:   os.Args[1:]
来源：http://hfn.haohaochexian.top

Ruby: ARGV
来源：http://lxu.yongpay.top

C#:   args 数组（Main 方法参数）
来源：http://tgn.shangyingyoupin.top

[M02] 读取环境变量
来源：http://bvr.zhoulong.xyz

Py:   os.environ.get("HOME")
来源：http://wct.chenzaomai.com

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://eqn.jianghu66.top

JS:   process.env.HOME
来源：http://cyx.mhx1999.top

TS:   process.env.HOME
来源：http://hzv.jyoumei.cn

Java: System.getenv("HOME")
来源：http://vag.fanxiaobao.xyz

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://kxu.vqdsnc.cn

Ruby: ENV["HOME"]
来源：http://qrr.0kj1m.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://bff.daxiang520.top

[M03] 执行外部命令
来源：http://lxu.jinyuanbaomall.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://vkq.hfpthk.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://woy.svipenyu.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://lbp.yvedp.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://slf.316326.xyz


<!-- 参考信息 -->