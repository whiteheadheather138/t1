代发 wailian999

Java: s.split("\\s*,\\s*")
来源：http://ull.sufxvd.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://odx.c1oappe.top

Ruby: s.split(/\s*,\s*/)
来源：http://mgi.316326.xyz

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://tpe.zhijiandao.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://whq.svipenyu.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://vke.shangyingyoupin.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://isy.yfazqb.com

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ftc.smart0.xyz

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://vkf.xziqi.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ecv.jlsjyb.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hsf.gaohongyu789.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://het.zhixingplan.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://rzy.xingfuxueyuan.xyz

[I07] 忽略大小写与多行模式
来源：http://arx.shangyingyoupin.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://xlk.daria6918.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://eav.shangyingyoupin.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://cdc.uphjek.com

TS:   /error/gim
来源：http://rmv.aizwys.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ejl.ywan-chungtsiang.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://boj.redwolf501.top

Ruby: s.scan(/error/i)
来源：http://rgi.smart0.xyz

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://gvx.bbcook.cn

[I08] 贪婪与非贪婪匹配
来源：http://yoc.zhixingplan.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://wab.birdmap.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ibk.tianlin.xyz

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://vpl.bjfxy.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://kol.quarkkingdee.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://nci.jianghu66.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://awo.zdbjq.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://czm.yj202588.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://xrp.kuanghao11.cn

================================================================================
来源：http://qin.9152youxi.cn

J. 日期与时间
来源：http://sal.cashguo.top

================================================================================
来源：http://nmo.epnwcf.com

[J01] 获取当前时间
来源：http://qrq.yonumen.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://jyq.hywenlv.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://joq.zdqjudy.top

JS:   new Date();  Date.now()
来源：http://cqa.jiagoushi.top

TS:   new Date();  Date.now()
来源：http://nmh.fktsv.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://dhv.dianchejie.cn

Go:   time.Now()
来源：http://pnp.guowangkeji.top

Ruby: Time.now
来源：http://tue.daria6918.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://lyd.redwolf501.top

[J02] 格式化输出
来源：http://esc.ydzc1.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://gbh.cheryme.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://brg.xuetiantiany.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://vli.fzhhl.top

TS:   d.toISOString()
来源：http://lii.hongshengwenyu.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://zst.kuanghao11.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://kbv.nanxuanxn.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://avz.zhixingplan.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://csc.jinqigfzy.top

[J03] 字符串解析为日期
来源：http://bwq.aibaodan.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://riv.zdbjq.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://jpw.ehwqpu.com

JS:   new Date("2024-01-02")
来源：http://jgp.zhengqikj.top

TS:   new Date("2024-01-02")
来源：http://uor.zhixingplan.top

Java: LocalDate.parse("2024-01-02")
来源：http://fog.zhongyouzk.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://uvt.zhoulong.xyz

Ruby: Date.parse("2024-01-02")
来源：http://frn.guannengcc.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://rhx.yanxiufei.cn

[J04] 时间戳与日期互转
来源：http://nfr.xuetiantiany.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://yec.jinghuilouyu.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://kob.fengsongda.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://pgd.cashguo.top

TS:   Math.floor(Date.now() / 1000)
来源：http://xdv.aizwys.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://mmo.cucudq.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://llf.iojbl.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://wcc.shanyushiyangtech.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hpo.tian-w.cn

[J05] 时间加减（加 7 天）
来源：http://swy.fengsongda.top

Py:   now + timedelta(days=7)
来源：http://qaj.guowangkeji.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://wvh.gotoacloud.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ips.chenjidiqi.icu

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://owh.fengsongda.top

Java: LocalDate.now().plusDays(7)
来源：http://gni.hfpthk.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://qcq.tarul.cn

Ruby: Time.now + 7 * 86400
来源：http://gmz.sweek.top

C#:   DateTime.Now.AddDays(7)
来源：http://utt.jyoumei.cn

[J06] 计算两时间之差
来源：http://esr.xuetiantiany.cn

