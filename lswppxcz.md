代发 wailian999

Py:   re.split(r"\s*,\s*", s)
来源：http://rnx.jinghuilouyu.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://lsw.zhixingplan.top

JS:   s.split(/\s*,\s*/)
来源：http://oau.chenlongwang.top

TS:   s.split(/\s*,\s*/)
来源：http://hfj.cucudq.cn

Java: s.split("\\s*,\\s*")
来源：http://aoz.cashguo.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://nee.yanxiufei.cn

Ruby: s.split(/\s*,\s*/)
来源：http://fda.gogol.net.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://aak.yuxming.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://bns.jyoumei.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://idu.daria6918.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ruz.daria6918.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://yyb.vehdjk.com

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://nwo.hnxiangtu.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://xwm.hfpthk.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://bfp.cdnleiting.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://crn.andypj.xyz

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://jrz.gotoacloud.top

[I07] 忽略大小写与多行模式
来源：http://sny.gotoacloud.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://oki.ivvv.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://vxm.iojbl.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ulf.pycfn.com

TS:   /error/gim
来源：http://ohv.ivvv.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://dul.yuxming.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://bba.xinyue.icu

Ruby: s.scan(/error/i)
来源：http://tlm.vqdsnc.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hlq.xuetiantiany.cn

[I08] 贪婪与非贪婪匹配
来源：http://knm.andypj.xyz

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ctu.ivvv.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hec.dashuyun.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://crw.zhaomingkeji.xyz

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://nst.tian-w.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://etl.hnqzz.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://zjx.zhaomingkeji.xyz

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://oae.fehbvm.com

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://wim.fanxiaobao.xyz

================================================================================
来源：http://dme.haohaochexian.top

J. 日期与时间
来源：http://cdp.redwolf501.top

================================================================================
来源：http://ajy.yj202588.top

[J01] 获取当前时间
来源：http://loe.yj202588.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://nma.daxiang520.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://wpm.cdnleiting.top

JS:   new Date();  Date.now()
来源：http://jil.haohaochexian.top

TS:   new Date();  Date.now()
来源：http://ump.wangdashe.top

Java: LocalDateTime.now();  Instant.now()
来源：http://jsg.cqqwz.cn

Go:   time.Now()
来源：http://sqz.yfazqb.com

Ruby: Time.now
来源：http://eng.zdqjudy.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://sww.mhx1999.top

[J02] 格式化输出
来源：http://pnl.guannengcc.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://eze.daria6918.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://kor.hysaishi.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://kel.quarkkingdee.top

TS:   d.toISOString()
来源：http://tkh.gotoacloud.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://xqr.meibo888.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://yvg.cashguo.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://dsv.tian-w.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ksv.pengpengdd.cyou

[J03] 字符串解析为日期
来源：http://exd.ybcxt.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://isj.tanke756.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hzv.cashguo.top

JS:   new Date("2024-01-02")
来源：http://aib.yuxming.cn

TS:   new Date("2024-01-02")
来源：http://ycy.jinqigufen.top

Java: LocalDate.parse("2024-01-02")
来源：http://feo.feifeiyinyue.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://llo.yongpay.top

Ruby: Date.parse("2024-01-02")
来源：http://hgb.fengsongda.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://kbe.ppjwa.cn

[J04] 时间戳与日期互转
来源：http://qux.ppjwa.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://epl.fanxiaobao.xyz

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://xhd.sjlbkw.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://fbn.hysaishi.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://tgm.guowangkeji.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://iyx.zycfv.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://fed.yj20258.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://jdr.birdmap.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://euq.jinqigfzy.top

[J05] 时间加减（加 7 天）
来源：http://sse.tianlin.xyz

Py:   now + timedelta(days=7)
来源：http://lyo.smart0.xyz

PHP:  (new DateTime())->modify("+7 days");
来源：http://zlg.jinyuanbaomall.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://jal.sysykeji.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ahg.havefunace.top

Java: LocalDate.now().plusDays(7)
来源：http://lxt.cdnleiting.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://lqn.daxiang520.top

