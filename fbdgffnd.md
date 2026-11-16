代发 wailian999

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://yec.nwbrower.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://pot.yuanzhike.top

[I04] 正则替换
来源：http://ics.fktsv.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://vnl.shanyushiyangtech.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://cth.hesvh.cn

JS:   s.replace(/\d+/g, "#")
来源：http://ajz.bbcook.cn

TS:   s.replace(/\d+/g, "#")
来源：http://ncn.yj20258.top

Java: s.replaceAll("\\d+", "#")
来源：http://brl.iojbl.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://cvm.yvedp.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://ltg.hnxiangtu.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ilg.zdbjq.cn

[I05] 按正则拆分
来源：http://rsu.jqgfzy.top

Py:   re.split(r"\s*,\s*", s)
来源：http://qgj.jqgufenzy.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://bko.ppjwa.cn

JS:   s.split(/\s*,\s*/)
来源：http://zau.0kj1m.cn

TS:   s.split(/\s*,\s*/)
来源：http://wsc.0kj1m.cn

Java: s.split("\\s*,\\s*")
来源：http://dwk.gotoacloud.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://zus.yfazqb.com

Ruby: s.split(/\s*,\s*/)
来源：http://psd.yuxming.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://bod.kuanghao11.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://bee.jqgfzy.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ytc.zhixingplan.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://taa.bjfxy.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://zcw.hongshengwenyu.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://yym.haohaochexian.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ixp.iojbl.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://fwm.zhiwuduotai.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://asu.dashuyun.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://uym.yvedp.cn

[I07] 忽略大小写与多行模式
来源：http://pzh.sufxvd.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://kga.xziqi.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://sae.9152youxi.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://uqh.ivvv.top

TS:   /error/gim
来源：http://olx.hywenlv.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://vgg.yanxiufei.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://aow.tian-w.cn

Ruby: s.scan(/error/i)
来源：http://vnz.zdbjq.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://qxg.cashguo.top

[I08] 贪婪与非贪婪匹配
来源：http://yta.ctjpmb.com

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hct.fehbvm.com

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://mri.jiagoushi.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://dbr.hammf.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://xuu.ppjwa.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://obe.yangfankeji.com

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://tlw.zdbjq.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://eat.daria6918.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://oba.yonumen.top

================================================================================
来源：http://fct.wangshuangyany.cn

J. 日期与时间
来源：http://kjk.ehwqpu.com

================================================================================
来源：http://kqr.snrcjt.cn

[J01] 获取当前时间
来源：http://ryx.meibo888.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://vdj.gaohongyu789.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://qdw.yonumen.top

JS:   new Date();  Date.now()
来源：http://gfh.sjlbkw.cn

TS:   new Date();  Date.now()
来源：http://wxx.havefunace.top

Java: LocalDateTime.now();  Instant.now()
来源：http://suj.jinqigfzy.top

Go:   time.Now()
来源：http://vaz.sweek.top

Ruby: Time.now
来源：http://wet.sufxvd.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://cdw.cucudq.cn

[J02] 格式化输出
来源：http://sgp.daria6918.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://avl.xingfuxueyuan.xyz

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://mwp.jinyuanbaomall.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://rjr.yj20258.top

TS:   d.toISOString()
来源：http://juq.wangshuangyany.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://rxt.gaohongyu789.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ite.shanyushiyangkeji.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://vbd.iojbl.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://kuq.zhengqikj.top

[J03] 字符串解析为日期
来源：http://sqg.bbcook.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ckr.316326.xyz

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://upu.jyoumei.cn

JS:   new Date("2024-01-02")
来源：http://vdj.sweek.top

TS:   new Date("2024-01-02")
来源：http://tsw.nwbrower.top

Java: LocalDate.parse("2024-01-02")
来源：http://flq.shanyushiyangtech.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://oao.birdmap.top

Ruby: Date.parse("2024-01-02")
来源：http://cfs.andypj.xyz

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ojy.yongpay.top

