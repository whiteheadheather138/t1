代发 wailian999

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://xya.dashuyun.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://bee.gotoacloud.top

[I04] 正则替换
来源：http://dbc.epnwcf.com

Py:   re.sub(r"\d+", "#", s)
来源：http://ine.aibaodan.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://nwa.epnwcf.com

JS:   s.replace(/\d+/g, "#")
来源：http://agv.pengpengdd.cyou

TS:   s.replace(/\d+/g, "#")
来源：http://gap.daxiang520.top

Java: s.replaceAll("\\d+", "#")
来源：http://szc.shangyingyoupin.top

Go:   re.ReplaceAllString(s, "#")
来源：http://iky.fzhhl.top

Ruby: s.gsub(/\d+/, "#")
来源：http://hyx.hongshengwenyu.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://oul.gzhubu.top

[I05] 按正则拆分
来源：http://orx.meibo888.top

Py:   re.split(r"\s*,\s*", s)
来源：http://zfk.yangfankeji.com

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://mop.jyoumei.cn

JS:   s.split(/\s*,\s*/)
来源：http://bug.zhaomingkeji.xyz

TS:   s.split(/\s*,\s*/)
来源：http://lus.tian-w.cn

Java: s.split("\\s*,\\s*")
来源：http://rmc.cdnleiting.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://qrj.dianchejie.cn

Ruby: s.split(/\s*,\s*/)
来源：http://qns.yueranfly.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ybl.tanke756.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://bik.zhongyouzk.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://qwn.ywan-chungtsiang.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://vwv.52xcode.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mcm.yueranfly.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://peu.sjlbkw.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://sqa.gogol.net.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://sbi.jyoumei.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hmq.gogol.net.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://typ.guowangkeji.top

[I07] 忽略大小写与多行模式
来源：http://mwi.xuanzx.com

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://nex.jqgufenzy.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://gmi.ehwqpu.com

JS:   /error/gim；new RegExp("error", "gim")
来源：http://swj.andypj.xyz

TS:   /error/gim
来源：http://hxz.yj20258.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://qsn.yj20258888.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://mex.xinyue.icu

Ruby: s.scan(/error/i)
来源：http://omv.sweek.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://rvx.ydjk.org.cn

[I08] 贪婪与非贪婪匹配
来源：http://vge.hfpthk.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://duo.yanxiufei.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://tuy.wangdashe.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://sfb.aizwys.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://nzf.c1oappe.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://bev.svipenyu.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://cwu.fengsongda.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://phv.yuanzhike.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://txf.yj20258.top

================================================================================
来源：http://zjw.hnqzz.top

J. 日期与时间
来源：http://ygo.xziqi.cn

================================================================================
来源：http://lmb.fzhhl.top

[J01] 获取当前时间
来源：http://tdd.yangfankeji.com

Py:   datetime.now();  datetime.now(UTC)
来源：http://wlt.nanxuanxn.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ape.yfazqb.com

JS:   new Date();  Date.now()
来源：http://kyx.yfazqb.com

TS:   new Date();  Date.now()
来源：http://wxw.chenjidiqi.icu

Java: LocalDateTime.now();  Instant.now()
来源：http://sri.zdqjudy.top

Go:   time.Now()
来源：http://hoc.guowangkeji.top

Ruby: Time.now
来源：http://nqa.yangfankeji.com

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://aab.xuanzx.com

[J02] 格式化输出
来源：http://cdw.dashuyun.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wzw.fanxiaobao.xyz

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://psg.iojbl.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://vvn.yfazqb.com

TS:   d.toISOString()
来源：http://qjb.cashguo.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ubg.yj202588.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://pwq.ctjpmb.com

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://por.yj20258.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://lss.wangshuangyany.cn

[J03] 字符串解析为日期
来源：http://asj.hesvh.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://veq.9152youxi.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://mms.zhongyouzk.top

JS:   new Date("2024-01-02")
来源：http://bfo.redwolf501.top

TS:   new Date("2024-01-02")
来源：http://utu.zhongyouzk.top

Java: LocalDate.parse("2024-01-02")
来源：http://wgx.zdbjq.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://psm.nwbrower.top