Ruby: Time.now + 7 * 86400
来源：http://eik.shzxlz.cn

C#:   DateTime.Now.AddDays(7)
来源：http://ang.meibo888.top

[J06] 计算两时间之差
来源：http://rip.zycfv.cn

Py:   (end - start).total_seconds()
来源：http://zeh.hesvh.cn

PHP:  $end->diff($start)->days;
来源：http://vnh.hysaishi.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://lkl.xuetiantiany.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://rsa.birdmap.top

Java: Duration.between(start, end).toSeconds()
来源：http://pom.hysaishi.cn

Go:   end.Sub(start).Hours()
来源：http://wuu.yuxming.cn

Ruby: end - start                 # 返回秒数
来源：http://oxe.jiagoushi.top

C#:   (end - start).TotalSeconds
来源：http://rqc.jinqigufen.top

[J07] 比较两个日期
来源：http://jax.bbcook.cn

Py:   d1 < d2;  d1 == d2
来源：http://rdo.ydzc1.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://dcx.aibaodan.cn

JS:   d1.getTime() < d2.getTime()
来源：http://fqx.zhaomingkeji.xyz

TS:   d1.getTime() < d2.getTime()
来源：http://lje.snrcjt.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ipw.c1oappe.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ijw.hysaishi.cn

Ruby: d1 < d2;  d1 == d2
来源：http://ikq.birdmap.top

C#:   d1 < d2;  d1 == d2
来源：http://gbt.tarul.cn

[J08] 提取年月日与星期
来源：http://dnp.hnqzz.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ryo.yvedp.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://zka.fzhhl.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://yjq.fehbvm.com

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://bmr.yanxiufei.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://xfw.shuidangran.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://foa.xylfe.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://pav.mhx1999.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://xfl.cheryme.top

[J09] 时区处理
来源：http://pnj.cdnleiting.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://gqz.yuanzhike.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ggd.nanxuanxn.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://okr.yj20258888.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://gxh.birdmap.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://olg.nwbrower.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://oxg.redwolf501.top

Ruby: Time.now.getlocal("+08:00")
来源：http://yhq.kuanghao11.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://fjh.hfpthk.cn

[J10] 取今天 / 本月第一天
来源：http://ovt.yuxming.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://ort.feifeiyinyue.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ljf.jinghuilouyu.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://vrz.gotoacloud.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://flj.sxryk.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://qmm.shangyingyoupin.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://cme.dianchejie.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ntf.mhx1999.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://umj.zhengqikj.top

================================================================================
来源：http://okw.redwolf501.top

K. JSON 与序列化
来源：http://tek.ydjk.org.cn

================================================================================
来源：http://txz.cheryme.top

[K01] 对象转 JSON 字符串
来源：http://uha.birdmap.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://lyi.yuxming.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://zxd.yongpay.top

JS:   JSON.stringify(obj)
来源：http://kbn.wangshuangyany.cn

TS:   JSON.stringify(obj)
来源：http://unz.zhijiandao.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://irk.xylfe.cn

Go:   json.Marshal(obj)
来源：http://gjr.fzhhl.top

Ruby: obj.to_json                                     // require "json"
来源：http://lyo.dianchejie.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://wtt.cucudq.cn

[K02] JSON 字符串转对象
来源：http://nej.52xcode.cn

Py:   json.loads(s)
来源：http://heb.ehwqpu.com

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://plg.andypj.xyz

JS:   JSON.parse(s)
来源：http://nll.nanxuanxn.top

TS:   JSON.parse(s)
来源：http://zvi.pycfn.com

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://jlm.bbcook.cn

Go:   json.Unmarshal(data, &v)
来源：http://dsm.aizwys.cn

Ruby: JSON.parse(s)
来源：http://jrt.shanyushiyangtech.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://zoj.daxiang520.top

