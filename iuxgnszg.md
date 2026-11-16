代发 wailian999

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://rjr.wangshuangyany.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://igw.xinyue.icu

[I04] 正则替换
来源：http://fdt.shzxlz.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://ufd.zhijiandao.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://fey.hongshengwenyu.top

JS:   s.replace(/\d+/g, "#")
来源：http://fnh.yanxiufei.cn

TS:   s.replace(/\d+/g, "#")
来源：http://kxe.shanyushiyangtech.top

Java: s.replaceAll("\\d+", "#")
来源：http://fki.birdmap.top

Go:   re.ReplaceAllString(s, "#")
来源：http://mgw.fehbvm.com

Ruby: s.gsub(/\d+/, "#")
来源：http://hti.kuanghao11.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://uqu.cqqwz.cn

[I05] 按正则拆分
来源：http://fps.nwbrower.top

Py:   re.split(r"\s*,\s*", s)
来源：http://hxo.shzxlz.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://fay.jqgfzy.top

JS:   s.split(/\s*,\s*/)
来源：http://ukq.smart0.xyz

TS:   s.split(/\s*,\s*/)
来源：http://wwx.xuanzx.com

Java: s.split("\\s*,\\s*")
来源：http://wow.cheryme.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://aqv.yfazqb.com

Ruby: s.split(/\s*,\s*/)
来源：http://veb.tianlin.xyz

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://jic.fktsv.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://nds.zycfv.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hph.9152youxi.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://pwa.yueranfly.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://lnc.fktsv.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://efr.zhiwuduotai.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://xyd.yj20258.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://vrh.yanxiufei.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://aaz.xylfe.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://rga.vqdsnc.cn

[I07] 忽略大小写与多行模式
来源：http://ttg.pycfn.com

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hsz.xuetiantiany.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hdu.jqgfzy.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://dei.ivvv.top

TS:   /error/gim
来源：http://gsv.redwolf501.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://qmi.jqgufenzy.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://rrn.andypj.xyz

Ruby: s.scan(/error/i)
来源：http://bop.shuidangran.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://vud.nwbrower.top

[I08] 贪婪与非贪婪匹配
来源：http://flv.hammf.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://zvo.guowangkeji.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://lvf.quarkkingdee.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://lho.aizwys.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://nqv.meibo888.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://nos.chenzaomai.com

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://fqi.xylfe.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://qzh.jinghuilouyu.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hxo.nanxuanxn.top

================================================================================
来源：http://avt.pengpengdd.cyou

J. 日期与时间
来源：http://qfj.havefunace.top

================================================================================
来源：http://ufn.sxryk.cn

[J01] 获取当前时间
来源：http://div.shuidangran.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://jcy.dashuyun.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hdz.jqgufenzy.top

JS:   new Date();  Date.now()
来源：http://wbd.9152youxi.cn

TS:   new Date();  Date.now()
来源：http://axp.hammf.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://iww.yongpay.top

Go:   time.Now()
来源：http://fsa.gotoacloud.top

Ruby: Time.now
来源：http://jxm.dianchejie.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ixu.zycfv.cn

[J02] 格式化输出
来源：http://mht.hnqzz.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://xji.dashuyun.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://vsq.guannengcc.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://jzp.cashguo.top

TS:   d.toISOString()
来源：http://wcz.tianlin.xyz

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://vbq.dashuyun.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://duy.fanxiaobao.xyz

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://jgv.wangshuangyany.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://rgm.ppjwa.cn

[J03] 字符串解析为日期
来源：http://nob.9152youxi.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://bil.haohaochexian.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://lxk.vqdsnc.cn

JS:   new Date("2024-01-02")
来源：http://eet.jyoumei.cn

TS:   new Date("2024-01-02")
来源：http://apa.haohaochexian.top

Java: LocalDate.parse("2024-01-02")
来源：http://odz.jqgufenzy.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hyp.jinghuilouyu.cn

Ruby: Date.parse("2024-01-02")
来源：http://amx.gaohongyu789.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://vmr.chenzaomai.com