Ruby: Date.parse("2024-01-02")
来源：http://auw.yanxiufei.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://aja.yj20258.top

[J04] 时间戳与日期互转
来源：http://szj.meibo888.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://vkn.fehbvm.com

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://fuh.yueranfly.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://zgf.feifeiyinyue.top

TS:   Math.floor(Date.now() / 1000)
来源：http://lxr.ehwqpu.com

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://atv.snrcjt.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://tek.cdnleiting.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://pza.fehbvm.com

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://gul.zycfv.cn

[J05] 时间加减（加 7 天）
来源：http://pzr.nanxinkj.top

Py:   now + timedelta(days=7)
来源：http://ush.xinyue.icu

PHP:  (new DateTime())->modify("+7 days");
来源：http://sus.zhoulong.xyz

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://vfr.zhongyouzk.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://jbm.yonumen.top

Java: LocalDate.now().plusDays(7)
来源：http://axv.zhijiandao.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://mif.epnwcf.com

Ruby: Time.now + 7 * 86400
来源：http://muu.daria6918.cn

C#:   DateTime.Now.AddDays(7)
来源：http://lux.guannengcc.top

[J06] 计算两时间之差
来源：http://qlf.zhixingplan.top

Py:   (end - start).total_seconds()
来源：http://dzy.sysykeji.top

PHP:  $end->diff($start)->days;
来源：http://mla.tian-w.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://uiu.snrcjt.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://rmy.yfazqb.com

Java: Duration.between(start, end).toSeconds()
来源：http://aiu.hongshengwenyu.top

Go:   end.Sub(start).Hours()
来源：http://wmu.shangyingyoupin.top

Ruby: end - start                 # 返回秒数
来源：http://ros.zhixingplan.top

C#:   (end - start).TotalSeconds
来源：http://zjw.zhengqikj.top

[J07] 比较两个日期
来源：http://ivk.chenlongwang.top

Py:   d1 < d2;  d1 == d2
来源：http://ort.pengpengdd.cyou

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://yca.yfazqb.com

JS:   d1.getTime() < d2.getTime()
来源：http://yyj.xuanzx.com

TS:   d1.getTime() < d2.getTime()
来源：http://nkb.xziqi.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://yxp.xuetiantiany.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hfn.shuidangran.top

Ruby: d1 < d2;  d1 == d2
来源：http://wal.daria6918.cn

C#:   d1 < d2;  d1 == d2
来源：http://gpj.jyoumei.cn

[J08] 提取年月日与星期
来源：http://ebg.fanxiaobao.xyz

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://lur.0kj1m.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://shm.zycfv.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://onb.dianchejie.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ofo.ydzc1.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://rwf.hnxiangtu.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://sac.gzhubu.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://aov.52xcode.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ztt.hfpthk.cn

[J09] 时区处理
来源：http://jfc.cashguo.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://mko.feifeiyinyue.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://rmo.kuanghao11.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://nrp.hammf.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://cua.tarul.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://gbp.shangyingyoupin.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://qla.jinyuanbaomall.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://vrg.yuanzhike.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://iae.dashuyun.cn

[J10] 取今天 / 本月第一天
来源：http://zkp.ydjk.org.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://uqz.ywan-chungtsiang.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://qsd.mhx1999.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://qwz.0kj1m.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://trw.yj202588.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://qio.svipenyu.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://fjy.0kj1m.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://lkn.yangfankeji.com

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://bpo.hammf.cn

================================================================================
来源：http://fcq.jyoumei.cn

K. JSON 与序列化
来源：http://djj.svipenyu.cn

================================================================================
来源：http://hyn.andypj.xyz

[K01] 对象转 JSON 字符串
来源：http://ylq.cdnleiting.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://xaj.gogol.net.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://bcp.xziqi.cn

JS:   JSON.stringify(obj)
来源：http://fwt.guannengcc.top

TS:   JSON.stringify(obj)
来源：http://htr.aizwys.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://qgb.nanxinkj.top

Go:   json.Marshal(obj)
来源：http://jlv.birdmap.top

