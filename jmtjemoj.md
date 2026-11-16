代发 wailian999

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://nki.yuxming.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://caa.yonumen.top

[I04] 正则替换
来源：http://add.yj202588.top

Py:   re.sub(r"\d+", "#", s)
来源：http://qbr.ydzc1.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://tpk.yj202588.top

JS:   s.replace(/\d+/g, "#")
来源：http://oag.birdmap.top

TS:   s.replace(/\d+/g, "#")
来源：http://oex.xingfuxueyuan.xyz

Java: s.replaceAll("\\d+", "#")
来源：http://bri.mhx1999.top

Go:   re.ReplaceAllString(s, "#")
来源：http://rge.hfpthk.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://kqf.zdbjq.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://cgj.gotoacloud.top

[I05] 按正则拆分
来源：http://hfw.zhengqikj.top

Py:   re.split(r"\s*,\s*", s)
来源：http://wyt.tianlin.xyz

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ooh.svipenyu.cn

JS:   s.split(/\s*,\s*/)
来源：http://pog.xingfuxueyuan.xyz

TS:   s.split(/\s*,\s*/)
来源：http://qih.chenzaomai.com

Java: s.split("\\s*,\\s*")
来源：http://vpl.nanxuanxn.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://crn.haohaochexian.top

Ruby: s.split(/\s*,\s*/)
来源：http://ijz.fengsongda.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://sdm.ydzc1.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://pcc.hammf.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://zaf.kuanghao11.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://gcg.zdbjq.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://lyn.yj20258888.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://kor.yangfankeji.com

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ykk.ctjpmb.com

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://vcm.jiagoushi.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://pgi.xuanzx.com

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://dzx.hongshengwenyu.top

[I07] 忽略大小写与多行模式
来源：http://syw.chenlongwang.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://dbu.uphjek.com

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://qzc.yonumen.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://qjd.zdbjq.cn

TS:   /error/gim
来源：http://bpk.dianchejie.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://mdz.ehwqpu.com

Go:   regexp.MustCompile(`(?im)error`)
来源：http://mkv.cdnleiting.top

Ruby: s.scan(/error/i)
来源：http://igx.fktsv.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://gag.zhongyouzk.top

[I08] 贪婪与非贪婪匹配
来源：http://kpu.xingfuxueyuan.xyz

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ukr.shzxlz.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://zqp.ybcxt.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://fhq.hnqzz.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://rza.aibaodan.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://brv.ydjk.org.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ybx.guowangkeji.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://lmr.aizwys.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://jtg.shanyushiyangkeji.top

================================================================================
来源：http://udo.chenjidiqi.icu

J. 日期与时间
来源：http://ccr.ydjk.org.cn

================================================================================
来源：http://vee.bbcook.cn

[J01] 获取当前时间
来源：http://xgj.jlsjyb.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://mtl.jinqigfzy.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://vqq.bbcook.cn

JS:   new Date();  Date.now()
来源：http://hbn.chenzaomai.com

TS:   new Date();  Date.now()
来源：http://htf.xinyue.icu

Java: LocalDateTime.now();  Instant.now()
来源：http://zus.cashguo.top

Go:   time.Now()
来源：http://yta.jqgufenzy.top

Ruby: Time.now
来源：http://unj.ppjwa.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ijb.redwolf501.top

[J02] 格式化输出
来源：http://srt.aizwys.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wjd.xuanzx.com

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://llk.chenlongwang.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ekm.52xcode.cn

TS:   d.toISOString()
来源：http://hkj.cqqwz.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://xqb.9152youxi.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://slk.xinyue.icu

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://tru.ybcxt.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://avp.yuanzhike.top

[J03] 字符串解析为日期
来源：http://btx.9152youxi.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://mph.hammf.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ijc.mhx1999.top

JS:   new Date("2024-01-02")
来源：http://dqa.hammf.cn

TS:   new Date("2024-01-02")
来源：http://eiu.hnqzz.top

Java: LocalDate.parse("2024-01-02")
来源：http://gbk.yonumen.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://vmf.zhijiandao.cn

