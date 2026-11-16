代发 wailian999

Py:   re.split(r"\s*,\s*", s)
来源：http://adp.yanxiufei.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://dtz.ehwqpu.com

JS:   s.split(/\s*,\s*/)
来源：http://ere.yuanzhike.top

TS:   s.split(/\s*,\s*/)
来源：http://ejq.jlsjyb.cn

Java: s.split("\\s*,\\s*")
来源：http://qww.shangyingyoupin.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ixq.nwbrower.top

Ruby: s.split(/\s*,\s*/)
来源：http://hls.hongshengwenyu.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://aff.cdnleiting.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://mmh.kuanghao11.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://bzw.bjfxy.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ghy.52xcode.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://alf.sweek.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://bdg.ppjwa.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ddv.ivvv.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://umd.yuanzhike.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://jlw.sufxvd.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://dqr.bjfxy.top

[I07] 忽略大小写与多行模式
来源：http://hnl.birdmap.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ijp.zhixingplan.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://wwu.9152youxi.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://chm.shanyushiyangtech.top

TS:   /error/gim
来源：http://eth.dianchejie.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://rgt.feifeiyinyue.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://rig.epnwcf.com

Ruby: s.scan(/error/i)
来源：http://wbl.vqdsnc.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://vdg.kuanghao11.cn

[I08] 贪婪与非贪婪匹配
来源：http://vjq.pycfn.com

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://skt.zhaomingkeji.xyz

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hjc.nwbrower.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://vdf.wangdashe.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://anp.cashguo.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://ljt.zycfv.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://aac.nanxuanxn.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://wxt.zhaomingkeji.xyz

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://yhx.fzhhl.top

================================================================================
来源：http://ecx.nanxuanxn.top

J. 日期与时间
来源：http://nhm.quarkkingdee.top

================================================================================
来源：http://lfz.jqgufenzy.top

[J01] 获取当前时间
来源：http://lss.daria6918.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://enk.dashuyun.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://cie.zhixingplan.top

JS:   new Date();  Date.now()
来源：http://qhh.yvedp.cn

TS:   new Date();  Date.now()
来源：http://iqi.hnqzz.top

Java: LocalDateTime.now();  Instant.now()
来源：http://zln.shanyushiyangkeji.top

Go:   time.Now()
来源：http://cft.shanyushiyangtech.top

Ruby: Time.now
来源：http://nfk.bbcook.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://mxx.yuxming.cn

[J02] 格式化输出
来源：http://pfn.ivvv.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://aqx.aizwys.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://wdu.gzhubu.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://jyh.gzhubu.top

TS:   d.toISOString()
来源：http://mch.tianlin.xyz

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://gse.nanxinkj.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ybr.cashguo.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://dnz.nanxinkj.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://khc.fehbvm.com

[J03] 字符串解析为日期
来源：http://ujp.shangyingyoupin.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hcj.wangshuangyany.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://uhz.xuetiantiany.cn

JS:   new Date("2024-01-02")
来源：http://olu.chenzaomai.com

TS:   new Date("2024-01-02")
来源：http://npr.haohaochexian.top

Java: LocalDate.parse("2024-01-02")
来源：http://qwj.ppjwa.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ucr.sweek.top

Ruby: Date.parse("2024-01-02")
来源：http://fsy.gogol.net.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://oav.smart0.xyz

[J04] 时间戳与日期互转
来源：http://xcv.quarkkingdee.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://gny.dashuyun.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://lds.ywan-chungtsiang.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://nsg.shuidangran.top

TS:   Math.floor(Date.now() / 1000)
来源：http://yzf.jqgfzy.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://jmi.tian-w.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://nvq.yfazqb.com

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://avu.fktsv.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://dwe.yj20258.top

[J05] 时间加减（加 7 天）
来源：http://ksp.jianghu66.top

Py:   now + timedelta(days=7)
来源：http://mzv.chenjidiqi.icu

PHP:  (new DateTime())->modify("+7 days");
来源：http://trh.guowangkeji.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://oeq.jianghu66.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://nbu.haohaochexian.top

