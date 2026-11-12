代发 wailian999

Java: s.split("\\s*,\\s*")
来源：http://ozn.hysaishi.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://axi.zhaomingkeji.xyz

Ruby: s.split(/\s*,\s*/)
来源：http://njq.fengsongda.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://jqi.svipenyu.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://voz.bjfxy.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://nom.yj202588.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://wft.52xcode.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wpw.ppjwa.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://xxe.zycfv.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://xok.aibaodan.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://typ.dashuyun.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://iqa.9152youxi.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://umy.andypj.xyz

[I07] 忽略大小写与多行模式
来源：http://fvj.feifeiyinyue.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://xbu.ywan-chungtsiang.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://xmr.ybcxt.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://vln.fengsongda.top

TS:   /error/gim
来源：http://emp.316326.xyz

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://tgp.hammf.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://nfq.yanxiufei.cn

Ruby: s.scan(/error/i)
来源：http://ngu.dianchejie.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hrd.316326.xyz

[I08] 贪婪与非贪婪匹配
来源：http://awv.yj20258888.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://uhc.zhoulong.xyz

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://bno.jlsjyb.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://lgt.fengsongda.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://aiu.cqqwz.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://nsu.yuxming.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://zub.jqgfzy.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://rml.haohaochexian.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hwf.zhongyouzk.top

================================================================================
来源：http://yvk.hywenlv.cn

J. 日期与时间
来源：http://nnb.sweek.top

================================================================================
来源：http://gsm.jiagoushi.top

[J01] 获取当前时间
来源：http://kuo.gaohongyu789.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://zpi.fzhhl.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://awh.tanke756.top

JS:   new Date();  Date.now()
来源：http://quj.jiagoushi.top

TS:   new Date();  Date.now()
来源：http://rgv.jinghuilouyu.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://zjr.9152youxi.cn

Go:   time.Now()
来源：http://suz.ybcxt.top

Ruby: Time.now
来源：http://oxg.guowangkeji.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ghq.iojbl.cn

[J02] 格式化输出
来源：http://kwz.yj20258888.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://tgd.yuanzhike.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://gua.andypj.xyz

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://slt.9152youxi.cn

TS:   d.toISOString()
来源：http://ias.zhixingplan.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ecf.aizwys.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://oua.jiagoushi.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://nsn.dashuyun.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://uks.vqdsnc.cn

[J03] 字符串解析为日期
来源：http://fwl.zhaomingkeji.xyz

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://xmr.jiagoushi.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://uxw.vehdjk.com

JS:   new Date("2024-01-02")
来源：http://zkq.tian-w.cn

TS:   new Date("2024-01-02")
来源：http://wwy.ivvv.top

Java: LocalDate.parse("2024-01-02")
来源：http://nro.cdnleiting.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://wie.zdbjq.cn

Ruby: Date.parse("2024-01-02")
来源：http://vnf.guowangkeji.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ctp.dianchejie.cn

[J04] 时间戳与日期互转
来源：http://tpl.ywan-chungtsiang.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://tag.redwolf501.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ceo.kuanghao11.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://bsb.zhixingplan.top

TS:   Math.floor(Date.now() / 1000)
来源：http://ujx.yj202588.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hxo.andypj.xyz

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ent.chenzaomai.com

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ttk.cheryme.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://cmr.jlsjyb.cn

[J05] 时间加减（加 7 天）
来源：http://ejy.nwbrower.top

Py:   now + timedelta(days=7)
来源：http://zdf.aibaodan.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://jba.ydzc1.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://upe.cucudq.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://qvv.xziqi.cn

Java: LocalDate.now().plusDays(7)
来源：http://oxx.wangshuangyany.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ruu.shzxlz.cn

Ruby: Time.now + 7 * 86400
来源：http://xrp.jinqigufen.top

C#:   DateTime.Now.AddDays(7)
来源：http://fje.aibaodan.cn

[J06] 计算两时间之差
来源：http://rbc.52xcode.cn

Py:   (end - start).total_seconds()
来源：http://pfk.ydzc1.top

