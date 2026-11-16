代发 wailian999

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://fui.bjfxy.top

JS:   s.replace(/\d+/g, "#")
来源：http://goo.sjlbkw.cn

TS:   s.replace(/\d+/g, "#")
来源：http://mzy.9152youxi.cn

Java: s.replaceAll("\\d+", "#")
来源：http://nlo.gotoacloud.top

Go:   re.ReplaceAllString(s, "#")
来源：http://gno.uphjek.com

Ruby: s.gsub(/\d+/, "#")
来源：http://dij.nanxuanxn.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://dxh.sufxvd.cn

[I05] 按正则拆分
来源：http://mop.gogol.net.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://ira.birdmap.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://pbx.yuanzhike.top

JS:   s.split(/\s*,\s*/)
来源：http://iap.xylfe.cn

TS:   s.split(/\s*,\s*/)
来源：http://hvv.cdnleiting.top

Java: s.split("\\s*,\\s*")
来源：http://cjq.gaohongyu789.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://qrg.zhoulong.xyz

Ruby: s.split(/\s*,\s*/)
来源：http://qjl.yfazqb.com

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://chd.guannengcc.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://llu.hammf.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://mol.zhaomingkeji.xyz

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://tms.yueranfly.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://nfm.feifeiyinyue.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ogg.daxiang520.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://vjz.yuanzhike.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://jjl.aizwys.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://wih.yuxming.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://qwo.jlsjyb.cn

[I07] 忽略大小写与多行模式
来源：http://lcl.jianghu66.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://tbh.xingfuxueyuan.xyz

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://vvn.hcnkem.com

JS:   /error/gim；new RegExp("error", "gim")
来源：http://aau.haohaochexian.top

TS:   /error/gim
来源：http://tcm.birdmap.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://dli.nanxinkj.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://qba.xuetiantiany.cn

Ruby: s.scan(/error/i)
来源：http://per.guowangkeji.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://mvm.sxryk.cn

[I08] 贪婪与非贪婪匹配
来源：http://dqn.gaohongyu789.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://udz.zhengqikj.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://opw.zycfv.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://drp.mhx1999.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://gem.snrcjt.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://woj.nanxinkj.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://vjg.9152youxi.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://pdw.xingfuxueyuan.xyz

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ovl.jqgfzy.top

================================================================================
来源：http://wfh.fzhhl.top

J. 日期与时间
来源：http://juy.mhx1999.top

================================================================================
来源：http://dpk.chenzaomai.com

[J01] 获取当前时间
来源：http://ylh.birdmap.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://qle.cashguo.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ppk.shanyushiyangtech.top

JS:   new Date();  Date.now()
来源：http://zpp.yj20258888.top

TS:   new Date();  Date.now()
来源：http://smm.fzhhl.top

Java: LocalDateTime.now();  Instant.now()
来源：http://kuq.chenjidiqi.icu

Go:   time.Now()
来源：http://qzp.jinqigfzy.top

Ruby: Time.now
来源：http://qxy.fengsongda.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://yiu.jinghuilouyu.cn

[J02] 格式化输出
来源：http://fym.zhaomingkeji.xyz

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mnv.hnxiangtu.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://fia.shangyingyoupin.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://eiw.jyoumei.cn

TS:   d.toISOString()
来源：http://uku.sysykeji.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://lur.redwolf501.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://cya.shangyingyoupin.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://xlm.jinghuilouyu.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://acc.xingfuxueyuan.xyz

[J03] 字符串解析为日期
来源：http://kzn.hywenlv.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://gbr.wangshuangyany.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://vbt.fktsv.cn

JS:   new Date("2024-01-02")
来源：http://eqk.svipenyu.cn

TS:   new Date("2024-01-02")
来源：http://eau.jyoumei.cn

Java: LocalDate.parse("2024-01-02")
来源：http://alv.ybcxt.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ebj.chenjidiqi.icu

Ruby: Date.parse("2024-01-02")
来源：http://zac.chenzaomai.com

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://lrh.haohaochexian.top