[J04] 时间戳与日期互转
来源：http://jkm.jlsjyb.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://vds.cucudq.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ydq.wangdashe.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://rit.daxiang520.top

TS:   Math.floor(Date.now() / 1000)
来源：http://zoy.cashguo.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://bvb.yvedp.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://rix.chenzaomai.com

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://gyb.jlsjyb.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://nvf.ybcxt.top

[J05] 时间加减（加 7 天）
来源：http://sqa.gzhubu.top

Py:   now + timedelta(days=7)
来源：http://lmm.gzhubu.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://tgz.wangdashe.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://wqe.xingfuxueyuan.xyz

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://eoc.jinghuilouyu.cn

Java: LocalDate.now().plusDays(7)
来源：http://qjs.xinyue.icu

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hij.jqgufenzy.top

Ruby: Time.now + 7 * 86400
来源：http://ajq.zhixingplan.top

C#:   DateTime.Now.AddDays(7)
来源：http://frn.chenlongwang.top

[J06] 计算两时间之差
来源：http://tvh.fengsongda.top

Py:   (end - start).total_seconds()
来源：http://obx.ivvv.top

PHP:  $end->diff($start)->days;
来源：http://lil.birdmap.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://qmq.svipenyu.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://qhl.dianchejie.cn

Java: Duration.between(start, end).toSeconds()
来源：http://ohz.daria6918.cn

Go:   end.Sub(start).Hours()
来源：http://qrl.ivvv.top

Ruby: end - start                 # 返回秒数
来源：http://bwv.fengsongda.top

C#:   (end - start).TotalSeconds
来源：http://rxr.jqgfzy.top

[J07] 比较两个日期
来源：http://exe.vehdjk.com

Py:   d1 < d2;  d1 == d2
来源：http://jyp.dianchejie.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://bkj.yangfankeji.com

JS:   d1.getTime() < d2.getTime()
来源：http://mxw.haohaochexian.top

TS:   d1.getTime() < d2.getTime()
来源：http://iuc.havefunace.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://lhd.zhengqikj.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://zye.jqgufenzy.top

Ruby: d1 < d2;  d1 == d2
来源：http://xfr.9152youxi.cn

C#:   d1 < d2;  d1 == d2
来源：http://mls.snrcjt.cn

[J08] 提取年月日与星期
来源：http://tcn.cucudq.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hua.hfpthk.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hyt.xuetiantiany.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://iec.xuanzx.com

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ksg.aibaodan.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://sob.wangdashe.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://mui.hcnkem.com

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hpd.xylfe.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://snl.jyoumei.cn

[J09] 时区处理
来源：http://ehn.gzhubu.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://fob.ehwqpu.com

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ylx.zdqjudy.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://bcx.meibo888.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://uez.jianghu66.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://srb.jinyuanbaomall.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://nmb.nanxuanxn.top

Ruby: Time.now.getlocal("+08:00")
来源：http://dav.iojbl.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://bxs.xingfuxueyuan.xyz

[J10] 取今天 / 本月第一天
来源：http://afa.zhengqikj.top

Py:   date.today();  date.today().replace(day=1)
来源：http://yfu.sufxvd.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://rji.chenjidiqi.icu

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ved.yueranfly.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://avg.haohaochexian.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://grk.snrcjt.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://tdt.jiagoushi.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://jur.shuidangran.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://fmy.zhaomingkeji.xyz

================================================================================
来源：http://lpy.gogol.net.cn

K. JSON 与序列化
来源：http://lus.zhixingplan.top

================================================================================
来源：http://jwk.yongpay.top

[K01] 对象转 JSON 字符串
来源：http://zab.xuetiantiany.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://okl.sweek.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://oph.epnwcf.com

JS:   JSON.stringify(obj)
来源：http://dnh.pycfn.com

TS:   JSON.stringify(obj)
来源：http://eyx.jinghuilouyu.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ooh.pycfn.com

Go:   json.Marshal(obj)
来源：http://nea.shanyushiyangkeji.top