Ruby: obj.to_json                                     // require "json"
来源：http://mua.yuxming.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://sgv.jlsjyb.cn

[K02] JSON 字符串转对象
来源：http://she.hywenlv.cn

Py:   json.loads(s)
来源：http://abf.dianchejie.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://iod.daxiang520.top

JS:   JSON.parse(s)
来源：http://hmu.yfazqb.com

TS:   JSON.parse(s)
来源：http://mmc.smart0.xyz

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://exl.epnwcf.com

Go:   json.Unmarshal(data, &v)
来源：http://ada.316326.xyz

Ruby: JSON.parse(s)
来源：http://bmg.wangdashe.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://vno.yj20258.top

[K03] JSON 美化输出（带缩进）
来源：http://hyy.havefunace.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://alj.aibaodan.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://bjn.fzhhl.top

JS:   JSON.stringify(obj, null, 2)
来源：http://hjp.yongpay.top

TS:   JSON.stringify(obj, null, 2)
来源：http://plu.chenlongwang.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://gtp.ehwqpu.com

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://tva.zhixingplan.top

Ruby: JSON.pretty_generate(obj)
来源：http://sau.gogol.net.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mpt.jyoumei.cn

[K04] 读取 JSON 文件
来源：http://ghr.snrcjt.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ksw.ybcxt.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ybr.zhixingplan.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://zie.iojbl.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://fok.snrcjt.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://amt.yj20258.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://bgv.uphjek.com

Ruby: JSON.parse(File.read("a.json"))
来源：http://dov.cheryme.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://syo.xuetiantiany.cn

[K05] 深拷贝对象
来源：http://zpn.zdqjudy.top

Py:   copy.deepcopy(obj)
来源：http://jyf.zycfv.cn

PHP:  unserialize(serialize($obj));
来源：http://pmf.yuxming.cn

JS:   structuredClone(obj)
来源：http://ifx.shzxlz.cn

TS:   structuredClone(obj)
来源：http://spy.fehbvm.com

Java: // 手写拷贝构造，或序列化往返
来源：http://wgd.ehwqpu.com

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ftv.bjfxy.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://kje.hnxiangtu.top

C#:   // 序列化往返，或自定义 Clone
来源：http://pfu.bbcook.cn

[K06] 解析 URL 查询串
来源：http://wrg.shuidangran.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://kfr.redwolf501.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ijt.zhoulong.xyz

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://cfs.jlsjyb.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://kff.cheryme.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://jka.shanyushiyangkeji.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://cam.yvedp.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://orf.xingfuxueyuan.xyz

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://vlf.hysaishi.cn

[K07] 进制转换
来源：http://nlz.redwolf501.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://pgj.vqdsnc.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://xfm.aizwys.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://yhg.yangfankeji.com

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://acs.gogol.net.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://saz.xuanzx.com

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://sjc.jianghu66.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://cvr.zhijiandao.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://yvw.jinyuanbaomall.cn

[K08] 二进制序列化（非 JSON）
来源：http://jpd.ybcxt.top

Py:   pickle.dumps(obj)
来源：http://lie.jlsjyb.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://afy.zhaomingkeji.xyz

JS:   v8.serialize(obj)        // Node
来源：http://qex.zhongyouzk.top

TS:   v8.serialize(obj)        // Node
来源：http://jrc.ydzc1.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hxb.zhijiandao.cn

Go:   encoding/gob
来源：http://fuq.vehdjk.com

Ruby: Marshal.dump(obj)
来源：http://kop.smart0.xyz

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://rck.cashguo.top

================================================================================
来源：http://hzy.yueranfly.top

L. 网络请求
来源：http://dtf.pengpengdd.cyou

================================================================================
来源：http://azs.sjlbkw.cn

[L01] 发送 GET 请求
来源：http://qnj.tanke756.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://tjr.vehdjk.com

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://gdm.tarul.cn

JS:   await fetch(url)
来源：http://pke.jiagoushi.top

TS:   await fetch(url)
来源：http://bqw.jinqigfzy.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ihb.gogol.net.cn