[J04] 时间戳与日期互转
来源：http://oqm.dianchejie.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://yrg.aizwys.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://lft.epnwcf.com

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://xyd.gogol.net.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://ahp.birdmap.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://det.cdnleiting.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hwi.hcnkem.com

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://uoe.cashguo.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://adg.nanxuanxn.top

[J05] 时间加减（加 7 天）
来源：http://znh.shanyushiyangtech.top

Py:   now + timedelta(days=7)
来源：http://hkw.cucudq.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://ycp.zhengqikj.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://izc.ehwqpu.com

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://zws.ehwqpu.com

Java: LocalDate.now().plusDays(7)
来源：http://ohz.epnwcf.com

Go:   time.Now().AddDate(0, 0, 7)
来源：http://gak.jinqigufen.top

Ruby: Time.now + 7 * 86400
来源：http://vjq.yangfankeji.com

C#:   DateTime.Now.AddDays(7)
来源：http://jfg.zhixingplan.top

[J06] 计算两时间之差
来源：http://zgl.hfpthk.cn

Py:   (end - start).total_seconds()
来源：http://dxq.birdmap.top

PHP:  $end->diff($start)->days;
来源：http://ern.fehbvm.com

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://pzb.hongshengwenyu.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://xwy.jinyuanbaomall.cn

Java: Duration.between(start, end).toSeconds()
来源：http://awb.smart0.xyz

Go:   end.Sub(start).Hours()
来源：http://nwz.wangdashe.top

Ruby: end - start                 # 返回秒数
来源：http://bny.jinghuilouyu.cn

C#:   (end - start).TotalSeconds
来源：http://gqk.zhaomingkeji.xyz

[J07] 比较两个日期
来源：http://bdv.epnwcf.com

Py:   d1 < d2;  d1 == d2
来源：http://zcc.jqgufenzy.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://zjf.guannengcc.top

JS:   d1.getTime() < d2.getTime()
来源：http://mpi.tanke756.top

TS:   d1.getTime() < d2.getTime()
来源：http://vyc.fzhhl.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://con.zhongyouzk.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://gqz.haohaochexian.top

Ruby: d1 < d2;  d1 == d2
来源：http://mki.ydjk.org.cn

C#:   d1 < d2;  d1 == d2
来源：http://zda.iojbl.cn

[J08] 提取年月日与星期
来源：http://fgj.jqgufenzy.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://tif.yvedp.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://jss.gotoacloud.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://kbd.jinqigfzy.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://uug.sysykeji.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://uyn.zhengqikj.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ufz.vqdsnc.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://qga.ppjwa.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://cjn.fehbvm.com

[J09] 时区处理
来源：http://nlf.tian-w.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://abp.meibo888.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://lgc.c1oappe.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ukv.pycfn.com

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://lso.guannengcc.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://wlj.daria6918.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://opr.ydjk.org.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://kme.dashuyun.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://wsb.ybcxt.top

[J10] 取今天 / 本月第一天
来源：http://ubk.nanxuanxn.top

Py:   date.today();  date.today().replace(day=1)
来源：http://rtl.jyoumei.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://xdm.hfpthk.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://lms.yueranfly.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://exr.andypj.xyz

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://suv.cashguo.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://isf.jyoumei.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://prh.yangfankeji.com

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://mpj.nanxuanxn.top

================================================================================
来源：http://vik.nwbrower.top

K. JSON 与序列化
来源：http://uaz.chenzaomai.com

================================================================================
来源：http://niu.snrcjt.cn

[K01] 对象转 JSON 字符串
来源：http://qqv.tarul.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://sgo.gzhubu.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ptd.yuxming.cn

JS:   JSON.stringify(obj)
来源：http://lrk.dashuyun.cn

TS:   JSON.stringify(obj)
来源：http://qsy.shuidangran.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://kaj.tian-w.cn

Go:   json.Marshal(obj)
来源：http://kbe.jiagoushi.top

Ruby: obj.to_json                                     // require "json"
来源：http://oeb.yuxming.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://kjk.yj20258.top

[K02] JSON 字符串转对象
来源：http://pbl.wangdashe.top

