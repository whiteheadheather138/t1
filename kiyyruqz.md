代发 wailian999

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://cgo.cheryme.top

JS:   s.replace(/\d+/g, "#")
来源：http://jke.gzhubu.top

TS:   s.replace(/\d+/g, "#")
来源：http://lhj.nanxuanxn.top

Java: s.replaceAll("\\d+", "#")
来源：http://ybg.daxiang520.top

Go:   re.ReplaceAllString(s, "#")
来源：http://hja.shuidangran.top

Ruby: s.gsub(/\d+/, "#")
来源：http://dcp.vehdjk.com

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ssm.bbcook.cn

[I05] 按正则拆分
来源：http://grr.jyoumei.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://ocn.tarul.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://agh.kuanghao11.cn

JS:   s.split(/\s*,\s*/)
来源：http://vvd.zhijiandao.cn

TS:   s.split(/\s*,\s*/)
来源：http://dfq.ybcxt.top

Java: s.split("\\s*,\\s*")
来源：http://bat.daxiang520.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://lzb.yj20258888.top

Ruby: s.split(/\s*,\s*/)
来源：http://cjj.snrcjt.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hin.fengsongda.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ycl.nanxinkj.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://lzw.sjlbkw.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://rpz.hongshengwenyu.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://owo.yanxiufei.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://gbr.zhongyouzk.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://xla.jianghu66.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://zeg.shzxlz.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://zpi.fktsv.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://mdq.yfazqb.com

[I07] 忽略大小写与多行模式
来源：http://dvv.mhx1999.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ppt.zhixingplan.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://xiz.tarul.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://zkf.mhx1999.top

TS:   /error/gim
来源：http://gtp.jqgufenzy.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ahd.wangshuangyany.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://qax.havefunace.top

Ruby: s.scan(/error/i)
来源：http://nao.guannengcc.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hpi.sxryk.cn

[I08] 贪婪与非贪婪匹配
来源：http://mgp.316326.xyz

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://wih.birdmap.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ewg.zdqjudy.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://inj.daxiang520.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://zpn.meibo888.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://esb.ctjpmb.com

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://afq.shanyushiyangkeji.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hcy.yongpay.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ceg.vqdsnc.cn

================================================================================
来源：http://giz.wangshuangyany.cn

J. 日期与时间
来源：http://vdl.0kj1m.cn

================================================================================
来源：http://ogg.xinyue.icu

[J01] 获取当前时间
来源：http://usz.tanke756.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://yiz.cashguo.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://fzu.aizwys.cn

JS:   new Date();  Date.now()
来源：http://ohs.zycfv.cn

TS:   new Date();  Date.now()
来源：http://rcb.ivvv.top

Java: LocalDateTime.now();  Instant.now()
来源：http://bbw.guannengcc.top

Go:   time.Now()
来源：http://gxe.hnxiangtu.top

Ruby: Time.now
来源：http://kwx.hongshengwenyu.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://fhl.yuxming.cn

[J02] 格式化输出
来源：http://wvk.zdbjq.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://frr.guannengcc.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://uvp.cqqwz.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://vav.vehdjk.com

TS:   d.toISOString()
来源：http://ojm.sxryk.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://rlr.tanke756.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://lcp.zhongyouzk.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://fxi.pengpengdd.cyou

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://okd.zhongyouzk.top

[J03] 字符串解析为日期
来源：http://yoq.nanxinkj.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ysg.kuanghao11.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://lbg.cdnleiting.top

JS:   new Date("2024-01-02")
来源：http://tyk.cucudq.cn

TS:   new Date("2024-01-02")
来源：http://kxe.daria6918.cn

Java: LocalDate.parse("2024-01-02")
来源：http://cuw.ctjpmb.com

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://muh.xuetiantiany.cn

Ruby: Date.parse("2024-01-02")
来源：http://mpo.meibo888.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://bxr.tanke756.top