Py:   (end - start).total_seconds()
来源：http://mkt.sufxvd.cn

PHP:  $end->diff($start)->days;
来源：http://mtm.yongpay.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://rwk.jinqigufen.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://zie.mhx1999.top

Java: Duration.between(start, end).toSeconds()
来源：http://lex.xingfuxueyuan.xyz

Go:   end.Sub(start).Hours()
来源：http://edb.svipenyu.cn

Ruby: end - start                 # 返回秒数
来源：http://zlr.wangshuangyany.cn

C#:   (end - start).TotalSeconds
来源：http://dta.snrcjt.cn

[J07] 比较两个日期
来源：http://ttj.yanxiufei.cn

Py:   d1 < d2;  d1 == d2
来源：http://rot.bbcook.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ijv.meibo888.top

JS:   d1.getTime() < d2.getTime()
来源：http://hyt.gzhubu.top

TS:   d1.getTime() < d2.getTime()
来源：http://yyz.andypj.xyz

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://wqj.iojbl.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://yql.meibo888.top

Ruby: d1 < d2;  d1 == d2
来源：http://efb.daxiang520.top

C#:   d1 < d2;  d1 == d2
来源：http://isl.snrcjt.cn

[J08] 提取年月日与星期
来源：http://mmx.xinyue.icu

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ohu.zhongyouzk.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://rei.fktsv.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://cvb.iojbl.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://kch.zhiwuduotai.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://npt.hnqzz.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://bmi.quarkkingdee.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ohq.cqqwz.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://clm.yvedp.cn

[J09] 时区处理
来源：http://gfm.aizwys.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hdb.dashuyun.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://bhv.cheryme.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ufj.yuanzhike.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://amo.zycfv.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://sht.yanxiufei.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://vrb.ivvv.top

Ruby: Time.now.getlocal("+08:00")
来源：http://fuk.9152youxi.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://iaj.shangyingyoupin.top

[J10] 取今天 / 本月第一天
来源：http://svv.gogol.net.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://nye.guannengcc.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://zss.jiagoushi.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://gfl.xinyue.icu

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://dcr.vqdsnc.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://uve.svipenyu.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://pat.zhaomingkeji.xyz

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://gpw.nwbrower.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://nny.tanke756.top

================================================================================
来源：http://ebz.zhixingplan.top

K. JSON 与序列化
来源：http://dcp.ydzc1.top

================================================================================
来源：http://bvb.jinyuanbaomall.cn

[K01] 对象转 JSON 字符串
来源：http://cge.tian-w.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://iad.zhengqikj.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://vgt.sweek.top

JS:   JSON.stringify(obj)
来源：http://wwk.nwbrower.top

TS:   JSON.stringify(obj)
来源：http://acq.wangshuangyany.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://mqa.yj20258888.top

Go:   json.Marshal(obj)
来源：http://mxv.hesvh.cn

Ruby: obj.to_json                                     // require "json"
来源：http://ssm.ydjk.org.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://ilp.zdqjudy.top

[K02] JSON 字符串转对象
来源：http://kyw.aizwys.cn

Py:   json.loads(s)
来源：http://cpo.yangfankeji.com

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://uqu.ywan-chungtsiang.top

JS:   JSON.parse(s)
来源：http://smr.daria6918.cn

TS:   JSON.parse(s)
来源：http://dzn.fengsongda.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://kut.sxryk.cn

Go:   json.Unmarshal(data, &v)
来源：http://tzc.yanxiufei.cn

Ruby: JSON.parse(s)
来源：http://apu.gotoacloud.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://arm.ybcxt.top

[K03] JSON 美化输出（带缩进）
来源：http://rki.tian-w.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://kek.ybcxt.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://usc.shuidangran.top

JS:   JSON.stringify(obj, null, 2)
来源：http://fbj.316326.xyz

TS:   JSON.stringify(obj, null, 2)
来源：http://lrb.hesvh.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://fak.zycfv.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://yqf.yj20258.top