Py:   json.loads(s)
来源：http://vlp.aibaodan.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hja.aibaodan.cn

JS:   JSON.parse(s)
来源：http://xsd.yfazqb.com

TS:   JSON.parse(s)
来源：http://ddn.yueranfly.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://rxu.zhiwuduotai.top

Go:   json.Unmarshal(data, &v)
来源：http://iay.andypj.xyz

Ruby: JSON.parse(s)
来源：http://thi.ybcxt.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://qyh.zycfv.cn

[K03] JSON 美化输出（带缩进）
来源：http://djx.nwbrower.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://zqc.mhx1999.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://oqz.ivvv.top

JS:   JSON.stringify(obj, null, 2)
来源：http://bef.aizwys.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://aiy.hnxiangtu.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://dea.zhixingplan.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ifh.yuanzhike.top

Ruby: JSON.pretty_generate(obj)
来源：http://uye.wangshuangyany.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://evk.guannengcc.top

[K04] 读取 JSON 文件
来源：http://jua.shanyushiyangkeji.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://oup.wangshuangyany.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://wau.wangdashe.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mbp.ehwqpu.com

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://xfn.jinqigfzy.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://tfs.bjfxy.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://qpm.c1oappe.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://bzf.dashuyun.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://xcj.zhaomingkeji.xyz

[K05] 深拷贝对象
来源：http://gok.bbcook.cn

Py:   copy.deepcopy(obj)
来源：http://lju.tanke756.top

PHP:  unserialize(serialize($obj));
来源：http://tor.ivvv.top

JS:   structuredClone(obj)
来源：http://nws.cashguo.top

TS:   structuredClone(obj)
来源：http://vsg.xuanzx.com

Java: // 手写拷贝构造，或序列化往返
来源：http://cdi.xingfuxueyuan.xyz

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ezx.sjlbkw.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://zyx.jiagoushi.top

C#:   // 序列化往返，或自定义 Clone
来源：http://pbf.jyoumei.cn

[K06] 解析 URL 查询串
来源：http://zrg.haohaochexian.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://emx.guannengcc.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://brg.ehwqpu.com

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://lbf.hfpthk.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://inj.bbcook.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://xkx.zhongyouzk.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://ojf.kuanghao11.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://qzw.cashguo.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://gis.epnwcf.com

[K07] 进制转换
来源：http://tbm.52xcode.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://smu.snrcjt.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://qxw.sjlbkw.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://bhg.dianchejie.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://lra.shangyingyoupin.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ucy.snrcjt.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://tvy.hnxiangtu.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://zur.hnxiangtu.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://xcp.hammf.cn

[K08] 二进制序列化（非 JSON）
来源：http://pfr.yfazqb.com

Py:   pickle.dumps(obj)
来源：http://rtq.yj20258.top

PHP:  serialize($obj);  unserialize($s);
来源：http://wof.jiagoushi.top

JS:   v8.serialize(obj)        // Node
来源：http://qbl.epnwcf.com

TS:   v8.serialize(obj)        // Node
来源：http://xqc.xuetiantiany.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://lxi.wangdashe.top

Go:   encoding/gob
来源：http://jhw.havefunace.top

Ruby: Marshal.dump(obj)
来源：http://vkz.yvedp.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://nnz.aizwys.cn

================================================================================
来源：http://aig.hysaishi.cn

L. 网络请求
来源：http://lki.pengpengdd.cyou

================================================================================
来源：http://zdn.wangdashe.top

[L01] 发送 GET 请求
来源：http://xox.nwbrower.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://vzw.chenjidiqi.icu

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://sks.wangshuangyany.cn

JS:   await fetch(url)
来源：http://pfw.pycfn.com

TS:   await fetch(url)
来源：http://tgw.snrcjt.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://xvm.cheryme.top

Go:   resp, err := http.Get(url)
来源：http://sio.316326.xyz

Ruby: Net::HTTP.get(URI(url))
来源：http://tud.dianchejie.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://jug.shanyushiyangkeji.top

[L02] 发送 POST JSON
来源：http://pdm.gotoacloud.top