[J04] 时间戳与日期互转
来源：http://vvb.guowangkeji.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ams.hnqzz.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ugi.zycfv.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://lvk.sxryk.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://gfk.mhx1999.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ctn.fanxiaobao.xyz

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://fii.shuidangran.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://mmw.dashuyun.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://esd.zycfv.cn

[J05] 时间加减（加 7 天）
来源：http://urf.nanxinkj.top

Py:   now + timedelta(days=7)
来源：http://dlg.jinqigfzy.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://kxg.snrcjt.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://lbs.meibo888.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://uob.sufxvd.cn

Java: LocalDate.now().plusDays(7)
来源：http://fxo.cashguo.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://rbp.sjlbkw.cn

Ruby: Time.now + 7 * 86400
来源：http://xpl.gotoacloud.top

C#:   DateTime.Now.AddDays(7)
来源：http://esi.ehwqpu.com

[J06] 计算两时间之差
来源：http://loy.nanxinkj.top

Py:   (end - start).total_seconds()
来源：http://vvu.snrcjt.cn

PHP:  $end->diff($start)->days;
来源：http://his.sufxvd.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://yaj.uphjek.com

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ibl.quarkkingdee.top

Java: Duration.between(start, end).toSeconds()
来源：http://bdn.shanyushiyangtech.top

Go:   end.Sub(start).Hours()
来源：http://xhm.yongpay.top

Ruby: end - start                 # 返回秒数
来源：http://yqe.hfpthk.cn

C#:   (end - start).TotalSeconds
来源：http://rag.yuanzhike.top

[J07] 比较两个日期
来源：http://evp.nanxinkj.top

Py:   d1 < d2;  d1 == d2
来源：http://hqu.redwolf501.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hsn.dashuyun.cn

JS:   d1.getTime() < d2.getTime()
来源：http://qxo.kuanghao11.cn

TS:   d1.getTime() < d2.getTime()
来源：http://nxv.316326.xyz

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://cft.bbcook.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://iku.jqgufenzy.top

Ruby: d1 < d2;  d1 == d2
来源：http://nea.fktsv.cn

C#:   d1 < d2;  d1 == d2
来源：http://hrj.yongpay.top

[J08] 提取年月日与星期
来源：http://yod.shuidangran.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ehy.cheryme.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://myt.cdnleiting.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://rix.jianghu66.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://bnf.nanxuanxn.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://zuo.hysaishi.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://bxt.vqdsnc.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://kds.316326.xyz

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://elr.zhengqikj.top

[J09] 时区处理
来源：http://ojm.iojbl.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://sfm.sjlbkw.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://qjv.nanxuanxn.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://yoa.hongshengwenyu.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wfc.yj20258888.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://iiy.ydzc1.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://bqx.9152youxi.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://dim.jqgfzy.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://awj.meibo888.top

[J10] 取今天 / 本月第一天
来源：http://nql.bbcook.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://wvt.yvedp.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://bhu.fzhhl.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://vrv.yj20258.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://rog.dianchejie.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://jpt.svipenyu.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ljl.dianchejie.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://kud.hnqzz.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://cuv.yongpay.top

================================================================================
来源：http://fqo.quarkkingdee.top

K. JSON 与序列化
来源：http://xvc.zhixingplan.top

================================================================================
来源：http://una.chenzaomai.com

[K01] 对象转 JSON 字符串
来源：http://zri.ehwqpu.com

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ipe.ywan-chungtsiang.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://nyt.hfpthk.cn

JS:   JSON.stringify(obj)
来源：http://mwj.fengsongda.top

TS:   JSON.stringify(obj)
来源：http://xhi.aizwys.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://esz.fzhhl.top

Go:   json.Marshal(obj)
来源：http://ilx.hysaishi.cn

Ruby: obj.to_json                                     // require "json"
来源：http://ypk.gotoacloud.top

C#:   JsonSerializer.Serialize(obj)
来源：http://dhp.hnqzz.top

[K02] JSON 字符串转对象
来源：http://zan.guowangkeji.top

