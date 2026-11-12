代发 wailian999

Java: s.split("\\s*,\\s*")
来源：http://cmi.fktsv.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://mlt.yfazqb.com

Ruby: s.split(/\s*,\s*/)
来源：http://fuc.9152youxi.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://gek.yj20258.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://tza.svipenyu.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ulz.zhijiandao.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://prd.nwbrower.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://vvp.jinyuanbaomall.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://giz.fanxiaobao.xyz

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://lpi.zdbjq.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hnt.nwbrower.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://pgz.cheryme.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://xsr.hesvh.cn

[I07] 忽略大小写与多行模式
来源：http://ayr.zdbjq.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://pzk.ctjpmb.com

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://snh.zhaomingkeji.xyz

JS:   /error/gim；new RegExp("error", "gim")
来源：http://wqh.ybcxt.top

TS:   /error/gim
来源：http://xkl.nanxuanxn.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://zwy.fengsongda.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://anw.jqgufenzy.top

Ruby: s.scan(/error/i)
来源：http://kek.zdqjudy.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://uva.zhiwuduotai.top

[I08] 贪婪与非贪婪匹配
来源：http://qyo.xinyue.icu

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://seb.cqqwz.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ner.hongshengwenyu.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ley.wangdashe.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://iad.iojbl.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://zjq.epnwcf.com

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://xto.bbcook.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://lvf.52xcode.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://xhm.pengpengdd.cyou

================================================================================
来源：http://xzl.xinyue.icu

J. 日期与时间
来源：http://vno.zdbjq.cn

================================================================================
来源：http://enm.shanyushiyangtech.top

[J01] 获取当前时间
来源：http://hrx.wangdashe.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://yhb.yvedp.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://zhr.zhaomingkeji.xyz

JS:   new Date();  Date.now()
来源：http://abe.tian-w.cn

TS:   new Date();  Date.now()
来源：http://iwi.52xcode.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://zlq.redwolf501.top

Go:   time.Now()
来源：http://tar.nanxinkj.top

Ruby: Time.now
来源：http://ofq.shuidangran.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hle.chenlongwang.top

[J02] 格式化输出
来源：http://fef.fanxiaobao.xyz

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://xpm.uphjek.com

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://vls.andypj.xyz

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://zvm.chenzaomai.com

TS:   d.toISOString()
来源：http://maz.gogol.net.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hos.jqgufenzy.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://qam.jlsjyb.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://kki.bjfxy.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://pnj.yonumen.top

[J03] 字符串解析为日期
来源：http://npo.sufxvd.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://kqx.birdmap.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://vnu.jinqigufen.top

JS:   new Date("2024-01-02")
来源：http://olu.jinghuilouyu.cn

TS:   new Date("2024-01-02")
来源：http://xqi.fanxiaobao.xyz

Java: LocalDate.parse("2024-01-02")
来源：http://alj.cdnleiting.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://tzs.jyoumei.cn

Ruby: Date.parse("2024-01-02")
来源：http://lnb.snrcjt.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ast.fktsv.cn

[J04] 时间戳与日期互转
来源：http://mpo.kuanghao11.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://bqs.hfpthk.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ehk.yfazqb.com

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://bzr.sxryk.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://ybt.zhengqikj.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://oal.jinghuilouyu.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://whk.hongshengwenyu.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://quz.yj20258.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://loc.nwbrower.top

[J05] 时间加减（加 7 天）
来源：http://yny.daxiang520.top

Py:   now + timedelta(days=7)
来源：http://sgh.ydjk.org.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://rtu.hnxiangtu.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://qbu.shzxlz.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://kom.ctjpmb.com

Java: LocalDate.now().plusDays(7)
来源：http://are.gzhubu.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://onb.dianchejie.cn

Ruby: Time.now + 7 * 86400
来源：http://sug.tanke756.top

C#:   DateTime.Now.AddDays(7)
来源：http://kev.ctjpmb.com

