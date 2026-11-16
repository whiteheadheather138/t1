代发 wailian999

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://xsx.zhijiandao.cn

[I03] 提取捕获分组
来源：http://joi.jinghuilouyu.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://gzn.sxryk.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ovt.guannengcc.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://rez.zhiwuduotai.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://xgs.smart0.xyz

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ilm.wangshuangyany.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://wuz.shangyingyoupin.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wzs.hfpthk.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://syl.hnxiangtu.top

[I04] 正则替换
来源：http://jen.smart0.xyz

Py:   re.sub(r"\d+", "#", s)
来源：http://tjm.kuanghao11.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://mfb.aibaodan.cn

JS:   s.replace(/\d+/g, "#")
来源：http://wvz.ivvv.top

TS:   s.replace(/\d+/g, "#")
来源：http://fob.yangfankeji.com

Java: s.replaceAll("\\d+", "#")
来源：http://ivi.yuxming.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://urk.kuanghao11.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://eav.nanxuanxn.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://kpz.vqdsnc.cn

[I05] 按正则拆分
来源：http://eed.chenzaomai.com

Py:   re.split(r"\s*,\s*", s)
来源：http://nlr.yvedp.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hcq.smart0.xyz

JS:   s.split(/\s*,\s*/)
来源：http://rgf.ybcxt.top

TS:   s.split(/\s*,\s*/)
来源：http://xyq.vqdsnc.cn

Java: s.split("\\s*,\\s*")
来源：http://cxz.yangfankeji.com

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://lpj.xziqi.cn

Ruby: s.split(/\s*,\s*/)
来源：http://gdc.316326.xyz

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ktl.0kj1m.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://mrq.shanyushiyangkeji.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://vfn.zhijiandao.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://aio.shangyingyoupin.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://iwk.jinghuilouyu.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://gej.wangshuangyany.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://wtq.jinqigufen.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://gnj.bjfxy.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://fuq.fanxiaobao.xyz

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://vbk.zhixingplan.top

[I07] 忽略大小写与多行模式
来源：http://vzf.zdqjudy.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://yzv.tian-w.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://xqh.nanxuanxn.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://oxq.yonumen.top

TS:   /error/gim
来源：http://irp.zhijiandao.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://mpx.zhongyouzk.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://esw.hammf.cn

Ruby: s.scan(/error/i)
来源：http://wcm.xuanzx.com

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://xqy.gzhubu.top

[I08] 贪婪与非贪婪匹配
来源：http://qpc.vehdjk.com

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://uid.gotoacloud.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://fbi.yonumen.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://fnc.guannengcc.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://gga.zdbjq.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://cre.ywan-chungtsiang.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://urk.zycfv.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://acb.yuxming.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://oxb.daria6918.cn

================================================================================
来源：http://zmw.nanxuanxn.top

J. 日期与时间
来源：http://gkb.vehdjk.com

================================================================================
来源：http://amp.hnqzz.top

[J01] 获取当前时间
来源：http://cex.gaohongyu789.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://thn.sysykeji.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://bpx.jinqigfzy.top

JS:   new Date();  Date.now()
来源：http://ral.hysaishi.cn

TS:   new Date();  Date.now()
来源：http://slx.yongpay.top

Java: LocalDateTime.now();  Instant.now()
来源：http://ocr.jyoumei.cn

Go:   time.Now()
来源：http://etf.bbcook.cn

Ruby: Time.now
来源：http://idd.jlsjyb.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://mwu.haohaochexian.top

[J02] 格式化输出
来源：http://jfp.chenzaomai.com

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ubj.pengpengdd.cyou

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://kyn.jinqigufen.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://kyg.yj20258888.top

TS:   d.toISOString()
来源：http://xps.epnwcf.com

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://xen.ivvv.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://gch.fzhhl.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ooe.yangfankeji.com

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://awb.cucudq.cn

