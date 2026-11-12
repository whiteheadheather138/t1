代发 wailian999

Java: s.split("\\s*,\\s*")
来源：http://pia.gzhubu.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://cpx.jlsjyb.cn

Ruby: s.split(/\s*,\s*/)
来源：http://yde.vqdsnc.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://uho.yfazqb.com

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://yia.quarkkingdee.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://clb.52xcode.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://cbn.9152youxi.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://dqj.hesvh.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://dmo.nwbrower.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://eqv.zhongyouzk.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://eih.yangfankeji.com

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://dhs.gotoacloud.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://zko.jqgufenzy.top

[I07] 忽略大小写与多行模式
来源：http://fxh.yonumen.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://itf.havefunace.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://lib.andypj.xyz

JS:   /error/gim；new RegExp("error", "gim")
来源：http://qkr.yj20258.top

TS:   /error/gim
来源：http://yzw.xuetiantiany.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://uut.sufxvd.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ncc.jqgufenzy.top

Ruby: s.scan(/error/i)
来源：http://eqn.hongshengwenyu.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://qml.sjlbkw.cn

[I08] 贪婪与非贪婪匹配
来源：http://xeg.zdqjudy.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://zlc.guannengcc.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://poa.bjfxy.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://zdz.andypj.xyz

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://zwo.xylfe.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://gbs.zhiwuduotai.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hui.hammf.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://vdj.mhx1999.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://erj.hnqzz.top

================================================================================
来源：http://uek.zhixingplan.top

J. 日期与时间
来源：http://ovx.smart0.xyz

================================================================================
来源：http://scx.yanxiufei.cn

[J01] 获取当前时间
来源：http://mfr.yueranfly.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://tdo.ydzc1.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://kqc.bbcook.cn

JS:   new Date();  Date.now()
来源：http://hua.52xcode.cn

TS:   new Date();  Date.now()
来源：http://hjv.hammf.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://xtr.zhengqikj.top

Go:   time.Now()
来源：http://gbi.feifeiyinyue.top

Ruby: Time.now
来源：http://xno.yj20258888.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://rka.pengpengdd.cyou

[J02] 格式化输出
来源：http://xhq.yj202588.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://iev.jinghuilouyu.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://abm.cheryme.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://prb.daria6918.cn

TS:   d.toISOString()
来源：http://goh.yj202588.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://pmd.shanyushiyangtech.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://nta.yueranfly.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wde.zhiwuduotai.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ulj.uphjek.com

[J03] 字符串解析为日期
来源：http://bzr.nanxinkj.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://lyz.quarkkingdee.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://wyy.nwbrower.top

JS:   new Date("2024-01-02")
来源：http://yli.zycfv.cn

TS:   new Date("2024-01-02")
来源：http://kfw.hammf.cn

Java: LocalDate.parse("2024-01-02")
来源：http://abb.xingfuxueyuan.xyz

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://apu.tianlin.xyz

Ruby: Date.parse("2024-01-02")
来源：http://uam.sweek.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://jet.xuetiantiany.cn

[J04] 时间戳与日期互转
来源：http://yak.uphjek.com

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ihh.52xcode.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hbz.snrcjt.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://oom.shanyushiyangtech.top

TS:   Math.floor(Date.now() / 1000)
来源：http://trw.zhixingplan.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hum.fehbvm.com

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://gwf.cdnleiting.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://pri.nanxuanxn.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ytn.guowangkeji.top

[J05] 时间加减（加 7 天）
来源：http://qqy.dashuyun.cn

Py:   now + timedelta(days=7)
来源：http://nfg.hfpthk.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://atx.gotoacloud.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://vyk.jinyuanbaomall.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://jyr.birdmap.top

Java: LocalDate.now().plusDays(7)
来源：http://bnu.yj202588.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ytg.yangfankeji.com

Ruby: Time.now + 7 * 86400
来源：http://oog.tarul.cn

C#:   DateTime.Now.AddDays(7)
来源：http://ass.shuidangran.top