[J06] 计算两时间之差
来源：http://udv.yongpay.top

Py:   (end - start).total_seconds()
来源：http://xmn.yj20258.top

PHP:  $end->diff($start)->days;
来源：http://slc.zdqjudy.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://wzv.shangyingyoupin.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://mer.sysykeji.top

Java: Duration.between(start, end).toSeconds()
来源：http://zsa.hongshengwenyu.top

Go:   end.Sub(start).Hours()
来源：http://dwb.zhijiandao.cn

Ruby: end - start                 # 返回秒数
来源：http://ipw.gzhubu.top

C#:   (end - start).TotalSeconds
来源：http://bgq.haohaochexian.top

[J07] 比较两个日期
来源：http://tuq.52xcode.cn

Py:   d1 < d2;  d1 == d2
来源：http://bcb.redwolf501.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://evx.bbcook.cn

JS:   d1.getTime() < d2.getTime()
来源：http://ctm.yj20258888.top

TS:   d1.getTime() < d2.getTime()
来源：http://snq.hnqzz.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ggk.yj20258.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://rfx.tianlin.xyz

Ruby: d1 < d2;  d1 == d2
来源：http://hzi.iojbl.cn

C#:   d1 < d2;  d1 == d2
来源：http://qhq.zycfv.cn

[J08] 提取年月日与星期
来源：http://tfv.jinqigfzy.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://fyo.sysykeji.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://mkm.gzhubu.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ppr.jqgufenzy.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://avx.jinghuilouyu.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://zsb.zhixingplan.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hle.yj20258888.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hzq.cdnleiting.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://bpo.cqqwz.cn

[J09] 时区处理
来源：http://akr.jlsjyb.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://rze.jinghuilouyu.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://qoj.nanxuanxn.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://rkk.hysaishi.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://iqy.c1oappe.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://wbb.shzxlz.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://waw.zdbjq.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://pez.xingfuxueyuan.xyz

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://kme.zhengqikj.top

[J10] 取今天 / 本月第一天
来源：http://vbr.zhaomingkeji.xyz

Py:   date.today();  date.today().replace(day=1)
来源：http://nmv.tanke756.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://xtt.shanyushiyangtech.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hhc.xuanzx.com

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://eja.jianghu66.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://kel.svipenyu.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://fha.xylfe.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://vmi.dianchejie.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://svw.hnxiangtu.top

================================================================================
来源：http://wul.uphjek.com

K. JSON 与序列化
来源：http://ksi.zdbjq.cn

================================================================================
来源：http://cnr.gotoacloud.top

[K01] 对象转 JSON 字符串
来源：http://vrl.jinyuanbaomall.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://dqb.bjfxy.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://zke.jinqigfzy.top

JS:   JSON.stringify(obj)
来源：http://sux.zdbjq.cn

TS:   JSON.stringify(obj)
来源：http://kti.smart0.xyz

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ttp.pengpengdd.cyou

Go:   json.Marshal(obj)
来源：http://tgy.tanke756.top

Ruby: obj.to_json                                     // require "json"
来源：http://vgm.aizwys.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://tqs.birdmap.top

[K02] JSON 字符串转对象
来源：http://enf.yvedp.cn

Py:   json.loads(s)
来源：http://emh.hongshengwenyu.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://jax.zdbjq.cn

JS:   JSON.parse(s)
来源：http://elv.cheryme.top

TS:   JSON.parse(s)
来源：http://zjl.shanyushiyangkeji.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://kmw.fktsv.cn

Go:   json.Unmarshal(data, &v)
来源：http://qfl.jinyuanbaomall.cn

Ruby: JSON.parse(s)
来源：http://xzj.yonumen.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://qob.jyoumei.cn

[K03] JSON 美化输出（带缩进）
来源：http://ofs.jyoumei.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ytt.zhoulong.xyz

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hap.hesvh.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://kvs.daria6918.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://rhy.fehbvm.com

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://fid.jlsjyb.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://avu.sufxvd.cn