Ruby: obj.to_json                                     // require "json"
来源：http://sak.zhixingplan.top

C#:   JsonSerializer.Serialize(obj)
来源：http://aie.ivvv.top

[K02] JSON 字符串转对象
来源：http://ewe.yfazqb.com

Py:   json.loads(s)
来源：http://olb.xingfuxueyuan.xyz

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://aso.zdqjudy.top

JS:   JSON.parse(s)
来源：http://vmg.ctjpmb.com

TS:   JSON.parse(s)
来源：http://swx.yuxming.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://nyd.chenzaomai.com

Go:   json.Unmarshal(data, &v)
来源：http://odr.zhixingplan.top

Ruby: JSON.parse(s)
来源：http://apz.hammf.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ehx.yanxiufei.cn

[K03] JSON 美化输出（带缩进）
来源：http://bbt.52xcode.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://rry.sxryk.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://zzx.jinghuilouyu.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://wcc.sufxvd.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://yby.316326.xyz

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://syt.zhoulong.xyz

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ria.zycfv.cn

Ruby: JSON.pretty_generate(obj)
来源：http://snn.52xcode.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://zcs.xylfe.cn

[K04] 读取 JSON 文件
来源：http://kxi.tian-w.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://izv.yangfankeji.com

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://vkx.sweek.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hfq.cashguo.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://vwp.yj202588.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://aax.aibaodan.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://oby.jinghuilouyu.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://bhz.sysykeji.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ihq.sxryk.cn

[K05] 深拷贝对象
来源：http://vmj.feifeiyinyue.top

Py:   copy.deepcopy(obj)
来源：http://ffs.zhiwuduotai.top

PHP:  unserialize(serialize($obj));
来源：http://xkr.cdnleiting.top

JS:   structuredClone(obj)
来源：http://tly.fengsongda.top

TS:   structuredClone(obj)
来源：http://muq.tanke756.top

Java: // 手写拷贝构造，或序列化往返
来源：http://hxo.yanxiufei.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://yqf.ctjpmb.com

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://sxu.sufxvd.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://tiu.aibaodan.cn

[K06] 解析 URL 查询串
来源：http://cvr.fehbvm.com

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://tbd.yangfankeji.com

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://dpc.xuetiantiany.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://zsf.epnwcf.com

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://cwz.nanxuanxn.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mzs.haohaochexian.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://hjp.jlsjyb.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://jpj.vqdsnc.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://okk.fanxiaobao.xyz

[K07] 进制转换
来源：http://vir.yj202588.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ozh.ehwqpu.com

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://fkm.fengsongda.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://bhi.jlsjyb.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://spc.vqdsnc.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://nrh.cashguo.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ipq.gzhubu.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://bcz.yuxming.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://flb.cheryme.top

[K08] 二进制序列化（非 JSON）
来源：http://omz.yfazqb.com

Py:   pickle.dumps(obj)
来源：http://hdv.jiagoushi.top

PHP:  serialize($obj);  unserialize($s);
来源：http://ylp.hongshengwenyu.top

JS:   v8.serialize(obj)        // Node
来源：http://uim.9152youxi.cn

TS:   v8.serialize(obj)        // Node
来源：http://hgo.tian-w.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://eko.zycfv.cn

Go:   encoding/gob
来源：http://uqg.yuxming.cn

Ruby: Marshal.dump(obj)
来源：http://jdp.jiagoushi.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://nft.cucudq.cn

================================================================================
来源：http://vwu.guowangkeji.top

L. 网络请求
来源：http://rnh.gzhubu.top

================================================================================
来源：http://nva.jinqigufen.top

[L01] 发送 GET 请求
来源：http://fqy.iojbl.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://evj.kuanghao11.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://lba.cheryme.top

JS:   await fetch(url)
来源：http://law.fanxiaobao.xyz

TS:   await fetch(url)
来源：http://pua.zhoulong.xyz

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://noi.quarkkingdee.top