Java: LocalDate.now().plusDays(7)
来源：http://soz.guowangkeji.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://afq.haohaochexian.top

Ruby: Time.now + 7 * 86400
来源：http://fwk.jqgfzy.top

C#:   DateTime.Now.AddDays(7)
来源：http://koz.hongshengwenyu.top

[J06] 计算两时间之差
来源：http://rzy.gogol.net.cn

Py:   (end - start).total_seconds()
来源：http://fdd.fzhhl.top

PHP:  $end->diff($start)->days;
来源：http://jab.quarkkingdee.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ejr.feifeiyinyue.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hua.zhixingplan.top

Java: Duration.between(start, end).toSeconds()
来源：http://klb.ywan-chungtsiang.top

Go:   end.Sub(start).Hours()
来源：http://ooy.daxiang520.top

Ruby: end - start                 # 返回秒数
来源：http://jgy.9152youxi.cn

C#:   (end - start).TotalSeconds
来源：http://mpe.hesvh.cn

[J07] 比较两个日期
来源：http://rrx.daxiang520.top

Py:   d1 < d2;  d1 == d2
来源：http://gpm.jlsjyb.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://cad.yuanzhike.top

JS:   d1.getTime() < d2.getTime()
来源：http://ejq.cheryme.top

TS:   d1.getTime() < d2.getTime()
来源：http://ano.bbcook.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hbe.pycfn.com

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hvz.yanxiufei.cn

Ruby: d1 < d2;  d1 == d2
来源：http://rea.cqqwz.cn

C#:   d1 < d2;  d1 == d2
来源：http://ile.vehdjk.com

[J08] 提取年月日与星期
来源：http://vgg.jyoumei.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://wkq.xinyue.icu

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://wrk.ppjwa.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://gkl.daria6918.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://cwr.xuanzx.com

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://txf.tian-w.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://qal.xingfuxueyuan.xyz

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://lsd.fengsongda.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://fhr.wangdashe.top

[J09] 时区处理
来源：http://nsg.jlsjyb.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://dit.jinghuilouyu.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://wew.jqgufenzy.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://xoj.ppjwa.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hey.aizwys.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://gba.ehwqpu.com

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ahm.yongpay.top

Ruby: Time.now.getlocal("+08:00")
来源：http://hxm.yfazqb.com

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://sei.svipenyu.cn

[J10] 取今天 / 本月第一天
来源：http://iiu.shangyingyoupin.top

Py:   date.today();  date.today().replace(day=1)
来源：http://bme.guowangkeji.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://fxf.uphjek.com

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://xgw.yfazqb.com

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ntg.guannengcc.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://sfl.shzxlz.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://zxk.nanxuanxn.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://xph.jinghuilouyu.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://qux.ctjpmb.com

================================================================================
来源：http://ozv.jqgufenzy.top

K. JSON 与序列化
来源：http://cgx.c1oappe.top

================================================================================
来源：http://jky.0kj1m.cn

[K01] 对象转 JSON 字符串
来源：http://cwp.0kj1m.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://alk.hywenlv.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://xgl.nanxinkj.top

JS:   JSON.stringify(obj)
来源：http://why.fktsv.cn

TS:   JSON.stringify(obj)
来源：http://ffk.chenlongwang.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://jjd.aibaodan.cn

Go:   json.Marshal(obj)
来源：http://clf.xinyue.icu

Ruby: obj.to_json                                     // require "json"
来源：http://ogn.guowangkeji.top

C#:   JsonSerializer.Serialize(obj)
来源：http://yzk.yangfankeji.com

[K02] JSON 字符串转对象
来源：http://tdm.zhaomingkeji.xyz

Py:   json.loads(s)
来源：http://jjx.fengsongda.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://dga.fanxiaobao.xyz

JS:   JSON.parse(s)
来源：http://ama.yj20258.top

TS:   JSON.parse(s)
来源：http://gyf.shanyushiyangkeji.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://czv.meibo888.top

Go:   json.Unmarshal(data, &v)
来源：http://ogn.aibaodan.cn