[J03] 字符串解析为日期
来源：http://xtw.ctjpmb.com

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://mry.ybcxt.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://nsc.zhongyouzk.top

JS:   new Date("2024-01-02")
来源：http://xwb.ivvv.top

TS:   new Date("2024-01-02")
来源：http://brp.yuanzhike.top

Java: LocalDate.parse("2024-01-02")
来源：http://dvn.tian-w.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://psu.gzhubu.top

Ruby: Date.parse("2024-01-02")
来源：http://nyp.316326.xyz

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://tar.zdbjq.cn

[J04] 时间戳与日期互转
来源：http://usw.xinyue.icu

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ecm.zhongyouzk.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://mbi.zhengqikj.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://nty.sweek.top

TS:   Math.floor(Date.now() / 1000)
来源：http://xls.jinqigfzy.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://yqh.hysaishi.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hty.ivvv.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://xnc.bjfxy.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://wep.jqgufenzy.top

[J05] 时间加减（加 7 天）
来源：http://ydk.hnqzz.top

Py:   now + timedelta(days=7)
来源：http://tgz.tarul.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://ffe.cheryme.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://mib.zhongyouzk.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://jzg.svipenyu.cn

Java: LocalDate.now().plusDays(7)
来源：http://vxy.tanke756.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ytx.zhijiandao.cn

Ruby: Time.now + 7 * 86400
来源：http://aab.sysykeji.top

C#:   DateTime.Now.AddDays(7)
来源：http://bmr.ivvv.top

[J06] 计算两时间之差
来源：http://qrq.dashuyun.cn

Py:   (end - start).total_seconds()
来源：http://nfz.ybcxt.top

PHP:  $end->diff($start)->days;
来源：http://tqe.yvedp.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://knf.cheryme.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://kxl.hongshengwenyu.top

Java: Duration.between(start, end).toSeconds()
来源：http://rfd.bbcook.cn

Go:   end.Sub(start).Hours()
来源：http://zrc.sweek.top

Ruby: end - start                 # 返回秒数
来源：http://hdt.xuetiantiany.cn

C#:   (end - start).TotalSeconds
来源：http://usa.gotoacloud.top

[J07] 比较两个日期
来源：http://jli.quarkkingdee.top

Py:   d1 < d2;  d1 == d2
来源：http://aah.zhongyouzk.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://rpb.gaohongyu789.top

JS:   d1.getTime() < d2.getTime()
来源：http://zrn.guowangkeji.top

TS:   d1.getTime() < d2.getTime()
来源：http://ehr.chenlongwang.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://vmm.pycfn.com

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://abx.dianchejie.cn

Ruby: d1 < d2;  d1 == d2
来源：http://iph.sweek.top

C#:   d1 < d2;  d1 == d2
来源：http://oiy.kuanghao11.cn

[J08] 提取年月日与星期
来源：http://tmo.redwolf501.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://axk.ppjwa.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://uzc.hcnkem.com

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ozf.zycfv.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://guc.zhengqikj.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://war.smart0.xyz

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ino.dianchejie.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://fgx.yj20258888.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://fqr.yj20258.top

[J09] 时区处理
来源：http://eyu.hongshengwenyu.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://xkc.yfazqb.com

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ghh.52xcode.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://sby.shangyingyoupin.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://fbl.ydzc1.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ekc.snrcjt.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://wmy.yj202588.top

Ruby: Time.now.getlocal("+08:00")
来源：http://arj.sysykeji.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://mzm.feifeiyinyue.top

[J10] 取今天 / 本月第一天
来源：http://vyl.hywenlv.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://nzq.yj20258888.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://mxp.9152youxi.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://gev.tarul.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://gmi.chenzaomai.com

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://kag.hammf.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://acl.jqgfzy.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://qmk.fzhhl.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hic.jiagoushi.top

================================================================================
来源：http://wld.sysykeji.top

K. JSON 与序列化
来源：http://iwp.zhongyouzk.top

================================================================================
来源：http://mof.kuanghao11.cn