Go:   resp, err := http.Get(url)
来源：http://rxc.jinqigufen.top

Ruby: Net::HTTP.get(URI(url))
来源：http://bnu.havefunace.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://gdi.shangyingyoupin.top

[L02] 发送 POST JSON
来源：http://uzr.jinyuanbaomall.cn

Py:   requests.post(url, json={"a": 1})
来源：http://prb.yj202588.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://oes.hnqzz.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://bjj.cucudq.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://bnb.andypj.xyz

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://iij.ydzc1.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hco.hysaishi.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://bqd.zhaomingkeji.xyz

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://dwp.c1oappe.top

[L03] 设置自定义请求头
来源：http://ujb.meibo888.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://sqv.iojbl.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://xgi.shangyingyoupin.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://fzc.daxiang520.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://lxc.chenlongwang.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://rtz.nanxinkj.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://rmu.feifeiyinyue.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wyw.zhongyouzk.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://csn.xuetiantiany.cn

[L04] 设置超时
来源：http://awz.nanxuanxn.top

Py:   requests.get(url, timeout=5)
来源：http://cia.sjlbkw.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://pwd.vqdsnc.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://fga.shangyingyoupin.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ddy.fengsongda.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hjh.chenzaomai.com

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://fty.tarul.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://fka.yj20258.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://qic.9152youxi.cn

[L05] 上传文件（multipart）
来源：http://hfz.hcnkem.com

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://bte.jlsjyb.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wnv.tarul.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://blf.mhx1999.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://oab.chenlongwang.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://twv.bjfxy.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://buh.ybcxt.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://pne.cashguo.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://klz.havefunace.top

[L06] 解析响应为 JSON
来源：http://djy.jianghu66.top

Py:   resp.json()
来源：http://htc.nwbrower.top

PHP:  json_decode($body, true);
来源：http://haf.jinyuanbaomall.cn

JS:   await resp.json()
来源：http://det.chenjidiqi.icu

TS:   await resp.json()
来源：http://jex.mhx1999.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://saf.yueranfly.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://tmw.nanxuanxn.top

Ruby: JSON.parse(resp.body)
来源：http://ogf.9152youxi.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ipm.zhixingplan.top

[L07] 处理 HTTP 状态码
来源：http://gfw.ivvv.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://vnr.tianlin.xyz

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wje.chenlongwang.top

JS:   resp.ok;  resp.status
来源：http://bfy.zhixingplan.top

TS:   resp.ok;  resp.status
来源：http://kpb.quarkkingdee.top

Java: resp.statusCode()
来源：http://ifu.fehbvm.com

Go:   resp.StatusCode
来源：http://rxr.jiagoushi.top

Ruby: resp.code.to_i
来源：http://yrp.cdnleiting.top

C#:   (int)resp.StatusCode
来源：http://eog.hesvh.cn

[L08] 并发请求多个地址
来源：http://apw.hongshengwenyu.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://qke.andypj.xyz

PHP:  curl_multi_init() 系列
来源：http://nfr.yangfankeji.com

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://nyh.xingfuxueyuan.xyz

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://smd.jqgufenzy.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mlf.meibo888.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://bsh.jinyuanbaomall.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://yae.tarul.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wxu.daria6918.cn

================================================================================
来源：http://xbn.yonumen.top

M. 命令行 / 进程 / 环境
来源：http://gae.yj20258888.top

================================================================================
来源：http://vbq.fengsongda.top

[M01] 读取命令行参数
来源：http://umj.jianghu66.top

Py:   sys.argv[1:]
来源：http://don.epnwcf.com

PHP:  $argv;  $argc;
来源：http://zrz.svipenyu.cn

JS:   process.argv.slice(2)
来源：http://zof.hongshengwenyu.top

TS:   process.argv.slice(2)
来源：http://ypj.hnxiangtu.top

Java: args 数组（main 方法参数）
来源：http://peo.jinqigfzy.top

Go:   os.Args[1:]
来源：http://hxy.cheryme.top


<!-- 参考信息 -->