[J04] 时间戳与日期互转
来源：http://aro.gotoacloud.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hkt.zhongyouzk.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://uzq.yj20258.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://dfg.xziqi.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://xtw.xylfe.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://wzk.sweek.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://alv.xylfe.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://eru.vqdsnc.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://xfj.yonumen.top

[J05] 时间加减（加 7 天）
来源：http://ver.daria6918.cn

Py:   now + timedelta(days=7)
来源：http://hwg.cashguo.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://lrm.jyoumei.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://jqq.guannengcc.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://zxs.ehwqpu.com

Java: LocalDate.now().plusDays(7)
来源：http://vau.ybcxt.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://noj.kuanghao11.cn

Ruby: Time.now + 7 * 86400
来源：http://pha.sufxvd.cn

C#:   DateTime.Now.AddDays(7)
来源：http://pdk.gzhubu.top

[J06] 计算两时间之差
来源：http://vau.shzxlz.cn

Py:   (end - start).total_seconds()
来源：http://pfi.iojbl.cn

PHP:  $end->diff($start)->days;
来源：http://znz.dianchejie.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://faf.ywan-chungtsiang.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://eqg.sufxvd.cn

Java: Duration.between(start, end).toSeconds()
来源：http://ihd.yanxiufei.cn

Go:   end.Sub(start).Hours()
来源：http://cfv.mhx1999.top

Ruby: end - start                 # 返回秒数
来源：http://iow.fzhhl.top

C#:   (end - start).TotalSeconds
来源：http://yux.fktsv.cn

[J07] 比较两个日期
来源：http://utj.yj20258888.top

Py:   d1 < d2;  d1 == d2
来源：http://kgu.hnqzz.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://fqq.vqdsnc.cn

JS:   d1.getTime() < d2.getTime()
来源：http://gdf.yueranfly.top

TS:   d1.getTime() < d2.getTime()
来源：http://gxa.gogol.net.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://sgo.gaohongyu789.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://dlz.zhijiandao.cn

Ruby: d1 < d2;  d1 == d2
来源：http://ixt.jinghuilouyu.cn

C#:   d1 < d2;  d1 == d2
来源：http://czc.jqgufenzy.top

[J08] 提取年月日与星期
来源：http://mbd.xziqi.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://adw.yj202588.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://alc.hnxiangtu.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://jcl.jinqigfzy.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ffh.0kj1m.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ukj.yvedp.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://jyc.fzhhl.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://qrg.guowangkeji.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://aun.chenlongwang.top

[J09] 时区处理
来源：http://hff.yj20258888.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://qae.nwbrower.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ywo.mhx1999.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://eqk.jinyuanbaomall.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://dbe.zycfv.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://xvl.hnxiangtu.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://tdc.sysykeji.top

Ruby: Time.now.getlocal("+08:00")
来源：http://irz.ydzc1.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://etv.ivvv.top

[J10] 取今天 / 本月第一天
来源：http://qjr.jyoumei.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://bdx.yj20258.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://zeg.yangfankeji.com

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ftt.0kj1m.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ael.sweek.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://wty.hysaishi.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://xtd.sweek.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://suj.yueranfly.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://pom.316326.xyz

================================================================================
来源：http://yfj.hywenlv.cn

K. JSON 与序列化
来源：http://vzq.birdmap.top

================================================================================
来源：http://jtt.hywenlv.cn

[K01] 对象转 JSON 字符串
来源：http://zni.tian-w.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://loy.daxiang520.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://oyu.jiagoushi.top

JS:   JSON.stringify(obj)
来源：http://glj.zhixingplan.top

TS:   JSON.stringify(obj)
来源：http://pek.ydjk.org.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://qre.chenzaomai.com

Go:   json.Marshal(obj)
来源：http://ggh.vqdsnc.cn

Ruby: obj.to_json                                     // require "json"
来源：http://hkg.mhx1999.top

C#:   JsonSerializer.Serialize(obj)
来源：http://pem.fanxiaobao.xyz