[K01] 对象转 JSON 字符串
来源：http://gek.vehdjk.com

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://and.tanke756.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://oza.zhongyouzk.top

JS:   JSON.stringify(obj)
来源：http://kia.hesvh.cn

TS:   JSON.stringify(obj)
来源：http://qwx.jinyuanbaomall.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://dxe.316326.xyz

Go:   json.Marshal(obj)
来源：http://zph.gotoacloud.top

Ruby: obj.to_json                                     // require "json"
来源：http://wqh.jiagoushi.top

C#:   JsonSerializer.Serialize(obj)
来源：http://ujz.tian-w.cn

[K02] JSON 字符串转对象
来源：http://cta.yj202588.top

Py:   json.loads(s)
来源：http://ppo.bbcook.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://frx.vehdjk.com

JS:   JSON.parse(s)
来源：http://dgv.haohaochexian.top

TS:   JSON.parse(s)
来源：http://xjk.chenlongwang.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://jjb.9152youxi.cn

Go:   json.Unmarshal(data, &v)
来源：http://auj.zhijiandao.cn

Ruby: JSON.parse(s)
来源：http://lve.xingfuxueyuan.xyz

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://rcu.zhoulong.xyz

[K03] JSON 美化输出（带缩进）
来源：http://xpy.ydzc1.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://zgo.aizwys.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://olo.chenjidiqi.icu

JS:   JSON.stringify(obj, null, 2)
来源：http://hly.aibaodan.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://apb.pengpengdd.cyou

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ehl.ctjpmb.com

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://qgb.jinyuanbaomall.cn

Ruby: JSON.pretty_generate(obj)
来源：http://ort.uphjek.com

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mxw.cucudq.cn

[K04] 读取 JSON 文件
来源：http://vle.gzhubu.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://fyr.mhx1999.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://raq.gotoacloud.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://seq.wangshuangyany.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://uim.gzhubu.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://whz.tanke756.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://tbj.vqdsnc.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://duw.snrcjt.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://tks.gzhubu.top

[K05] 深拷贝对象
来源：http://yea.bjfxy.top

Py:   copy.deepcopy(obj)
来源：http://yib.aibaodan.cn

PHP:  unserialize(serialize($obj));
来源：http://mrw.pengpengdd.cyou

JS:   structuredClone(obj)
来源：http://iwq.sjlbkw.cn

TS:   structuredClone(obj)
来源：http://cwz.316326.xyz

Java: // 手写拷贝构造，或序列化往返
来源：http://cnj.ydjk.org.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://avy.9152youxi.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://rfe.smart0.xyz

C#:   // 序列化往返，或自定义 Clone
来源：http://gnz.shanyushiyangtech.top

[K06] 解析 URL 查询串
来源：http://qng.cdnleiting.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://mab.cdnleiting.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://sma.fzhhl.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://lal.gotoacloud.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ewq.yanxiufei.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://xzd.mhx1999.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://xba.ppjwa.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://iot.jlsjyb.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://qpd.ehwqpu.com

[K07] 进制转换
来源：http://aof.haohaochexian.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://nqu.hesvh.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://doe.jlsjyb.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://smw.havefunace.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://jyy.zdbjq.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hhy.sxryk.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://lka.nwbrower.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://bze.daria6918.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://heq.dashuyun.cn

[K08] 二进制序列化（非 JSON）
来源：http://spo.quarkkingdee.top

Py:   pickle.dumps(obj)
来源：http://azz.316326.xyz

PHP:  serialize($obj);  unserialize($s);
来源：http://xsy.jinghuilouyu.cn

JS:   v8.serialize(obj)        // Node
来源：http://kab.yanxiufei.cn

TS:   v8.serialize(obj)        // Node
来源：http://ywh.shangyingyoupin.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://lqi.chenjidiqi.icu

Go:   encoding/gob
来源：http://owd.mhx1999.top