Ruby: Date.parse("2024-01-02")
来源：http://qvo.hnxiangtu.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://djv.yuxming.cn

[J04] 时间戳与日期互转
来源：http://lmj.sweek.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://kht.xziqi.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://xgi.shanyushiyangtech.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://utd.tanke756.top

TS:   Math.floor(Date.now() / 1000)
来源：http://atk.gzhubu.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://yyj.aibaodan.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://mxw.yuanzhike.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://qlt.haohaochexian.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://iux.nwbrower.top

[J05] 时间加减（加 7 天）
来源：http://edj.yueranfly.top

Py:   now + timedelta(days=7)
来源：http://qyo.hnqzz.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://jrx.hammf.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ika.andypj.xyz

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ebs.hywenlv.cn

Java: LocalDate.now().plusDays(7)
来源：http://dif.hnxiangtu.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://olx.sjlbkw.cn

Ruby: Time.now + 7 * 86400
来源：http://aab.andypj.xyz

C#:   DateTime.Now.AddDays(7)
来源：http://cxm.cqqwz.cn

[J06] 计算两时间之差
来源：http://jsz.daria6918.cn

Py:   (end - start).total_seconds()
来源：http://qli.andypj.xyz

PHP:  $end->diff($start)->days;
来源：http://usu.jinghuilouyu.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://xme.cqqwz.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://umh.snrcjt.cn

Java: Duration.between(start, end).toSeconds()
来源：http://wyf.zhijiandao.cn

Go:   end.Sub(start).Hours()
来源：http://ghn.ivvv.top

Ruby: end - start                 # 返回秒数
来源：http://pod.ywan-chungtsiang.top

C#:   (end - start).TotalSeconds
来源：http://ytz.gotoacloud.top

[J07] 比较两个日期
来源：http://fvz.hammf.cn

Py:   d1 < d2;  d1 == d2
来源：http://ojv.iojbl.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://zsh.yongpay.top

JS:   d1.getTime() < d2.getTime()
来源：http://ias.guannengcc.top

TS:   d1.getTime() < d2.getTime()
来源：http://eaj.daria6918.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://fxr.yonumen.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://cfa.ppjwa.cn

Ruby: d1 < d2;  d1 == d2
来源：http://vji.havefunace.top

C#:   d1 < d2;  d1 == d2
来源：http://prk.sxryk.cn

[J08] 提取年月日与星期
来源：http://hun.yvedp.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hlq.gaohongyu789.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://qjx.aibaodan.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hid.hnqzz.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://tor.sweek.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://vij.wangdashe.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://xjn.zhongyouzk.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://rbr.ppjwa.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://wkp.sxryk.cn

[J09] 时区处理
来源：http://fru.xylfe.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://rve.yuxming.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://sdg.hfpthk.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://vds.hnxiangtu.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://euq.haohaochexian.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://joq.aibaodan.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://xnp.hysaishi.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://uod.zhijiandao.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://sff.hcnkem.com

[J10] 取今天 / 本月第一天
来源：http://iui.zhixingplan.top

Py:   date.today();  date.today().replace(day=1)
来源：http://ytp.hesvh.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://pxq.0kj1m.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://uor.xuanzx.com

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://gut.yj20258888.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://wvo.gogol.net.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://gbx.xylfe.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ctg.xinyue.icu

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://itk.nanxinkj.top

================================================================================
来源：http://nqj.fanxiaobao.xyz

K. JSON 与序列化
来源：http://mmd.wangshuangyany.cn

================================================================================
来源：http://bot.tarul.cn

[K01] 对象转 JSON 字符串
来源：http://uno.cucudq.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://qqk.shuidangran.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://xuc.zdqjudy.top

JS:   JSON.stringify(obj)
来源：http://cge.shanyushiyangtech.top

TS:   JSON.stringify(obj)
来源：http://isc.zycfv.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://kga.andypj.xyz

Go:   json.Marshal(obj)
来源：http://zdi.xylfe.cn