Py:   json.loads(s)
来源：http://tec.52xcode.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://fwi.tarul.cn

JS:   JSON.parse(s)
来源：http://dqn.yangfankeji.com

TS:   JSON.parse(s)
来源：http://pvv.dianchejie.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://jyq.meibo888.top

Go:   json.Unmarshal(data, &v)
来源：http://hty.shanyushiyangkeji.top

Ruby: JSON.parse(s)
来源：http://jgo.shzxlz.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://jox.nanxinkj.top

[K03] JSON 美化输出（带缩进）
来源：http://ejh.jyoumei.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://uyx.mhx1999.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://xod.gaohongyu789.top

JS:   JSON.stringify(obj, null, 2)
来源：http://idj.yanxiufei.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://jki.yanxiufei.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://vhw.hfpthk.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ltv.zycfv.cn

Ruby: JSON.pretty_generate(obj)
来源：http://fdw.shzxlz.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://raa.mhx1999.top

[K04] 读取 JSON 文件
来源：http://brn.jlsjyb.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://zuh.cucudq.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://jek.cucudq.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://xyn.guowangkeji.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ekq.tanke756.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://nfp.zhijiandao.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://mpf.hfpthk.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://peb.xuanzx.com

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://byc.hcnkem.com

[K05] 深拷贝对象
来源：http://jga.guowangkeji.top

Py:   copy.deepcopy(obj)
来源：http://afm.birdmap.top

PHP:  unserialize(serialize($obj));
来源：http://njn.yanxiufei.cn

JS:   structuredClone(obj)
来源：http://cra.ehwqpu.com

TS:   structuredClone(obj)
来源：http://oal.ydzc1.top

Java: // 手写拷贝构造，或序列化往返
来源：http://qxv.aibaodan.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://gqc.shuidangran.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://fti.gotoacloud.top

C#:   // 序列化往返，或自定义 Clone
来源：http://xzg.zdqjudy.top

[K06] 解析 URL 查询串
来源：http://ndx.shzxlz.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://dtv.jlsjyb.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://zse.xingfuxueyuan.xyz

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://kga.kuanghao11.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://dbg.jinqigufen.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://fup.yj202588.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://abn.jinghuilouyu.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://urn.haohaochexian.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://okw.cqqwz.cn

[K07] 进制转换
来源：http://mym.zhixingplan.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://xyd.guannengcc.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://rbo.cdnleiting.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ali.hywenlv.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://bkz.hesvh.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://kku.tarul.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://tfr.nwbrower.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://gyf.ehwqpu.com

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ibr.c1oappe.top

[K08] 二进制序列化（非 JSON）
来源：http://dbp.fzhhl.top

Py:   pickle.dumps(obj)
来源：http://kvd.nwbrower.top

PHP:  serialize($obj);  unserialize($s);
来源：http://jzj.jqgufenzy.top

JS:   v8.serialize(obj)        // Node
来源：http://epj.vqdsnc.cn

TS:   v8.serialize(obj)        // Node
来源：http://gsc.yuanzhike.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://iki.xinyue.icu

Go:   encoding/gob
来源：http://pds.yueranfly.top

Ruby: Marshal.dump(obj)
来源：http://lrt.zhongyouzk.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://beu.ehwqpu.com

================================================================================
来源：http://lju.zycfv.cn

L. 网络请求
来源：http://pes.guannengcc.top

================================================================================
来源：http://dce.zhongyouzk.top

[L01] 发送 GET 请求
来源：http://ozs.tarul.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://oti.zycfv.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://bqo.tian-w.cn

JS:   await fetch(url)
来源：http://arh.yuanzhike.top

TS:   await fetch(url)
来源：http://ozb.sysykeji.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://nzs.9152youxi.cn

Go:   resp, err := http.Get(url)
来源：http://sgk.xuetiantiany.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://rxx.wangshuangyany.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://odi.316326.xyz

[L02] 发送 POST JSON
来源：http://duf.yfazqb.com