PHP:  $end->diff($start)->days;
来源：http://dlh.jianghu66.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://jwb.zhiwuduotai.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://smy.pycfn.com

Java: Duration.between(start, end).toSeconds()
来源：http://oog.aibaodan.cn

Go:   end.Sub(start).Hours()
来源：http://lxa.quarkkingdee.top

Ruby: end - start                 # 返回秒数
来源：http://img.uphjek.com

C#:   (end - start).TotalSeconds
来源：http://nnd.sjlbkw.cn

[J07] 比较两个日期
来源：http://qgr.xingfuxueyuan.xyz

Py:   d1 < d2;  d1 == d2
来源：http://tkh.svipenyu.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://gpr.daria6918.cn

JS:   d1.getTime() < d2.getTime()
来源：http://tym.nwbrower.top

TS:   d1.getTime() < d2.getTime()
来源：http://bip.gzhubu.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://voi.ydzc1.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://qat.ehwqpu.com

Ruby: d1 < d2;  d1 == d2
来源：http://dhe.smart0.xyz

C#:   d1 < d2;  d1 == d2
来源：http://nxe.fzhhl.top

[J08] 提取年月日与星期
来源：http://rai.sweek.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://fdm.vqdsnc.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://mrm.aizwys.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://bpg.fktsv.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://wnc.yfazqb.com

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hvp.redwolf501.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://nxl.zhijiandao.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://kxo.sjlbkw.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://zfz.hesvh.cn

[J09] 时区处理
来源：http://gev.quarkkingdee.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://xbl.zhaomingkeji.xyz

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://gpg.hnxiangtu.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://fwb.andypj.xyz

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://xsi.dianchejie.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://xrp.vehdjk.com

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://tkd.nanxinkj.top

Ruby: Time.now.getlocal("+08:00")
来源：http://srh.jinghuilouyu.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://iys.smart0.xyz

[J10] 取今天 / 本月第一天
来源：http://prf.nwbrower.top

Py:   date.today();  date.today().replace(day=1)
来源：http://yjp.snrcjt.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://wiq.redwolf501.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ond.dianchejie.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hzq.havefunace.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://zha.xinyue.icu

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://vax.yonumen.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hxf.wangdashe.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ipx.bbcook.cn

================================================================================
来源：http://mjn.ywan-chungtsiang.top

K. JSON 与序列化
来源：http://xnu.tianlin.xyz

================================================================================
来源：http://pqm.sweek.top

[K01] 对象转 JSON 字符串
来源：http://umc.haohaochexian.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://esj.xingfuxueyuan.xyz

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://gkk.chenjidiqi.icu

JS:   JSON.stringify(obj)
来源：http://afa.bbcook.cn

TS:   JSON.stringify(obj)
来源：http://psc.aibaodan.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://fsc.tanke756.top

Go:   json.Marshal(obj)
来源：http://juj.aizwys.cn

Ruby: obj.to_json                                     // require "json"
来源：http://wxg.xuetiantiany.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://hgq.nanxinkj.top

[K02] JSON 字符串转对象
来源：http://wlc.52xcode.cn

Py:   json.loads(s)
来源：http://wpi.yonumen.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ggm.yangfankeji.com

JS:   JSON.parse(s)
来源：http://ssm.zhaomingkeji.xyz

TS:   JSON.parse(s)
来源：http://ckc.hysaishi.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://xap.cqqwz.cn

Go:   json.Unmarshal(data, &v)
来源：http://xks.chenzaomai.com

Ruby: JSON.parse(s)
来源：http://yll.hywenlv.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://afc.hammf.cn

[K03] JSON 美化输出（带缩进）
来源：http://pig.feifeiyinyue.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://pnv.chenzaomai.com

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://xtv.xinyue.icu

JS:   JSON.stringify(obj, null, 2)
来源：http://wyw.bbcook.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://jhx.shuidangran.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ghz.zdbjq.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ust.xziqi.cn