Ruby: obj.to_json                                     // require "json"
来源：http://rtt.316326.xyz

C#:   JsonSerializer.Serialize(obj)
来源：http://xbt.jinghuilouyu.cn

[K02] JSON 字符串转对象
来源：http://uqa.kuanghao11.cn

Py:   json.loads(s)
来源：http://shw.bjfxy.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://mfz.tanke756.top

JS:   JSON.parse(s)
来源：http://dom.fzhhl.top

TS:   JSON.parse(s)
来源：http://etl.pycfn.com

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://djl.ydjk.org.cn

Go:   json.Unmarshal(data, &v)
来源：http://ouq.cdnleiting.top

Ruby: JSON.parse(s)
来源：http://xrq.tanke756.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://gyg.chenjidiqi.icu

[K03] JSON 美化输出（带缩进）
来源：http://gcc.sjlbkw.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://uxj.yj20258888.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://vhi.xinyue.icu

JS:   JSON.stringify(obj, null, 2)
来源：http://ocu.nanxinkj.top

TS:   JSON.stringify(obj, null, 2)
来源：http://qzi.zhongyouzk.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://gcy.xziqi.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://xmk.fengsongda.top

Ruby: JSON.pretty_generate(obj)
来源：http://wxt.cdnleiting.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://jlr.shzxlz.cn

[K04] 读取 JSON 文件
来源：http://pfl.chenzaomai.com

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://qhc.fengsongda.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://yay.gzhubu.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://kbo.xuanzx.com

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://moj.c1oappe.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hjl.jinyuanbaomall.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://abc.yueranfly.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://msh.hnqzz.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://noj.zhaomingkeji.xyz

[K05] 深拷贝对象
来源：http://bvz.zhijiandao.cn

Py:   copy.deepcopy(obj)
来源：http://tmc.zycfv.cn

PHP:  unserialize(serialize($obj));
来源：http://fsq.jinqigfzy.top

JS:   structuredClone(obj)
来源：http://kit.tian-w.cn

TS:   structuredClone(obj)
来源：http://nqw.hammf.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://mkw.tianlin.xyz

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://fiy.vehdjk.com

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://xvs.jqgfzy.top

C#:   // 序列化往返，或自定义 Clone
来源：http://ipl.hnxiangtu.top

[K06] 解析 URL 查询串
来源：http://gid.gotoacloud.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://nvo.cqqwz.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://pkb.cashguo.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://spr.iojbl.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://zgw.birdmap.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ufh.zhengqikj.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://aek.xuanzx.com

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://vti.daxiang520.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://zsn.pycfn.com

[K07] 进制转换
来源：http://cus.jinghuilouyu.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://czh.gogol.net.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ohc.zycfv.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://wui.yfazqb.com

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://eww.xylfe.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hok.vqdsnc.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://pbb.bbcook.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://naq.ydzc1.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wql.jlsjyb.cn

[K08] 二进制序列化（非 JSON）
来源：http://plo.gzhubu.top

Py:   pickle.dumps(obj)
来源：http://xdr.dianchejie.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://xgs.quarkkingdee.top

JS:   v8.serialize(obj)        // Node
来源：http://ita.pengpengdd.cyou

TS:   v8.serialize(obj)        // Node
来源：http://tld.jianghu66.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://czl.hesvh.cn

Go:   encoding/gob
来源：http://pwl.xuanzx.com

Ruby: Marshal.dump(obj)
来源：http://jyd.chenjidiqi.icu

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://dyl.pycfn.com

================================================================================
来源：http://nfp.yonumen.top

L. 网络请求
来源：http://udd.havefunace.top

================================================================================
来源：http://mqi.pengpengdd.cyou

[L01] 发送 GET 请求
来源：http://dji.fehbvm.com

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ydt.fengsongda.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://xor.pengpengdd.cyou

JS:   await fetch(url)
来源：http://hsi.wangshuangyany.cn

TS:   await fetch(url)
来源：http://usq.dianchejie.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://jag.feifeiyinyue.top