Ruby: JSON.pretty_generate(obj)
来源：http://pah.yanxiufei.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://lpr.havefunace.top

[K04] 读取 JSON 文件
来源：http://sxr.jinqigufen.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://fqm.yangfankeji.com

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://htu.zdbjq.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://xte.meibo888.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ofo.cashguo.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://doq.dashuyun.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://otv.yfazqb.com

Ruby: JSON.parse(File.read("a.json"))
来源：http://mih.shzxlz.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ijx.feifeiyinyue.top

[K05] 深拷贝对象
来源：http://zoe.svipenyu.cn

Py:   copy.deepcopy(obj)
来源：http://kdm.yuxming.cn

PHP:  unserialize(serialize($obj));
来源：http://anb.hnqzz.top

JS:   structuredClone(obj)
来源：http://aio.bjfxy.top

TS:   structuredClone(obj)
来源：http://uyy.gaohongyu789.top

Java: // 手写拷贝构造，或序列化往返
来源：http://fco.yanxiufei.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://fww.gaohongyu789.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://iys.hywenlv.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://sdn.zdqjudy.top

[K06] 解析 URL 查询串
来源：http://bnn.52xcode.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://uhc.ybcxt.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ixj.yanxiufei.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://dja.andypj.xyz

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://bhp.guannengcc.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://bvd.vqdsnc.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://nqa.jinyuanbaomall.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://zmt.ydjk.org.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://iot.zhaomingkeji.xyz

[K07] 进制转换
来源：http://swl.aibaodan.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ppi.cheryme.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hmb.nwbrower.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://eng.guowangkeji.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://kvo.cashguo.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ktu.zhixingplan.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://opo.jinqigufen.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ggc.hongshengwenyu.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://bgl.chenjidiqi.icu

[K08] 二进制序列化（非 JSON）
来源：http://aat.yj202588.top

Py:   pickle.dumps(obj)
来源：http://evk.xylfe.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://cks.fehbvm.com

JS:   v8.serialize(obj)        // Node
来源：http://gja.sjlbkw.cn

TS:   v8.serialize(obj)        // Node
来源：http://uua.quarkkingdee.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wqy.hongshengwenyu.top

Go:   encoding/gob
来源：http://dny.birdmap.top

Ruby: Marshal.dump(obj)
来源：http://ntm.bjfxy.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://bhs.fanxiaobao.xyz

================================================================================
来源：http://tqw.yj202588.top

L. 网络请求
来源：http://spi.uphjek.com

================================================================================
来源：http://foj.cqqwz.cn

[L01] 发送 GET 请求
来源：http://rtb.jiagoushi.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mbs.yuanzhike.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://kyj.shzxlz.cn

JS:   await fetch(url)
来源：http://hnp.aizwys.cn

TS:   await fetch(url)
来源：http://qsj.shanyushiyangkeji.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://epo.quarkkingdee.top

Go:   resp, err := http.Get(url)
来源：http://idn.guannengcc.top

Ruby: Net::HTTP.get(URI(url))
来源：http://ltv.mhx1999.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://lzb.cucudq.cn

[L02] 发送 POST JSON
来源：http://rue.gogol.net.cn

Py:   requests.post(url, json={"a": 1})
来源：http://ara.vehdjk.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://pmp.jianghu66.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://tkt.daxiang520.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://rbo.pycfn.com

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wne.zhiwuduotai.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://jzd.uphjek.com

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wpn.shuidangran.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://zso.hesvh.cn

[L03] 设置自定义请求头
来源：http://rtg.feifeiyinyue.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://jgp.ctjpmb.com

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://gnr.jiagoushi.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://jos.hysaishi.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ewh.hfpthk.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://nrp.hnqzz.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://gyx.yj20258.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://vdz.ctjpmb.com

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ewf.bbcook.cn

[L04] 设置超时
来源：http://zsu.tianlin.xyz