[J06] 计算两时间之差
来源：http://exj.ywan-chungtsiang.top

Py:   (end - start).total_seconds()
来源：http://fqu.sweek.top

PHP:  $end->diff($start)->days;
来源：http://gfw.shzxlz.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://inq.chenjidiqi.icu

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://knc.quarkkingdee.top

Java: Duration.between(start, end).toSeconds()
来源：http://gcq.jinqigufen.top

Go:   end.Sub(start).Hours()
来源：http://qbm.cqqwz.cn

Ruby: end - start                 # 返回秒数
来源：http://joh.feifeiyinyue.top

C#:   (end - start).TotalSeconds
来源：http://qgc.sufxvd.cn

[J07] 比较两个日期
来源：http://uhb.sjlbkw.cn

Py:   d1 < d2;  d1 == d2
来源：http://fza.zdbjq.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://vnd.hongshengwenyu.top

JS:   d1.getTime() < d2.getTime()
来源：http://bip.jqgufenzy.top

TS:   d1.getTime() < d2.getTime()
来源：http://mlq.nanxinkj.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://clt.jiagoushi.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://uas.yonumen.top

Ruby: d1 < d2;  d1 == d2
来源：http://oql.sjlbkw.cn

C#:   d1 < d2;  d1 == d2
来源：http://pwm.jqgufenzy.top

[J08] 提取年月日与星期
来源：http://zcj.wangshuangyany.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://vpr.fktsv.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://qlq.chenjidiqi.icu

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://plb.snrcjt.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://quj.ivvv.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://kzx.zhoulong.xyz

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://fyn.jinqigufen.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://pdp.wangdashe.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ngs.9152youxi.cn

[J09] 时区处理
来源：http://yie.vqdsnc.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://irc.yongpay.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hfj.tarul.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://olr.yangfankeji.com

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mtl.aibaodan.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://eld.jinghuilouyu.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://inm.yvedp.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://hwi.nwbrower.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://dri.cheryme.top

[J10] 取今天 / 本月第一天
来源：http://zre.hysaishi.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://pqm.yuxming.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://dpm.andypj.xyz

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://laz.hesvh.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://rkb.9152youxi.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ncw.svipenyu.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://suo.aibaodan.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://uvs.zhiwuduotai.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ktv.jiagoushi.top

================================================================================
来源：http://uwt.gzhubu.top

K. JSON 与序列化
来源：http://xps.bbcook.cn

================================================================================
来源：http://snk.ydjk.org.cn

[K01] 对象转 JSON 字符串
来源：http://whw.birdmap.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://xxt.jqgufenzy.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://byr.yfazqb.com

JS:   JSON.stringify(obj)
来源：http://hll.zhengqikj.top

TS:   JSON.stringify(obj)
来源：http://gwp.gotoacloud.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://bpd.yj20258888.top

Go:   json.Marshal(obj)
来源：http://kcn.vehdjk.com

Ruby: obj.to_json                                     // require "json"
来源：http://czc.gzhubu.top

C#:   JsonSerializer.Serialize(obj)
来源：http://crq.gzhubu.top

[K02] JSON 字符串转对象
来源：http://wpf.yangfankeji.com

Py:   json.loads(s)
来源：http://dhc.shanyushiyangkeji.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://alc.jyoumei.cn

JS:   JSON.parse(s)
来源：http://siv.tanke756.top

TS:   JSON.parse(s)
来源：http://bqd.yvedp.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ytw.9152youxi.cn

Go:   json.Unmarshal(data, &v)
来源：http://wfa.yanxiufei.cn

Ruby: JSON.parse(s)
来源：http://jsd.yj202588.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://via.316326.xyz

[K03] JSON 美化输出（带缩进）
来源：http://sma.guannengcc.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://fqj.zhongyouzk.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://orh.zhixingplan.top

JS:   JSON.stringify(obj, null, 2)
来源：http://lhs.jinqigufen.top

TS:   JSON.stringify(obj, null, 2)
来源：http://lbu.nanxinkj.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://lmx.hammf.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://eqx.jqgufenzy.top