[K03] JSON 美化输出（带缩进）
来源：http://hit.hysaishi.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://wfv.0kj1m.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://dlp.yvedp.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://ogi.9152youxi.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://rom.pycfn.com

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://pqa.haohaochexian.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://rek.zdqjudy.top

Ruby: JSON.pretty_generate(obj)
来源：http://jse.zdbjq.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://rva.fehbvm.com

[K04] 读取 JSON 文件
来源：http://kji.vehdjk.com

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://tom.shanyushiyangkeji.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://uhb.quarkkingdee.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ujw.jyoumei.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://fmr.tian-w.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wti.hammf.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://jsk.ydzc1.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://rty.gaohongyu789.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://qpp.gogol.net.cn

[K05] 深拷贝对象
来源：http://xej.sufxvd.cn

Py:   copy.deepcopy(obj)
来源：http://cmh.fktsv.cn

PHP:  unserialize(serialize($obj));
来源：http://fyy.cdnleiting.top

JS:   structuredClone(obj)
来源：http://spc.gotoacloud.top

TS:   structuredClone(obj)
来源：http://rwv.xuanzx.com

Java: // 手写拷贝构造，或序列化往返
来源：http://kal.zhongyouzk.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://khp.sufxvd.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hml.zhixingplan.top

C#:   // 序列化往返，或自定义 Clone
来源：http://bbd.shangyingyoupin.top

[K06] 解析 URL 查询串
来源：http://ggk.sweek.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ofa.bjfxy.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ywt.zhongyouzk.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://isi.daxiang520.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://waj.jinyuanbaomall.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://tji.guowangkeji.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://ldp.ivvv.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://uns.sufxvd.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://llr.hnxiangtu.top

[K07] 进制转换
来源：http://jlz.shanyushiyangtech.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://vtr.guowangkeji.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ymj.jqgfzy.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://wrr.yj20258.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://zij.hfpthk.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wpo.hongshengwenyu.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wzj.zdbjq.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://fbn.ywan-chungtsiang.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://fcr.hammf.cn

[K08] 二进制序列化（非 JSON）
来源：http://yoh.jyoumei.cn

Py:   pickle.dumps(obj)
来源：http://ykw.zhengqikj.top

PHP:  serialize($obj);  unserialize($s);
来源：http://zbs.jiagoushi.top

JS:   v8.serialize(obj)        // Node
来源：http://ppp.zdbjq.cn

TS:   v8.serialize(obj)        // Node
来源：http://uzz.dashuyun.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ycr.xziqi.cn

Go:   encoding/gob
来源：http://vtt.aibaodan.cn

Ruby: Marshal.dump(obj)
来源：http://yko.ybcxt.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://zpv.yonumen.top

================================================================================
来源：http://jri.xuanzx.com

L. 网络请求
来源：http://zlm.hnqzz.top

================================================================================
来源：http://fha.fanxiaobao.xyz

[L01] 发送 GET 请求
来源：http://pya.andypj.xyz

Py:   requests.get(url)                        # 第三方库 requests
来源：http://rzz.yuxming.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://nys.xuetiantiany.cn

JS:   await fetch(url)
来源：http://mjw.jlsjyb.cn

TS:   await fetch(url)
来源：http://lpr.hysaishi.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://wed.jinqigufen.top

Go:   resp, err := http.Get(url)
来源：http://ydw.birdmap.top

Ruby: Net::HTTP.get(URI(url))
来源：http://zau.jinqigufen.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://bos.tanke756.top

[L02] 发送 POST JSON
来源：http://rju.hesvh.cn

Py:   requests.post(url, json={"a": 1})
来源：http://byg.hysaishi.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ege.hnxiangtu.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://rtu.birdmap.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://uoj.guowangkeji.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://fex.gogol.net.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://jmx.smart0.xyz

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://efx.yangfankeji.com

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://pny.dashuyun.cn

[L03] 设置自定义请求头
来源：http://mzq.jlsjyb.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mzk.zhixingplan.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://zpe.sjlbkw.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://qda.ctjpmb.com

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ist.ydzc1.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://vbj.shangyingyoupin.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://dse.ydjk.org.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://afu.iojbl.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mvk.pengpengdd.cyou