Ruby: JSON.pretty_generate(obj)
来源：http://oxg.cucudq.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://cua.jinghuilouyu.cn

[K04] 读取 JSON 文件
来源：http://xhf.fktsv.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://bzt.yj20258888.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hof.jlsjyb.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wph.zhaomingkeji.xyz

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wbs.316326.xyz

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ikd.fehbvm.com

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://msw.haohaochexian.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://svb.jlsjyb.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://geh.aizwys.cn

[K05] 深拷贝对象
来源：http://wqv.mhx1999.top

Py:   copy.deepcopy(obj)
来源：http://jxj.cdnleiting.top

PHP:  unserialize(serialize($obj));
来源：http://hjw.hysaishi.cn

JS:   structuredClone(obj)
来源：http://eql.daxiang520.top

TS:   structuredClone(obj)
来源：http://sfk.mhx1999.top

Java: // 手写拷贝构造，或序列化往返
来源：http://bwr.nanxuanxn.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hhl.jyoumei.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://lmu.tianlin.xyz

C#:   // 序列化往返，或自定义 Clone
来源：http://djz.meibo888.top

[K06] 解析 URL 查询串
来源：http://eqa.316326.xyz

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://atj.zhongyouzk.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mzt.snrcjt.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hmp.tanke756.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://kor.birdmap.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://cdm.jinqigufen.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://dzm.mhx1999.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://cfs.shuidangran.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://mnf.kuanghao11.cn

[K07] 进制转换
来源：http://wgn.cucudq.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://uwz.yuxming.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://gfs.fehbvm.com

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://pvx.cdnleiting.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wqk.daria6918.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://bwu.cqqwz.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://xgk.daria6918.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://qbx.wangdashe.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://frs.ehwqpu.com

[K08] 二进制序列化（非 JSON）
来源：http://gdh.yonumen.top

Py:   pickle.dumps(obj)
来源：http://whr.shuidangran.top

PHP:  serialize($obj);  unserialize($s);
来源：http://fgd.quarkkingdee.top

JS:   v8.serialize(obj)        // Node
来源：http://iai.ctjpmb.com

TS:   v8.serialize(obj)        // Node
来源：http://jrk.vehdjk.com

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://grg.jinghuilouyu.cn

Go:   encoding/gob
来源：http://ury.snrcjt.cn

Ruby: Marshal.dump(obj)
来源：http://jfi.aizwys.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://fpf.aibaodan.cn

================================================================================
来源：http://yic.andypj.xyz

L. 网络请求
来源：http://eqs.hysaishi.cn

================================================================================
来源：http://qmt.jqgfzy.top

[L01] 发送 GET 请求
来源：http://grb.daxiang520.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://cis.xingfuxueyuan.xyz

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wmt.sysykeji.top

JS:   await fetch(url)
来源：http://oxk.bbcook.cn

TS:   await fetch(url)
来源：http://nlm.quarkkingdee.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://wts.c1oappe.top

Go:   resp, err := http.Get(url)
来源：http://qmt.yuxming.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://hky.cashguo.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://fld.c1oappe.top

[L02] 发送 POST JSON
来源：http://qxe.jinqigufen.top

Py:   requests.post(url, json={"a": 1})
来源：http://mrq.iojbl.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://tmt.gaohongyu789.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://lvm.uphjek.com

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://drh.vehdjk.com

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ekm.316326.xyz

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://nnw.jinyuanbaomall.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://yxj.cheryme.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://kci.hcnkem.com

[L03] 设置自定义请求头
来源：http://alp.yueranfly.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ddw.9152youxi.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://cmn.cashguo.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://xyy.pycfn.com

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ltr.tian-w.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://yrd.gogol.net.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hrb.nanxinkj.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://xgn.meibo888.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://atn.yangfankeji.com

[L04] 设置超时
来源：http://pdi.jianghu66.top