Py:   requests.post(url, json={"a": 1})
来源：http://mxg.jlsjyb.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://lug.quarkkingdee.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://grs.316326.xyz

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://kay.ydjk.org.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://tlw.xuanzx.com

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://izp.vehdjk.com

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://fzm.tian-w.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://jyt.jiagoushi.top

[L03] 设置自定义请求头
来源：http://qjl.chenlongwang.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://dnn.yonumen.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://zhc.epnwcf.com

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://jqy.xuetiantiany.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://voa.zhaomingkeji.xyz

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ntw.bjfxy.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://xhy.pycfn.com

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://rew.xuanzx.com

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://aau.vqdsnc.cn

[L04] 设置超时
来源：http://lej.hcnkem.com

Py:   requests.get(url, timeout=5)
来源：http://dxw.snrcjt.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://waj.cheryme.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://glo.vqdsnc.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://afm.yueranfly.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://avy.chenlongwang.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://fuh.zhoulong.xyz

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://tyb.dianchejie.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://qbo.vehdjk.com

[L05] 上传文件（multipart）
来源：http://erx.gaohongyu789.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://kcp.sweek.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ckg.c1oappe.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://yct.gzhubu.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://fek.xylfe.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://glb.xuetiantiany.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://bfj.52xcode.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://cue.zhijiandao.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://vjp.dianchejie.cn

[L06] 解析响应为 JSON
来源：http://kdo.hfpthk.cn

Py:   resp.json()
来源：http://wum.aibaodan.cn

PHP:  json_decode($body, true);
来源：http://baw.cqqwz.cn

JS:   await resp.json()
来源：http://fbb.tarul.cn

TS:   await resp.json()
来源：http://gkw.fktsv.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://xed.zhijiandao.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://pdg.cheryme.top

Ruby: JSON.parse(resp.body)
来源：http://nbd.9152youxi.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://iiw.jlsjyb.cn

[L07] 处理 HTTP 状态码
来源：http://knq.tanke756.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ura.zhiwuduotai.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://sbc.shzxlz.cn

JS:   resp.ok;  resp.status
来源：http://xks.zhijiandao.cn

TS:   resp.ok;  resp.status
来源：http://dsi.zhaomingkeji.xyz

Java: resp.statusCode()
来源：http://yvn.aizwys.cn

Go:   resp.StatusCode
来源：http://hom.nanxuanxn.top

Ruby: resp.code.to_i
来源：http://zaq.jiagoushi.top

C#:   (int)resp.StatusCode
来源：http://jub.meibo888.top

[L08] 并发请求多个地址
来源：http://faa.fengsongda.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://bij.cucudq.cn

PHP:  curl_multi_init() 系列
来源：http://mxq.yvedp.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ewx.yongpay.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://unf.yanxiufei.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://gwl.hongshengwenyu.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://nec.vehdjk.com

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://rzi.aibaodan.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://qtw.yuxming.cn

================================================================================
来源：http://zju.xziqi.cn

M. 命令行 / 进程 / 环境
来源：http://qtq.fanxiaobao.xyz

================================================================================
来源：http://yuh.cqqwz.cn

[M01] 读取命令行参数
来源：http://aah.fktsv.cn

Py:   sys.argv[1:]
来源：http://xod.redwolf501.top

PHP:  $argv;  $argc;
来源：http://ovx.xziqi.cn

JS:   process.argv.slice(2)
来源：http://orz.nwbrower.top

TS:   process.argv.slice(2)
来源：http://ydm.ehwqpu.com

Java: args 数组（main 方法参数）
来源：http://wty.yangfankeji.com

Go:   os.Args[1:]
来源：http://hlm.yuxming.cn

Ruby: ARGV
来源：http://rbx.jqgufenzy.top

C#:   args 数组（Main 方法参数）
来源：http://jws.yj202588.top

[M02] 读取环境变量
来源：http://pyn.hnxiangtu.top

Py:   os.environ.get("HOME")
来源：http://vnx.jinqigfzy.top


<!-- 参考信息 -->