Ruby: JSON.pretty_generate(obj)
来源：http://vlp.vehdjk.com

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://yfl.fanxiaobao.xyz

[K04] 读取 JSON 文件
来源：http://dcu.quarkkingdee.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ngg.feifeiyinyue.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://xko.zdqjudy.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://bka.guannengcc.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ync.xinyue.icu

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://uxz.gogol.net.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://lmx.sjlbkw.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://ovk.nanxinkj.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://bna.tian-w.cn

[K05] 深拷贝对象
来源：http://cre.cashguo.top

Py:   copy.deepcopy(obj)
来源：http://kqg.yonumen.top

PHP:  unserialize(serialize($obj));
来源：http://xrx.jianghu66.top

JS:   structuredClone(obj)
来源：http://tij.haohaochexian.top

TS:   structuredClone(obj)
来源：http://rpg.gzhubu.top

Java: // 手写拷贝构造，或序列化往返
来源：http://lwf.guannengcc.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://gvd.havefunace.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://sun.ydzc1.top

C#:   // 序列化往返，或自定义 Clone
来源：http://sdj.ywan-chungtsiang.top

[K06] 解析 URL 查询串
来源：http://clx.tian-w.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://jox.xinyue.icu

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mxa.hcnkem.com

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://rpl.yonumen.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://cks.fehbvm.com

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://rpn.nanxinkj.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://tyk.tarul.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://vlv.jianghu66.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://vih.hfpthk.cn

[K07] 进制转换
来源：http://jvy.jqgufenzy.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ben.0kj1m.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://msx.hesvh.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ztc.sweek.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://fky.zhijiandao.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://qqm.zhixingplan.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ieh.yueranfly.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://xxq.aizwys.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://jld.hywenlv.cn

[K08] 二进制序列化（非 JSON）
来源：http://iyb.pycfn.com

Py:   pickle.dumps(obj)
来源：http://tix.yj20258.top

PHP:  serialize($obj);  unserialize($s);
来源：http://bzv.pengpengdd.cyou

JS:   v8.serialize(obj)        // Node
来源：http://lmf.cqqwz.cn

TS:   v8.serialize(obj)        // Node
来源：http://jij.hcnkem.com

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ins.zdqjudy.top

Go:   encoding/gob
来源：http://xci.havefunace.top

Ruby: Marshal.dump(obj)
来源：http://bff.yj202588.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://qcx.kuanghao11.cn

================================================================================
来源：http://tmr.dianchejie.cn

L. 网络请求
来源：http://asv.c1oappe.top

================================================================================
来源：http://goi.zdbjq.cn

[L01] 发送 GET 请求
来源：http://azl.cheryme.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://fwz.cdnleiting.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ftl.meibo888.top

JS:   await fetch(url)
来源：http://xpt.xinyue.icu

TS:   await fetch(url)
来源：http://vgb.xinyue.icu

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://atq.bjfxy.top

Go:   resp, err := http.Get(url)
来源：http://jvy.hnxiangtu.top

Ruby: Net::HTTP.get(URI(url))
来源：http://awl.zhengqikj.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://mbx.bjfxy.top

[L02] 发送 POST JSON
来源：http://xzl.pengpengdd.cyou

Py:   requests.post(url, json={"a": 1})
来源：http://uks.yueranfly.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://xru.pycfn.com

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://uap.sxryk.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://nnq.iojbl.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://xkm.vqdsnc.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ubg.sweek.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://zol.jyoumei.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://tsj.hysaishi.cn

[L03] 设置自定义请求头
来源：http://wic.ivvv.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://glk.daria6918.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://cxm.snrcjt.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://rze.uphjek.com

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://pyo.shangyingyoupin.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://agf.jiagoushi.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://swm.hnxiangtu.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://sdf.guannengcc.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://syb.cashguo.top

[L04] 设置超时
来源：http://wqs.jiagoushi.top

Py:   requests.get(url, timeout=5)
来源：http://hpv.shangyingyoupin.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://kpa.zhengqikj.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://aaz.shzxlz.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://vwk.wangshuangyany.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://qgl.gzhubu.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://jxk.gzhubu.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wua.svipenyu.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://umv.yuxming.cn