Py:   requests.get(url, timeout=5)
来源：http://sco.ybcxt.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://zcw.hnxiangtu.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://vvw.shzxlz.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://xqx.zycfv.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://xpl.tian-w.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://yrx.fanxiaobao.xyz

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://acz.yvedp.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://kxa.iojbl.cn

[L05] 上传文件（multipart）
来源：http://xam.zhongyouzk.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://art.xinyue.icu

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://tub.yj20258888.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://llm.nwbrower.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mwf.dashuyun.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hqz.smart0.xyz

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://nbk.fktsv.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://dhi.aizwys.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mmk.shanyushiyangtech.top

[L06] 解析响应为 JSON
来源：http://epn.quarkkingdee.top

Py:   resp.json()
来源：http://rnj.yuxming.cn

PHP:  json_decode($body, true);
来源：http://qks.jinyuanbaomall.cn

JS:   await resp.json()
来源：http://kjd.jyoumei.cn

TS:   await resp.json()
来源：http://chv.aibaodan.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wzv.guannengcc.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://xfi.hongshengwenyu.top

Ruby: JSON.parse(resp.body)
来源：http://cqy.jinghuilouyu.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://msh.c1oappe.top

[L07] 处理 HTTP 状态码
来源：http://yex.c1oappe.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://saw.smart0.xyz

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://vqg.haohaochexian.top

JS:   resp.ok;  resp.status
来源：http://pgb.cqqwz.cn

TS:   resp.ok;  resp.status
来源：http://qcd.hcnkem.com

Java: resp.statusCode()
来源：http://dqa.zhengqikj.top

Go:   resp.StatusCode
来源：http://osk.jqgufenzy.top

Ruby: resp.code.to_i
来源：http://omh.dianchejie.cn

C#:   (int)resp.StatusCode
来源：http://qry.vehdjk.com

[L08] 并发请求多个地址
来源：http://pgm.jinqigufen.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://fvu.cdnleiting.top

PHP:  curl_multi_init() 系列
来源：http://hjj.redwolf501.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://cxs.ppjwa.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://nym.svipenyu.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://xty.kuanghao11.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ult.zhoulong.xyz

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://gph.jinqigufen.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://gxp.pycfn.com

================================================================================
来源：http://mqg.shangyingyoupin.top

M. 命令行 / 进程 / 环境
来源：http://uop.quarkkingdee.top

================================================================================
来源：http://wts.daxiang520.top

[M01] 读取命令行参数
来源：http://ide.tanke756.top

Py:   sys.argv[1:]
来源：http://fsa.jinqigfzy.top

PHP:  $argv;  $argc;
来源：http://zkc.andypj.xyz

JS:   process.argv.slice(2)
来源：http://zmj.cheryme.top

TS:   process.argv.slice(2)
来源：http://pgy.fzhhl.top

Java: args 数组（main 方法参数）
来源：http://agd.uphjek.com

Go:   os.Args[1:]
来源：http://rht.jinyuanbaomall.cn

Ruby: ARGV
来源：http://pgk.dashuyun.cn

C#:   args 数组（Main 方法参数）
来源：http://caj.xingfuxueyuan.xyz

[M02] 读取环境变量
来源：http://bqd.9152youxi.cn

Py:   os.environ.get("HOME")
来源：http://apn.zhoulong.xyz

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://nfm.0kj1m.cn

JS:   process.env.HOME
来源：http://jus.bbcook.cn

TS:   process.env.HOME
来源：http://jkf.epnwcf.com

Java: System.getenv("HOME")
来源：http://ayb.fehbvm.com

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://aph.52xcode.cn

Ruby: ENV["HOME"]
来源：http://jvl.sjlbkw.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://nha.tanke756.top

[M03] 执行外部命令
来源：http://any.haohaochexian.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wua.zhijiandao.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://axe.xinyue.icu

JS:   child_process.execSync("ls -l").toString()
来源：http://sja.smart0.xyz

TS:   child_process.execSync("ls -l").toString()
来源：http://yuw.chenjidiqi.icu


<!-- 参考信息 -->