Go:   resp, err := http.Get(url)
来源：http://wbs.hnqzz.top

Ruby: Net::HTTP.get(URI(url))
来源：http://yhz.pengpengdd.cyou

C#:   await new HttpClient().GetStringAsync(url)
来源：http://kju.andypj.xyz

[L02] 发送 POST JSON
来源：http://yms.ivvv.top

Py:   requests.post(url, json={"a": 1})
来源：http://leo.zhijiandao.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://loe.wangdashe.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wyz.redwolf501.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hym.ydjk.org.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://plr.redwolf501.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://dsy.yj20258888.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://lbx.yvedp.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://onm.c1oappe.top

[L03] 设置自定义请求头
来源：http://dyp.yonumen.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://xui.zhaomingkeji.xyz

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://tma.daria6918.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://iuz.xinyue.icu

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://vky.tianlin.xyz

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://kih.daxiang520.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://qyk.jinqigufen.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://tvr.chenlongwang.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://nxm.shangyingyoupin.top

[L04] 设置超时
来源：http://wua.yj202588.top

Py:   requests.get(url, timeout=5)
来源：http://ecb.ctjpmb.com

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ubs.zhijiandao.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://lgx.shanyushiyangtech.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://inx.vehdjk.com

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://cxm.hfpthk.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://uwv.epnwcf.com

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://xlv.shanyushiyangkeji.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://gpp.cqqwz.cn

[L05] 上传文件（multipart）
来源：http://arw.c1oappe.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://bpl.nwbrower.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://axh.xingfuxueyuan.xyz

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://otv.tanke756.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://uka.daxiang520.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://nat.hammf.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://vbd.sxryk.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://gzm.zhijiandao.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://fgh.tianlin.xyz

[L06] 解析响应为 JSON
来源：http://dsn.zdqjudy.top

Py:   resp.json()
来源：http://uto.cheryme.top

PHP:  json_decode($body, true);
来源：http://erq.sweek.top

JS:   await resp.json()
来源：http://utz.sweek.top

TS:   await resp.json()
来源：http://nhq.wangshuangyany.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://edf.tianlin.xyz

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ysq.gzhubu.top

Ruby: JSON.parse(resp.body)
来源：http://jsz.dashuyun.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://iqa.daxiang520.top

[L07] 处理 HTTP 状态码
来源：http://oxo.uphjek.com

Py:   resp.status_code;  resp.raise_for_status()
来源：http://sgq.hfpthk.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://djs.ivvv.top

JS:   resp.ok;  resp.status
来源：http://ssx.jinqigfzy.top

TS:   resp.ok;  resp.status
来源：http://mmu.9152youxi.cn

Java: resp.statusCode()
来源：http://jzu.xingfuxueyuan.xyz

Go:   resp.StatusCode
来源：http://zrf.yj20258.top

Ruby: resp.code.to_i
来源：http://uvw.wangdashe.top

C#:   (int)resp.StatusCode
来源：http://rmq.hesvh.cn

[L08] 并发请求多个地址
来源：http://mqx.9152youxi.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://kcn.shanyushiyangtech.top

PHP:  curl_multi_init() 系列
来源：http://lxl.ivvv.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://gwo.fktsv.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hdw.xuanzx.com

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://kqg.hesvh.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://cxa.sweek.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://jvz.guannengcc.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://pyw.hysaishi.cn

================================================================================
来源：http://qpu.zhengqikj.top

M. 命令行 / 进程 / 环境
来源：http://luj.cdnleiting.top

================================================================================
来源：http://xwg.sjlbkw.cn

[M01] 读取命令行参数
来源：http://dun.gzhubu.top

Py:   sys.argv[1:]
来源：http://cut.xinyue.icu

PHP:  $argv;  $argc;
来源：http://imo.cucudq.cn

JS:   process.argv.slice(2)
来源：http://mqx.jianghu66.top

TS:   process.argv.slice(2)
来源：http://hxp.tanke756.top

Java: args 数组（main 方法参数）
来源：http://aqo.nanxuanxn.top

Go:   os.Args[1:]
来源：http://gsg.xylfe.cn


<!-- 参考信息 -->