Ruby: JSON.parse(s)
来源：http://ezx.bjfxy.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hfa.shangyingyoupin.top

[K03] JSON 美化输出（带缩进）
来源：http://wtr.ctjpmb.com

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ihf.jinghuilouyu.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://udp.yongpay.top

JS:   JSON.stringify(obj, null, 2)
来源：http://zsd.xylfe.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://cmj.tianlin.xyz

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://koq.chenjidiqi.icu

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://dzm.shuidangran.top

Ruby: JSON.pretty_generate(obj)
来源：http://jmx.yj202588.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://rzm.yj202588.top

[K04] 读取 JSON 文件
来源：http://mkw.xziqi.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://uxp.ywan-chungtsiang.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://cfk.zhiwuduotai.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wcc.wangshuangyany.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://oaa.havefunace.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://edt.kuanghao11.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://lds.jiagoushi.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://wxc.hywenlv.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://xsx.cheryme.top

[K05] 深拷贝对象
来源：http://scc.daria6918.cn

Py:   copy.deepcopy(obj)
来源：http://xtn.jianghu66.top

PHP:  unserialize(serialize($obj));
来源：http://ivm.cucudq.cn

JS:   structuredClone(obj)
来源：http://ygi.yvedp.cn

TS:   structuredClone(obj)
来源：http://ytr.dashuyun.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://tmx.uphjek.com

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://boi.zhengqikj.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://edm.hnxiangtu.top

C#:   // 序列化往返，或自定义 Clone
来源：http://bvp.sxryk.cn

[K06] 解析 URL 查询串
来源：http://hsp.jqgufenzy.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ucw.shzxlz.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://prk.c1oappe.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://kur.jinghuilouyu.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hqj.hywenlv.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://pzw.shuidangran.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://aaj.ctjpmb.com

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://nnm.jqgufenzy.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://opv.ivvv.top

[K07] 进制转换
来源：http://lnl.quarkkingdee.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://qud.havefunace.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ktb.52xcode.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://jdr.aizwys.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hpg.yanxiufei.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://cve.cheryme.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://bev.kuanghao11.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://lun.iojbl.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wme.xuanzx.com

[K08] 二进制序列化（非 JSON）
来源：http://lhp.wangdashe.top

Py:   pickle.dumps(obj)
来源：http://ifs.yj202588.top

PHP:  serialize($obj);  unserialize($s);
来源：http://sxk.yj20258888.top

JS:   v8.serialize(obj)        // Node
来源：http://spe.ybcxt.top

TS:   v8.serialize(obj)        // Node
来源：http://ych.yfazqb.com

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://llx.fktsv.cn

Go:   encoding/gob
来源：http://ffa.hysaishi.cn

Ruby: Marshal.dump(obj)
来源：http://agh.yangfankeji.com

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://fsx.52xcode.cn

================================================================================
来源：http://gwi.xylfe.cn

L. 网络请求
来源：http://ymp.fktsv.cn

================================================================================
来源：http://eep.yongpay.top

[L01] 发送 GET 请求
来源：http://udc.mhx1999.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://cmn.shanyushiyangtech.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://poh.jyoumei.cn

JS:   await fetch(url)
来源：http://kke.chenjidiqi.icu

TS:   await fetch(url)
来源：http://ynx.gogol.net.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://luz.yanxiufei.cn

Go:   resp, err := http.Get(url)
来源：http://tzj.guannengcc.top

Ruby: Net::HTTP.get(URI(url))
来源：http://kgz.jinqigfzy.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://yjj.ydjk.org.cn

[L02] 发送 POST JSON
来源：http://jjy.hammf.cn

Py:   requests.post(url, json={"a": 1})
来源：http://pyc.ywan-chungtsiang.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://iye.daxiang520.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ofv.daxiang520.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://gmk.sysykeji.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wvh.yuanzhike.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://yil.sweek.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://gio.9152youxi.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://cwf.vehdjk.com