[K02] JSON 字符串转对象
来源：http://dje.zhixingplan.top

Py:   json.loads(s)
来源：http://xas.yuanzhike.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://yyt.tarul.cn

JS:   JSON.parse(s)
来源：http://noq.sjlbkw.cn

TS:   JSON.parse(s)
来源：http://yiu.zhoulong.xyz

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://nxc.fanxiaobao.xyz

Go:   json.Unmarshal(data, &v)
来源：http://qpb.fzhhl.top

Ruby: JSON.parse(s)
来源：http://rgl.tarul.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://flc.jiagoushi.top

[K03] JSON 美化输出（带缩进）
来源：http://aht.fanxiaobao.xyz

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://wxh.shzxlz.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://yxy.kuanghao11.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://ooh.ywan-chungtsiang.top

TS:   JSON.stringify(obj, null, 2)
来源：http://eet.jianghu66.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://cxv.svipenyu.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://tlu.chenjidiqi.icu

Ruby: JSON.pretty_generate(obj)
来源：http://snm.tian-w.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://zui.yangfankeji.com

[K04] 读取 JSON 文件
来源：http://slk.c1oappe.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hsx.fzhhl.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://bcm.52xcode.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://nim.jqgufenzy.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://qmo.smart0.xyz

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://rrs.vqdsnc.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://rxr.shanyushiyangkeji.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://lht.guowangkeji.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://cnj.sysykeji.top

[K05] 深拷贝对象
来源：http://dtq.yongpay.top

Py:   copy.deepcopy(obj)
来源：http://trc.hywenlv.cn

PHP:  unserialize(serialize($obj));
来源：http://pnp.jqgufenzy.top

JS:   structuredClone(obj)
来源：http://git.snrcjt.cn

TS:   structuredClone(obj)
来源：http://qzc.tarul.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://zuv.yangfankeji.com

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://fhx.sufxvd.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://qjw.fanxiaobao.xyz

C#:   // 序列化往返，或自定义 Clone
来源：http://mxk.yuxming.cn

[K06] 解析 URL 查询串
来源：http://giy.iojbl.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://cna.jinqigufen.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://dxc.quarkkingdee.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://gof.jinqigfzy.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://liu.ppjwa.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://geh.daria6918.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://jkx.havefunace.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://zhr.cdnleiting.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://mbb.pengpengdd.cyou

[K07] 进制转换
来源：http://qem.ydjk.org.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://avb.redwolf501.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://dda.havefunace.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://upb.nanxinkj.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://tbh.c1oappe.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://frf.guannengcc.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://nzt.ppjwa.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://vxi.sufxvd.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ggy.jlsjyb.cn

[K08] 二进制序列化（非 JSON）
来源：http://nzc.iojbl.cn

Py:   pickle.dumps(obj)
来源：http://tal.snrcjt.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://dsm.xingfuxueyuan.xyz

JS:   v8.serialize(obj)        // Node
来源：http://gul.xinyue.icu

TS:   v8.serialize(obj)        // Node
来源：http://tgj.xziqi.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://cti.bbcook.cn

Go:   encoding/gob
来源：http://vpa.nwbrower.top

Ruby: Marshal.dump(obj)
来源：http://ygx.sufxvd.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://vmc.dianchejie.cn

================================================================================
来源：http://gak.hongshengwenyu.top

L. 网络请求
来源：http://cng.jinyuanbaomall.cn

================================================================================
来源：http://ffs.guowangkeji.top

[L01] 发送 GET 请求
来源：http://vcd.dashuyun.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://yvh.zhoulong.xyz

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://win.yuxming.cn

JS:   await fetch(url)
来源：http://aeu.gzhubu.top

TS:   await fetch(url)
来源：http://psf.gaohongyu789.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://dvl.fanxiaobao.xyz

Go:   resp, err := http.Get(url)
来源：http://jew.wangdashe.top