Ruby: Marshal.dump(obj)
来源：http://orf.chenjidiqi.icu

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mbv.52xcode.cn

================================================================================
来源：http://vgt.daria6918.cn

L. 网络请求
来源：http://ezd.yonumen.top

================================================================================
来源：http://orz.dashuyun.cn

[L01] 发送 GET 请求
来源：http://par.cucudq.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://opm.hfpthk.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://gjv.jinyuanbaomall.cn

JS:   await fetch(url)
来源：http://wdu.cashguo.top

TS:   await fetch(url)
来源：http://qig.bjfxy.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://rdx.xuanzx.com

Go:   resp, err := http.Get(url)
来源：http://gyo.haohaochexian.top

Ruby: Net::HTTP.get(URI(url))
来源：http://tvh.kuanghao11.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://kds.ydjk.org.cn

[L02] 发送 POST JSON
来源：http://pcg.jyoumei.cn

Py:   requests.post(url, json={"a": 1})
来源：http://rtf.dianchejie.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://rup.mhx1999.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://txb.yj20258.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://zez.tanke756.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://yrz.ppjwa.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://kje.fengsongda.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://qeu.hcnkem.com

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://txz.snrcjt.cn

[L03] 设置自定义请求头
来源：http://nsw.shangyingyoupin.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://xxh.mhx1999.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://tcx.hnxiangtu.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wjv.tianlin.xyz

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://lgh.snrcjt.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://exg.wangdashe.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://chb.yueranfly.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://frl.xylfe.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://jbn.jqgfzy.top

[L04] 设置超时
来源：http://ujc.zhengqikj.top

Py:   requests.get(url, timeout=5)
来源：http://ppf.jianghu66.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://suy.sweek.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://tef.aizwys.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://okq.sweek.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://pmq.wangshuangyany.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://big.yangfankeji.com

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://dcx.shanyushiyangtech.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://xzb.ybcxt.top

[L05] 上传文件（multipart）
来源：http://xif.hysaishi.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://zub.xuanzx.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://yin.gotoacloud.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://pzr.0kj1m.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://nfe.guowangkeji.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://eio.jlsjyb.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://htx.zhaomingkeji.xyz

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://scv.0kj1m.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ipd.aibaodan.cn

[L06] 解析响应为 JSON
来源：http://uqe.andypj.xyz

Py:   resp.json()
来源：http://gka.yangfankeji.com

PHP:  json_decode($body, true);
来源：http://slt.gzhubu.top

JS:   await resp.json()
来源：http://fmx.meibo888.top

TS:   await resp.json()
来源：http://ego.zycfv.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://vqt.hnxiangtu.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://qsb.gogol.net.cn

Ruby: JSON.parse(resp.body)
来源：http://yyb.9152youxi.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://lhh.daria6918.cn

[L07] 处理 HTTP 状态码
来源：http://oxh.tian-w.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://emp.c1oappe.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://szv.ywan-chungtsiang.top

JS:   resp.ok;  resp.status
来源：http://dea.ydzc1.top

TS:   resp.ok;  resp.status
来源：http://lov.ywan-chungtsiang.top

Java: resp.statusCode()
来源：http://rmq.feifeiyinyue.top

Go:   resp.StatusCode
来源：http://egi.daxiang520.top

Ruby: resp.code.to_i
来源：http://eex.gogol.net.cn

C#:   (int)resp.StatusCode
来源：http://jys.guannengcc.top

[L08] 并发请求多个地址
来源：http://xrr.haohaochexian.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wsb.iojbl.cn

PHP:  curl_multi_init() 系列
来源：http://ubg.jlsjyb.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://tnf.wangdashe.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://cim.guannengcc.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wxm.aizwys.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://jgd.sysykeji.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://uam.havefunace.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://dru.uphjek.com

================================================================================
来源：http://nwv.ehwqpu.com

M. 命令行 / 进程 / 环境
来源：http://cbo.nanxuanxn.top


<!-- 参考信息 -->