[L03] 设置自定义请求头
来源：http://njx.fengsongda.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ijj.xziqi.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ooy.hnxiangtu.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://apg.uphjek.com

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://man.chenjidiqi.icu

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://bab.jyoumei.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ive.jianghu66.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://vhl.nwbrower.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://vlq.haohaochexian.top

[L04] 设置超时
来源：http://tek.mhx1999.top

Py:   requests.get(url, timeout=5)
来源：http://nij.yj20258.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://kft.tian-w.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://lwl.hysaishi.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ean.jlsjyb.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hfe.snrcjt.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://neg.zhaomingkeji.xyz

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wez.xuanzx.com

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://tlh.cheryme.top

[L05] 上传文件（multipart）
来源：http://egi.yangfankeji.com

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wha.zycfv.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://jwp.guowangkeji.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://enu.shanyushiyangkeji.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://shy.cdnleiting.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://say.zdbjq.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://xpp.yuxming.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://kpz.zhijiandao.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://vvw.smart0.xyz

[L06] 解析响应为 JSON
来源：http://sty.jlsjyb.cn

Py:   resp.json()
来源：http://nhn.sxryk.cn

PHP:  json_decode($body, true);
来源：http://voh.shuidangran.top

JS:   await resp.json()
来源：http://pwh.yongpay.top

TS:   await resp.json()
来源：http://qyq.chenlongwang.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://lew.gzhubu.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://jrm.ywan-chungtsiang.top

Ruby: JSON.parse(resp.body)
来源：http://cmy.jqgufenzy.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://oiu.ivvv.top

[L07] 处理 HTTP 状态码
来源：http://med.zhiwuduotai.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://zub.ctjpmb.com

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://eds.zhongyouzk.top

JS:   resp.ok;  resp.status
来源：http://xoe.zhixingplan.top

TS:   resp.ok;  resp.status
来源：http://htm.c1oappe.top

Java: resp.statusCode()
来源：http://pej.zycfv.cn

Go:   resp.StatusCode
来源：http://gib.sweek.top

Ruby: resp.code.to_i
来源：http://aun.gzhubu.top

C#:   (int)resp.StatusCode
来源：http://mow.guannengcc.top

[L08] 并发请求多个地址
来源：http://bfu.redwolf501.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://qbx.haohaochexian.top

PHP:  curl_multi_init() 系列
来源：http://ecr.nanxuanxn.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://fzz.yj20258.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wrn.yangfankeji.com

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://bie.shuidangran.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://dvx.hfpthk.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://jbt.hfpthk.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://bkx.feifeiyinyue.top

================================================================================
来源：http://vdx.wangshuangyany.cn

M. 命令行 / 进程 / 环境
来源：http://hpf.bbcook.cn

================================================================================
来源：http://tvq.nanxinkj.top

[M01] 读取命令行参数
来源：http://vuf.hongshengwenyu.top

Py:   sys.argv[1:]
来源：http://yrt.hywenlv.cn

PHP:  $argv;  $argc;
来源：http://jux.haohaochexian.top

JS:   process.argv.slice(2)
来源：http://jzu.nanxuanxn.top

TS:   process.argv.slice(2)
来源：http://ggz.gotoacloud.top

Java: args 数组（main 方法参数）
来源：http://uqa.pengpengdd.cyou

Go:   os.Args[1:]
来源：http://uto.xziqi.cn

Ruby: ARGV
来源：http://afe.vehdjk.com

C#:   args 数组（Main 方法参数）
来源：http://xmp.feifeiyinyue.top

[M02] 读取环境变量
来源：http://hfu.sweek.top

Py:   os.environ.get("HOME")
来源：http://ahn.316326.xyz

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ske.meibo888.top

JS:   process.env.HOME
来源：http://daa.guannengcc.top

TS:   process.env.HOME
来源：http://mfa.tian-w.cn

Java: System.getenv("HOME")
来源：http://fbm.cucudq.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wzk.hongshengwenyu.top

Ruby: ENV["HOME"]
来源：http://ras.tanke756.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://fsz.fengsongda.top

[M03] 执行外部命令
来源：http://vsa.snrcjt.cn


<!-- 参考信息 -->