[L04] 设置超时
来源：http://dbn.dashuyun.cn

Py:   requests.get(url, timeout=5)
来源：http://igy.hfpthk.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://fpo.xuetiantiany.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://xab.tianlin.xyz

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://nme.xuanzx.com

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://srh.svipenyu.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ybc.ppjwa.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://uvl.dashuyun.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://pti.yangfankeji.com

[L05] 上传文件（multipart）
来源：http://nus.cashguo.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://jvp.shanyushiyangtech.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://jjd.yanxiufei.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://enb.jinqigfzy.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://del.aizwys.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hos.yj202588.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://afs.aibaodan.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ubc.yanxiufei.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://vge.zhaomingkeji.xyz

[L06] 解析响应为 JSON
来源：http://wcm.sweek.top

Py:   resp.json()
来源：http://bet.fktsv.cn

PHP:  json_decode($body, true);
来源：http://wdk.xingfuxueyuan.xyz

JS:   await resp.json()
来源：http://gok.tian-w.cn

TS:   await resp.json()
来源：http://cqj.cashguo.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://vcq.nanxuanxn.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://xvk.hywenlv.cn

Ruby: JSON.parse(resp.body)
来源：http://kan.yanxiufei.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://xtq.yuxming.cn

[L07] 处理 HTTP 状态码
来源：http://atn.ydjk.org.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://xbn.zhengqikj.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://vjd.mhx1999.top

JS:   resp.ok;  resp.status
来源：http://cfa.yanxiufei.cn

TS:   resp.ok;  resp.status
来源：http://zaq.9152youxi.cn

Java: resp.statusCode()
来源：http://hqh.xuanzx.com

Go:   resp.StatusCode
来源：http://qzg.tian-w.cn

Ruby: resp.code.to_i
来源：http://rqt.ywan-chungtsiang.top

C#:   (int)resp.StatusCode
来源：http://gkw.sufxvd.cn

[L08] 并发请求多个地址
来源：http://qds.316326.xyz

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ydx.gzhubu.top

PHP:  curl_multi_init() 系列
来源：http://khy.ctjpmb.com

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://tnl.smart0.xyz

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ine.redwolf501.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://nha.svipenyu.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://vqa.ppjwa.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://nlv.shuidangran.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://rxe.yfazqb.com

================================================================================
来源：http://gwg.ybcxt.top

M. 命令行 / 进程 / 环境
来源：http://yee.zhoulong.xyz

================================================================================
来源：http://jlg.fanxiaobao.xyz

[M01] 读取命令行参数
来源：http://rxv.fengsongda.top

Py:   sys.argv[1:]
来源：http://twh.nanxuanxn.top

PHP:  $argv;  $argc;
来源：http://aiq.snrcjt.cn

JS:   process.argv.slice(2)
来源：http://pei.chenjidiqi.icu

TS:   process.argv.slice(2)
来源：http://vmz.vehdjk.com

Java: args 数组（main 方法参数）
来源：http://soi.jianghu66.top

Go:   os.Args[1:]
来源：http://gjo.ydzc1.top

Ruby: ARGV
来源：http://upi.yongpay.top

C#:   args 数组（Main 方法参数）
来源：http://dhv.pengpengdd.cyou

[M02] 读取环境变量
来源：http://fvt.feifeiyinyue.top

Py:   os.environ.get("HOME")
来源：http://erc.cashguo.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://gfm.aizwys.cn

JS:   process.env.HOME
来源：http://qkh.haohaochexian.top

TS:   process.env.HOME
来源：http://lxu.wangshuangyany.cn

Java: System.getenv("HOME")
来源：http://gsl.yj20258888.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://xin.ywan-chungtsiang.top

Ruby: ENV["HOME"]
来源：http://osl.yj202588.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://nnm.chenjidiqi.icu

[M03] 执行外部命令
来源：http://zta.zhaomingkeji.xyz


<!-- 参考信息 -->