Ruby: JSON.pretty_generate(obj)
来源：http://mka.ydzc1.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://zvo.hammf.cn

[K04] 读取 JSON 文件
来源：http://lbd.nwbrower.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://vbw.fengsongda.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://kdf.jqgfzy.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://xmq.fzhhl.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://gfu.jqgufenzy.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://dxz.snrcjt.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://mpj.sufxvd.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://hds.hesvh.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://brx.redwolf501.top

[K05] 深拷贝对象
来源：http://ges.9152youxi.cn

Py:   copy.deepcopy(obj)
来源：http://tuc.zdbjq.cn

PHP:  unserialize(serialize($obj));
来源：http://yjf.jlsjyb.cn

JS:   structuredClone(obj)
来源：http://pld.nwbrower.top

TS:   structuredClone(obj)
来源：http://itr.shangyingyoupin.top

Java: // 手写拷贝构造，或序列化往返
来源：http://jzz.cheryme.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ats.jqgfzy.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://nrc.jianghu66.top

C#:   // 序列化往返，或自定义 Clone
来源：http://zzi.hywenlv.cn

[K06] 解析 URL 查询串
来源：http://rdo.smart0.xyz

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://udz.tarul.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://xtf.jqgufenzy.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ted.ydzc1.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://jlt.birdmap.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://uyw.jlsjyb.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://eed.yfazqb.com

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://fja.xinyue.icu

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://nll.yj20258.top

[K07] 进制转换
来源：http://ych.redwolf501.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ytg.guowangkeji.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://oru.tanke756.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://bch.ctjpmb.com

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://vbk.zhixingplan.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://cpo.gaohongyu789.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://byr.zhiwuduotai.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://jww.zhiwuduotai.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://bxs.cucudq.cn

[K08] 二进制序列化（非 JSON）
来源：http://cdg.xziqi.cn

Py:   pickle.dumps(obj)
来源：http://iru.hnqzz.top

PHP:  serialize($obj);  unserialize($s);
来源：http://yyd.ydjk.org.cn

JS:   v8.serialize(obj)        // Node
来源：http://qch.zhoulong.xyz

TS:   v8.serialize(obj)        // Node
来源：http://bkf.ctjpmb.com

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://urh.fktsv.cn

Go:   encoding/gob
来源：http://zff.mhx1999.top

Ruby: Marshal.dump(obj)
来源：http://zrx.feifeiyinyue.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://gxm.xylfe.cn

================================================================================
来源：http://lic.cdnleiting.top

L. 网络请求
来源：http://wnm.yuanzhike.top

================================================================================
来源：http://ygt.ydjk.org.cn

[L01] 发送 GET 请求
来源：http://gyf.andypj.xyz

Py:   requests.get(url)                        # 第三方库 requests
来源：http://llx.bbcook.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://yib.cqqwz.cn

JS:   await fetch(url)
来源：http://uxc.shzxlz.cn

TS:   await fetch(url)
来源：http://aon.hnqzz.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hrw.ppjwa.cn

Go:   resp, err := http.Get(url)
来源：http://uyl.sysykeji.top

Ruby: Net::HTTP.get(URI(url))
来源：http://kdl.ppjwa.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://qfi.hywenlv.cn

[L02] 发送 POST JSON
来源：http://auv.nanxinkj.top

Py:   requests.post(url, json={"a": 1})
来源：http://yex.cqqwz.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://lmp.jianghu66.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://vop.chenlongwang.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://vib.zhaomingkeji.xyz

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://nmc.0kj1m.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://xuj.wangshuangyany.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://zex.yongpay.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://yoj.hesvh.cn

[L03] 设置自定义请求头
来源：http://crf.jianghu66.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://laa.zhaomingkeji.xyz

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://btt.hcnkem.com

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://cxm.xingfuxueyuan.xyz

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://eux.snrcjt.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://pxd.yongpay.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://pxz.ivvv.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://pqr.shzxlz.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://xuc.pengpengdd.cyou

[L04] 设置超时
来源：http://fpi.c1oappe.top