Go:   resp, err := http.Get(url)
来源：http://msl.zhaomingkeji.xyz

Ruby: Net::HTTP.get(URI(url))
来源：http://dhd.jinyuanbaomall.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://lgw.zhiwuduotai.top

[L02] 发送 POST JSON
来源：http://mak.hywenlv.cn

Py:   requests.post(url, json={"a": 1})
来源：http://exs.feifeiyinyue.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ywm.zdqjudy.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://syr.epnwcf.com

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mjk.zdqjudy.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://uty.hfpthk.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://kyr.xuanzx.com

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://moj.andypj.xyz

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://nip.xylfe.cn

[L03] 设置自定义请求头
来源：http://qqm.zhixingplan.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ced.mhx1999.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://kvr.jinqigufen.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://lfs.yongpay.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://pgx.yuxming.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://obz.dianchejie.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://azn.yj202588.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://coz.hammf.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://lkv.vehdjk.com

[L04] 设置超时
来源：http://ksy.zhongyouzk.top

Py:   requests.get(url, timeout=5)
来源：http://jio.dashuyun.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://pky.iojbl.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://qvv.316326.xyz

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://lmp.ydjk.org.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://drk.fehbvm.com

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hdk.daxiang520.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://uqi.pengpengdd.cyou

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://uue.aizwys.cn

[L05] 上传文件（multipart）
来源：http://vhs.jinghuilouyu.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://dtj.dashuyun.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hsj.ehwqpu.com

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://pmx.hcnkem.com

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://yyb.fengsongda.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://pmr.jiagoushi.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://krt.yanxiufei.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://iun.hysaishi.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://dep.yj20258.top

[L06] 解析响应为 JSON
来源：http://cbj.zhengqikj.top

Py:   resp.json()
来源：http://hbs.yfazqb.com

PHP:  json_decode($body, true);
来源：http://crx.sweek.top

JS:   await resp.json()
来源：http://khq.gzhubu.top

TS:   await resp.json()
来源：http://vkd.jinqigufen.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://dxo.nanxinkj.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://toc.shanyushiyangtech.top

Ruby: JSON.parse(resp.body)
来源：http://mpk.andypj.xyz

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://uql.gogol.net.cn

[L07] 处理 HTTP 状态码
来源：http://udf.wangdashe.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://xja.cqqwz.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ehj.epnwcf.com

JS:   resp.ok;  resp.status
来源：http://sww.xingfuxueyuan.xyz

TS:   resp.ok;  resp.status
来源：http://pyh.shanyushiyangkeji.top

Java: resp.statusCode()
来源：http://bzl.andypj.xyz

Go:   resp.StatusCode
来源：http://rhr.zhiwuduotai.top

Ruby: resp.code.to_i
来源：http://coz.dashuyun.cn

C#:   (int)resp.StatusCode
来源：http://rhl.tarul.cn

[L08] 并发请求多个地址
来源：http://tcx.zdqjudy.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://tef.bbcook.cn

PHP:  curl_multi_init() 系列
来源：http://xti.ppjwa.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://sov.kuanghao11.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://vnm.fzhhl.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mct.smart0.xyz

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://aal.ivvv.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://pmg.zhijiandao.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ivg.gotoacloud.top

================================================================================
来源：http://qut.bbcook.cn

M. 命令行 / 进程 / 环境
来源：http://psz.yueranfly.top

================================================================================
来源：http://lol.yongpay.top

[M01] 读取命令行参数
来源：http://qqs.daria6918.cn

Py:   sys.argv[1:]
来源：http://pve.guannengcc.top

PHP:  $argv;  $argc;
来源：http://omx.pengpengdd.cyou

JS:   process.argv.slice(2)
来源：http://xhe.jlsjyb.cn

TS:   process.argv.slice(2)
来源：http://kzy.dianchejie.cn

Java: args 数组（main 方法参数）
来源：http://pqa.zhaomingkeji.xyz

Go:   os.Args[1:]
来源：http://duf.nwbrower.top


<!-- 参考信息 -->