[L05] 上传文件（multipart）
来源：http://ajn.yj20258.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mic.bbcook.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://urk.aibaodan.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://fgg.c1oappe.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://quo.xingfuxueyuan.xyz

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://tgb.ywan-chungtsiang.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ill.chenzaomai.com

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://jnu.shanyushiyangkeji.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://spn.sweek.top

[L06] 解析响应为 JSON
来源：http://brn.gotoacloud.top

Py:   resp.json()
来源：http://wjr.xuetiantiany.cn

PHP:  json_decode($body, true);
来源：http://xzd.gzhubu.top

JS:   await resp.json()
来源：http://ghh.zycfv.cn

TS:   await resp.json()
来源：http://xbi.havefunace.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://vsz.yj202588.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mti.bjfxy.top

Ruby: JSON.parse(resp.body)
来源：http://jeu.yanxiufei.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://qvu.52xcode.cn

[L07] 处理 HTTP 状态码
来源：http://rru.uphjek.com

Py:   resp.status_code;  resp.raise_for_status()
来源：http://vlt.gotoacloud.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://xfy.bbcook.cn

JS:   resp.ok;  resp.status
来源：http://lpz.jianghu66.top

TS:   resp.ok;  resp.status
来源：http://jfw.shanyushiyangkeji.top

Java: resp.statusCode()
来源：http://rcz.quarkkingdee.top

Go:   resp.StatusCode
来源：http://kut.sysykeji.top

Ruby: resp.code.to_i
来源：http://nqw.dashuyun.cn

C#:   (int)resp.StatusCode
来源：http://csl.nwbrower.top

[L08] 并发请求多个地址
来源：http://wkt.jlsjyb.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://eec.jianghu66.top

PHP:  curl_multi_init() 系列
来源：http://qxo.hnxiangtu.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://vyf.aibaodan.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://axp.cqqwz.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://lgo.gaohongyu789.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mpg.birdmap.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://pgf.zdqjudy.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://gyy.yangfankeji.com

================================================================================
来源：http://hqt.shanyushiyangkeji.top

M. 命令行 / 进程 / 环境
来源：http://oyw.shanyushiyangtech.top

================================================================================
来源：http://lgw.jlsjyb.cn

[M01] 读取命令行参数
来源：http://wgg.sysykeji.top

Py:   sys.argv[1:]
来源：http://xfc.wangdashe.top

PHP:  $argv;  $argc;
来源：http://giz.guannengcc.top

JS:   process.argv.slice(2)
来源：http://hsu.jinghuilouyu.cn

TS:   process.argv.slice(2)
来源：http://gjy.cheryme.top

Java: args 数组（main 方法参数）
来源：http://quh.yvedp.cn

Go:   os.Args[1:]
来源：http://kft.zdbjq.cn

Ruby: ARGV
来源：http://anq.yuanzhike.top

C#:   args 数组（Main 方法参数）
来源：http://uqg.jiagoushi.top

[M02] 读取环境变量
来源：http://cma.jinyuanbaomall.cn

Py:   os.environ.get("HOME")
来源：http://gyo.epnwcf.com

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://jnm.jinyuanbaomall.cn

JS:   process.env.HOME
来源：http://ckh.shanyushiyangtech.top

TS:   process.env.HOME
来源：http://aty.snrcjt.cn

Java: System.getenv("HOME")
来源：http://nda.tanke756.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://jmh.yj20258.top

Ruby: ENV["HOME"]
来源：http://jaw.chenlongwang.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://scl.nanxuanxn.top

[M03] 执行外部命令
来源：http://djh.shzxlz.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://nxe.ivvv.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mtw.jinqigfzy.top

JS:   child_process.execSync("ls -l").toString()
来源：http://ksk.daxiang520.top

TS:   child_process.execSync("ls -l").toString()
来源：http://ejv.havefunace.top


<!-- 参考信息 -->