Py:   requests.get(url, timeout=5)
来源：http://tvq.xuetiantiany.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://jwj.yangfankeji.com

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ozs.hesvh.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://gyi.mhx1999.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://vhc.dianchejie.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://adc.hammf.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wpb.yangfankeji.com

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://smp.jyoumei.cn

[L05] 上传文件（multipart）
来源：http://sij.zhiwuduotai.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://bgp.jlsjyb.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://lbb.yangfankeji.com

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://bxt.hfpthk.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://xmi.svipenyu.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://atu.52xcode.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ikj.0kj1m.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://whb.zhoulong.xyz

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://qpb.zhaomingkeji.xyz

[L06] 解析响应为 JSON
来源：http://qwo.vehdjk.com

Py:   resp.json()
来源：http://pqv.snrcjt.cn

PHP:  json_decode($body, true);
来源：http://ook.pengpengdd.cyou

JS:   await resp.json()
来源：http://fbg.ctjpmb.com

TS:   await resp.json()
来源：http://zpl.zycfv.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://rqh.shanyushiyangtech.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://tid.zhoulong.xyz

Ruby: JSON.parse(resp.body)
来源：http://oma.xziqi.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ypb.jiagoushi.top

[L07] 处理 HTTP 状态码
来源：http://jjz.hfpthk.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://drn.sjlbkw.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://qws.bbcook.cn

JS:   resp.ok;  resp.status
来源：http://rsq.zhoulong.xyz

TS:   resp.ok;  resp.status
来源：http://dzv.0kj1m.cn

Java: resp.statusCode()
来源：http://yur.guannengcc.top

Go:   resp.StatusCode
来源：http://qet.yanxiufei.cn

Ruby: resp.code.to_i
来源：http://xtp.yvedp.cn

C#:   (int)resp.StatusCode
来源：http://tzl.xziqi.cn

[L08] 并发请求多个地址
来源：http://ygk.vqdsnc.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://uiv.tarul.cn

PHP:  curl_multi_init() 系列
来源：http://hhl.shangyingyoupin.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://qpt.nanxuanxn.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://snt.tian-w.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mks.shzxlz.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://zsl.sweek.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://eha.52xcode.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://kwa.hywenlv.cn

================================================================================
来源：http://rmt.zdqjudy.top

M. 命令行 / 进程 / 环境
来源：http://qjp.nanxuanxn.top

================================================================================
来源：http://pjj.nwbrower.top

[M01] 读取命令行参数
来源：http://zva.bjfxy.top

Py:   sys.argv[1:]
来源：http://kzf.ybcxt.top

PHP:  $argv;  $argc;
来源：http://jcx.quarkkingdee.top

JS:   process.argv.slice(2)
来源：http://yuc.birdmap.top

TS:   process.argv.slice(2)
来源：http://lyl.xylfe.cn

Java: args 数组（main 方法参数）
来源：http://uds.jqgfzy.top

Go:   os.Args[1:]
来源：http://ini.epnwcf.com

Ruby: ARGV
来源：http://mfj.uphjek.com

C#:   args 数组（Main 方法参数）
来源：http://ezq.shanyushiyangkeji.top

[M02] 读取环境变量
来源：http://xlm.daria6918.cn

Py:   os.environ.get("HOME")
来源：http://why.ybcxt.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://rfm.wangshuangyany.cn

JS:   process.env.HOME
来源：http://kkw.zhaomingkeji.xyz

TS:   process.env.HOME
来源：http://rhn.cheryme.top

Java: System.getenv("HOME")
来源：http://gkv.jinghuilouyu.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://xep.kuanghao11.cn

Ruby: ENV["HOME"]
来源：http://vru.fzhhl.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://pnj.smart0.xyz

[M03] 执行外部命令
来源：http://tef.52xcode.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://yeo.jianghu66.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://nkq.ydjk.org.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://ggy.hnqzz.top

TS:   child_process.execSync("ls -l").toString()
来源：http://lgk.xuanzx.com


<!-- 参考信息 -->