Py:   requests.get(url, timeout=5)
来源：http://jjj.meibo888.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://woq.fanxiaobao.xyz

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://onr.pengpengdd.cyou

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://yal.jinqigufen.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://fpx.tanke756.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ncn.fktsv.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://zaa.ctjpmb.com

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://nhh.zhijiandao.cn

[L05] 上传文件（multipart）
来源：http://idm.yonumen.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://qmz.cdnleiting.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://djo.pycfn.com

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hfk.cdnleiting.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hro.jinyuanbaomall.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://xpw.cucudq.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ylf.ctjpmb.com

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://rtd.aizwys.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://zcp.nanxinkj.top

[L06] 解析响应为 JSON
来源：http://rff.bbcook.cn

Py:   resp.json()
来源：http://guw.jinqigfzy.top

PHP:  json_decode($body, true);
来源：http://zli.hfpthk.cn

JS:   await resp.json()
来源：http://shg.zhixingplan.top

TS:   await resp.json()
来源：http://xwo.chenjidiqi.icu

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://fcn.xylfe.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://qsc.sysykeji.top

Ruby: JSON.parse(resp.body)
来源：http://dox.snrcjt.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://fyw.yueranfly.top

[L07] 处理 HTTP 状态码
来源：http://eia.epnwcf.com

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mpd.bbcook.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://nai.yfazqb.com

JS:   resp.ok;  resp.status
来源：http://eby.ppjwa.cn

TS:   resp.ok;  resp.status
来源：http://kth.zhiwuduotai.top

Java: resp.statusCode()
来源：http://ezq.chenjidiqi.icu

Go:   resp.StatusCode
来源：http://odg.sjlbkw.cn

Ruby: resp.code.to_i
来源：http://paj.pycfn.com

C#:   (int)resp.StatusCode
来源：http://ihh.bbcook.cn

[L08] 并发请求多个地址
来源：http://hhs.shanyushiyangtech.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://imq.nwbrower.top

PHP:  curl_multi_init() 系列
来源：http://lcq.hammf.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ymw.daria6918.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://dgh.nanxinkj.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://scb.fengsongda.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://eae.jianghu66.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wia.feifeiyinyue.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://exi.bjfxy.top

================================================================================
来源：http://fns.ehwqpu.com

M. 命令行 / 进程 / 环境
来源：http://kyl.jqgufenzy.top

================================================================================
来源：http://rhe.jlsjyb.cn

[M01] 读取命令行参数
来源：http://hor.jqgfzy.top

Py:   sys.argv[1:]
来源：http://soi.hfpthk.cn

PHP:  $argv;  $argc;
来源：http://qkp.pycfn.com

JS:   process.argv.slice(2)
来源：http://ekb.zycfv.cn

TS:   process.argv.slice(2)
来源：http://fsm.mhx1999.top

Java: args 数组（main 方法参数）
来源：http://atu.ivvv.top

Go:   os.Args[1:]
来源：http://ych.haohaochexian.top

Ruby: ARGV
来源：http://quk.tian-w.cn

C#:   args 数组（Main 方法参数）
来源：http://ept.andypj.xyz

[M02] 读取环境变量
来源：http://ven.tianlin.xyz

Py:   os.environ.get("HOME")
来源：http://mfz.316326.xyz

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://rdc.wangdashe.top

JS:   process.env.HOME
来源：http://afa.sxryk.cn

TS:   process.env.HOME
来源：http://tan.epnwcf.com

Java: System.getenv("HOME")
来源：http://plt.shanyushiyangkeji.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://jmz.haohaochexian.top

Ruby: ENV["HOME"]
来源：http://lkh.fengsongda.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mah.ywan-chungtsiang.top

[M03] 执行外部命令
来源：http://ezn.yuxming.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://geu.sweek.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ymr.yvedp.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://znw.ydjk.org.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://drj.jinqigfzy.top


<!-- 参考信息 -->