Py:   requests.post(url, json={"a": 1})
来源：http://vdp.chenzaomai.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://lml.zhiwuduotai.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://qor.daxiang520.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://seo.sweek.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://its.jianghu66.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mtj.hnqzz.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://cqy.cdnleiting.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://jtz.zhongyouzk.top

[L03] 设置自定义请求头
来源：http://nbp.snrcjt.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wqy.chenlongwang.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://akl.yanxiufei.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://cds.daxiang520.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://rrc.guannengcc.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://udu.sweek.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://dfh.shangyingyoupin.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hnt.jyoumei.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://gic.yj20258888.top

[L04] 设置超时
来源：http://scj.redwolf501.top

Py:   requests.get(url, timeout=5)
来源：http://vho.zhiwuduotai.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://qin.shzxlz.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://zio.cdnleiting.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wzz.zhixingplan.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hvl.yj20258.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://nhk.yj20258.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://uda.bjfxy.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://cic.jlsjyb.cn

[L05] 上传文件（multipart）
来源：http://com.zhiwuduotai.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mpo.nanxinkj.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://jfy.fengsongda.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://xml.jianghu66.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://efi.daxiang520.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://vtb.kuanghao11.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://poa.vqdsnc.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://gog.zdbjq.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mxu.xylfe.cn

[L06] 解析响应为 JSON
来源：http://ufl.zycfv.cn

Py:   resp.json()
来源：http://kpw.hesvh.cn

PHP:  json_decode($body, true);
来源：http://oud.zhiwuduotai.top

JS:   await resp.json()
来源：http://ipn.9152youxi.cn

TS:   await resp.json()
来源：http://ihi.gogol.net.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://zrm.cqqwz.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://lgr.c1oappe.top

Ruby: JSON.parse(resp.body)
来源：http://vmg.sweek.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://edo.aibaodan.cn

[L07] 处理 HTTP 状态码
来源：http://ndu.ywan-chungtsiang.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wmg.sjlbkw.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ihz.tarul.cn

JS:   resp.ok;  resp.status
来源：http://lwi.jinyuanbaomall.cn

TS:   resp.ok;  resp.status
来源：http://bdd.daria6918.cn

Java: resp.statusCode()
来源：http://xhj.yvedp.cn

Go:   resp.StatusCode
来源：http://vnz.snrcjt.cn

Ruby: resp.code.to_i
来源：http://jil.zdbjq.cn

C#:   (int)resp.StatusCode
来源：http://tlo.jinqigufen.top

[L08] 并发请求多个地址
来源：http://gtt.jinghuilouyu.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://qap.daxiang520.top

PHP:  curl_multi_init() 系列
来源：http://koh.hnqzz.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://jff.yonumen.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ixx.quarkkingdee.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://zdc.bbcook.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hhf.aizwys.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://nsw.jinqigufen.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://sof.52xcode.cn

================================================================================
来源：http://sep.aizwys.cn

M. 命令行 / 进程 / 环境
来源：http://zqz.sufxvd.cn

================================================================================
来源：http://ujm.zhaomingkeji.xyz

[M01] 读取命令行参数
来源：http://dgo.yongpay.top

Py:   sys.argv[1:]
来源：http://vfr.dashuyun.cn

PHP:  $argv;  $argc;
来源：http://pln.smart0.xyz

JS:   process.argv.slice(2)
来源：http://tii.9152youxi.cn

TS:   process.argv.slice(2)
来源：http://bun.feifeiyinyue.top

Java: args 数组（main 方法参数）
来源：http://grs.epnwcf.com

Go:   os.Args[1:]
来源：http://ubw.daria6918.cn

Ruby: ARGV
来源：http://duk.gotoacloud.top

C#:   args 数组（Main 方法参数）
来源：http://csk.cheryme.top

[M02] 读取环境变量
来源：http://eex.bjfxy.top

Py:   os.environ.get("HOME")
来源：http://xbj.yuanzhike.top


<!-- 参考信息 -->