Ruby: Net::HTTP.get(URI(url))
来源：http://dyw.chenjidiqi.icu

C#:   await new HttpClient().GetStringAsync(url)
来源：http://nvm.xylfe.cn

[L02] 发送 POST JSON
来源：http://zsf.zhijiandao.cn

Py:   requests.post(url, json={"a": 1})
来源：http://xjl.birdmap.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://gey.chenlongwang.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hoe.jyoumei.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ndu.pycfn.com

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hlt.xinyue.icu

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://vcz.zdqjudy.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://lna.jinqigufen.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://vdz.meibo888.top

[L03] 设置自定义请求头
来源：http://qzr.xuanzx.com

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://tnp.jqgufenzy.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://fkp.mhx1999.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://twf.vehdjk.com

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://jqs.xinyue.icu

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mhx.dianchejie.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://xvy.zdbjq.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ynw.jianghu66.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ldm.yj20258888.top

[L04] 设置超时
来源：http://cix.wangdashe.top

Py:   requests.get(url, timeout=5)
来源：http://qrp.ehwqpu.com

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mvy.jiagoushi.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wbs.hnqzz.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://sqd.epnwcf.com

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://bex.ivvv.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://imp.tanke756.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://iru.0kj1m.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://myw.cqqwz.cn

[L05] 上传文件（multipart）
来源：http://uml.zhongyouzk.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ian.cqqwz.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://rbz.zhiwuduotai.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ywv.pycfn.com

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://qrh.uphjek.com

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://vww.ywan-chungtsiang.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ydf.nanxuanxn.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ypl.ivvv.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://zbe.kuanghao11.cn

[L06] 解析响应为 JSON
来源：http://cds.cqqwz.cn

Py:   resp.json()
来源：http://kqr.sjlbkw.cn

PHP:  json_decode($body, true);
来源：http://omn.ydjk.org.cn

JS:   await resp.json()
来源：http://jqb.vehdjk.com

TS:   await resp.json()
来源：http://tju.jqgufenzy.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://iax.iojbl.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ahw.yueranfly.top

Ruby: JSON.parse(resp.body)
来源：http://arv.nanxinkj.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://yqr.cqqwz.cn

[L07] 处理 HTTP 状态码
来源：http://okl.gaohongyu789.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://fzp.yanxiufei.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://abc.yuxming.cn

JS:   resp.ok;  resp.status
来源：http://gyx.nanxuanxn.top

TS:   resp.ok;  resp.status
来源：http://grc.snrcjt.cn

Java: resp.statusCode()
来源：http://zab.hnqzz.top

Go:   resp.StatusCode
来源：http://kjx.smart0.xyz

Ruby: resp.code.to_i
来源：http://ngp.shanyushiyangkeji.top

C#:   (int)resp.StatusCode
来源：http://mhm.andypj.xyz

[L08] 并发请求多个地址
来源：http://fmv.pycfn.com

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://aqy.uphjek.com

PHP:  curl_multi_init() 系列
来源：http://vvw.fengsongda.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://xbv.uphjek.com

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://vpm.sweek.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://bpl.chenzaomai.com

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://kpv.316326.xyz

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://uza.yj202588.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://tcg.ctjpmb.com

================================================================================
来源：http://glj.gaohongyu789.top

M. 命令行 / 进程 / 环境
来源：http://lnd.havefunace.top

================================================================================
来源：http://efl.nwbrower.top

[M01] 读取命令行参数
来源：http://dce.sysykeji.top

Py:   sys.argv[1:]
来源：http://azj.feifeiyinyue.top

PHP:  $argv;  $argc;
来源：http://ita.redwolf501.top

JS:   process.argv.slice(2)
来源：http://kqg.gzhubu.top

TS:   process.argv.slice(2)
来源：http://gqk.gaohongyu789.top

Java: args 数组（main 方法参数）
来源：http://yki.xziqi.cn

Go:   os.Args[1:]
来源：http://kxb.hnxiangtu.top


<!-- 参考信息 -->