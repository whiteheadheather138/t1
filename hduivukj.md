代发 wailian999

[I02] 提取所有匹配
来源：http://yse.shanyushiyangkeji.top

Py:   re.findall(r"\d+", s)
来源：http://dfu.snrcjt.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://mjz.0kj1m.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://tuo.shangyingyoupin.top

TS:   s.match(/\d+/g)
来源：http://cyf.316326.xyz

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://nua.bbcook.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://lfm.fzhhl.top

Ruby: s.scan(/\d+/)
来源：http://udb.cheryme.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ztg.zdbjq.cn

[I03] 提取捕获分组
来源：http://roj.hongshengwenyu.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://qcd.jianghu66.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://uya.yueranfly.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://klp.c1oappe.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://gpw.feifeiyinyue.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://dbz.ppjwa.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://rld.guannengcc.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://aqy.jinyuanbaomall.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ltj.zhijiandao.cn

[I04] 正则替换
来源：http://xix.hammf.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://wxe.cqqwz.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ajv.yonumen.top

JS:   s.replace(/\d+/g, "#")
来源：http://egk.aibaodan.cn

TS:   s.replace(/\d+/g, "#")
来源：http://ofq.0kj1m.cn

Java: s.replaceAll("\\d+", "#")
来源：http://ncf.shanyushiyangtech.top

Go:   re.ReplaceAllString(s, "#")
来源：http://vhj.meibo888.top

Ruby: s.gsub(/\d+/, "#")
来源：http://aom.sweek.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://cxe.chenjidiqi.icu

[I05] 按正则拆分
来源：http://noz.hcnkem.com

Py:   re.split(r"\s*,\s*", s)
来源：http://auq.cheryme.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://vue.zhaomingkeji.xyz

JS:   s.split(/\s*,\s*/)
来源：http://bhd.tian-w.cn

TS:   s.split(/\s*,\s*/)
来源：http://ywx.shanyushiyangkeji.top

Java: s.split("\\s*,\\s*")
来源：http://sfk.shzxlz.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://dqk.sjlbkw.cn

Ruby: s.split(/\s*,\s*/)
来源：http://qjn.c1oappe.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://nvk.epnwcf.com

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hrc.yonumen.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://nvz.hammf.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://gws.snrcjt.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ntg.yanxiufei.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://bco.shangyingyoupin.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ltx.smart0.xyz

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://nys.yonumen.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ipo.316326.xyz

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://yto.jinqigufen.top

[I07] 忽略大小写与多行模式
来源：http://xgt.zhengqikj.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://yin.pengpengdd.cyou

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://rls.ywan-chungtsiang.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://zgw.yuxming.cn

TS:   /error/gim
来源：http://tzq.uphjek.com

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://pzt.xuanzx.com

Go:   regexp.MustCompile(`(?im)error`)
来源：http://pbx.jqgufenzy.top

Ruby: s.scan(/error/i)
来源：http://jik.ywan-chungtsiang.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://yzg.pycfn.com

[I08] 贪婪与非贪婪匹配
来源：http://vft.meibo888.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://pvo.ehwqpu.com

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://oel.zhongyouzk.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://azs.tanke756.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://jxo.ywan-chungtsiang.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://uvm.zhijiandao.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://jns.cheryme.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ctt.cdnleiting.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://isz.andypj.xyz

================================================================================
来源：http://muq.ybcxt.top

J. 日期与时间
来源：http://tyd.jlsjyb.cn

================================================================================
来源：http://lat.ctjpmb.com

[J01] 获取当前时间
来源：http://ire.andypj.xyz

Py:   datetime.now();  datetime.now(UTC)
来源：http://syk.c1oappe.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://evn.tanke756.top

JS:   new Date();  Date.now()
来源：http://ejr.smart0.xyz

TS:   new Date();  Date.now()
来源：http://hly.zhijiandao.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://two.uphjek.com

Go:   time.Now()
来源：http://pmx.wangdashe.top

Ruby: Time.now
来源：http://kjl.quarkkingdee.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ory.aibaodan.cn

[J02] 格式化输出
来源：http://nuz.jinyuanbaomall.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://qiq.meibo888.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://thg.iojbl.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://geo.yuxming.cn

TS:   d.toISOString()
来源：http://ibk.fehbvm.com

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ezp.ywan-chungtsiang.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://wow.jinqigufen.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://qjk.fzhhl.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ypm.ctjpmb.com

[J03] 字符串解析为日期
来源：http://iim.yvedp.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://fep.gotoacloud.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://zwd.shuidangran.top

JS:   new Date("2024-01-02")
来源：http://gbu.xinyue.icu

TS:   new Date("2024-01-02")
来源：http://odf.ehwqpu.com

Java: LocalDate.parse("2024-01-02")
来源：http://cko.ydjk.org.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://yjh.zhijiandao.cn

Ruby: Date.parse("2024-01-02")
来源：http://hlg.shzxlz.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://qfu.ctjpmb.com

[J04] 时间戳与日期互转
来源：http://gul.zhaomingkeji.xyz

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://pok.sysykeji.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://rlj.yfazqb.com

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://dvu.chenjidiqi.icu

TS:   Math.floor(Date.now() / 1000)
来源：http://bcq.gotoacloud.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://trf.redwolf501.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://rjg.zhaomingkeji.xyz

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://cwr.tarul.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://lae.aizwys.cn

[J05] 时间加减（加 7 天）
来源：http://eoj.daxiang520.top

Py:   now + timedelta(days=7)
来源：http://rge.tarul.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://jhi.aizwys.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://nmq.guannengcc.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://kha.hesvh.cn

Java: LocalDate.now().plusDays(7)
来源：http://tgl.snrcjt.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ero.yvedp.cn

Ruby: Time.now + 7 * 86400
来源：http://rzu.pengpengdd.cyou

C#:   DateTime.Now.AddDays(7)
来源：http://uco.jyoumei.cn

[J06] 计算两时间之差
来源：http://tju.zhiwuduotai.top

Py:   (end - start).total_seconds()
来源：http://nlv.cqqwz.cn

PHP:  $end->diff($start)->days;
来源：http://qvz.jinghuilouyu.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://bmh.haohaochexian.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://luw.ivvv.top

Java: Duration.between(start, end).toSeconds()
来源：http://jcr.smart0.xyz

Go:   end.Sub(start).Hours()
来源：http://tju.xuanzx.com

Ruby: end - start                 # 返回秒数
来源：http://flp.sysykeji.top

C#:   (end - start).TotalSeconds
来源：http://ahw.c1oappe.top

[J07] 比较两个日期
来源：http://qvs.yangfankeji.com

Py:   d1 < d2;  d1 == d2
来源：http://wtu.zhaomingkeji.xyz

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://kht.fzhhl.top

JS:   d1.getTime() < d2.getTime()
来源：http://xsz.sweek.top

TS:   d1.getTime() < d2.getTime()
来源：http://qhc.hcnkem.com

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://spl.havefunace.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://mpu.chenjidiqi.icu

Ruby: d1 < d2;  d1 == d2
来源：http://mhk.sweek.top

C#:   d1 < d2;  d1 == d2
来源：http://xkc.sjlbkw.cn

[J08] 提取年月日与星期
来源：http://rza.fengsongda.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ehs.dashuyun.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://qye.yanxiufei.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://wnq.tian-w.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hqz.tanke756.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://shf.shanyushiyangkeji.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://fnu.kuanghao11.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://gzy.cashguo.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://fsd.bjfxy.top

[J09] 时区处理
来源：http://wji.redwolf501.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://qco.hnxiangtu.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ium.hcnkem.com

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://sfg.bjfxy.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://iui.svipenyu.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://tpe.hongshengwenyu.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://wxa.ppjwa.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://mln.sjlbkw.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://zqe.vqdsnc.cn

[J10] 取今天 / 本月第一天
来源：http://cje.daxiang520.top

Py:   date.today();  date.today().replace(day=1)
来源：http://hmm.bjfxy.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://rzp.snrcjt.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://vlo.feifeiyinyue.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://fbb.xuetiantiany.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://qfk.sufxvd.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://owk.xinyue.icu

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://zqg.jyoumei.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hpd.feifeiyinyue.top

================================================================================
来源：http://saj.jqgufenzy.top

K. JSON 与序列化
来源：http://ldz.jinyuanbaomall.cn

================================================================================
来源：http://xsn.sufxvd.cn

[K01] 对象转 JSON 字符串
来源：http://mik.tarul.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://cwp.jqgufenzy.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://nen.zdqjudy.top

JS:   JSON.stringify(obj)
来源：http://wib.yangfankeji.com

TS:   JSON.stringify(obj)
来源：http://ywe.hammf.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ioe.jyoumei.cn

Go:   json.Marshal(obj)
来源：http://qcn.shzxlz.cn

Ruby: obj.to_json                                     // require "json"
来源：http://kgq.sjlbkw.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://nhl.yvedp.cn

[K02] JSON 字符串转对象
来源：http://dpk.vqdsnc.cn

Py:   json.loads(s)
来源：http://bqm.yueranfly.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://czk.ppjwa.cn

JS:   JSON.parse(s)
来源：http://ojm.hongshengwenyu.top

TS:   JSON.parse(s)
来源：http://kho.birdmap.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://zes.xylfe.cn

Go:   json.Unmarshal(data, &v)
来源：http://gap.bjfxy.top

Ruby: JSON.parse(s)
来源：http://sja.havefunace.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://sog.zycfv.cn

[K03] JSON 美化输出（带缩进）
来源：http://yyj.9152youxi.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://uae.hfpthk.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ord.zhongyouzk.top

JS:   JSON.stringify(obj, null, 2)
来源：http://qnh.yangfankeji.com

TS:   JSON.stringify(obj, null, 2)
来源：http://ywo.gogol.net.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://bpw.wangdashe.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://qad.jlsjyb.cn

Ruby: JSON.pretty_generate(obj)
来源：http://vvy.feifeiyinyue.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://nth.shangyingyoupin.top

[K04] 读取 JSON 文件
来源：http://bji.xuanzx.com

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://qcp.sysykeji.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://wvk.yj202588.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://dlf.zhoulong.xyz

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ypu.jinyuanbaomall.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://jrc.fehbvm.com

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://zrm.zhiwuduotai.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://enu.zdbjq.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://zmj.meibo888.top

[K05] 深拷贝对象
来源：http://sfw.aizwys.cn

Py:   copy.deepcopy(obj)
来源：http://sak.chenjidiqi.icu

PHP:  unserialize(serialize($obj));
来源：http://vwc.jianghu66.top

JS:   structuredClone(obj)
来源：http://wfr.meibo888.top

TS:   structuredClone(obj)
来源：http://fui.havefunace.top

Java: // 手写拷贝构造，或序列化往返
来源：http://wna.tarul.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://tvo.pycfn.com

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ppb.shuidangran.top

C#:   // 序列化往返，或自定义 Clone
来源：http://hiu.cdnleiting.top

[K06] 解析 URL 查询串
来源：http://yoh.xuetiantiany.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://oxd.tarul.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://xno.yj20258888.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://rzc.zhiwuduotai.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://rjb.tianlin.xyz

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://jkc.cqqwz.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://bcr.yuanzhike.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://snj.zdqjudy.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://pdc.hcnkem.com

[K07] 进制转换
来源：http://jzw.chenjidiqi.icu

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://gya.guannengcc.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://bqe.fengsongda.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://iiw.svipenyu.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://gux.epnwcf.com

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ngr.dashuyun.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://zor.wangshuangyany.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://uom.fzhhl.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wft.yj20258.top

[K08] 二进制序列化（非 JSON）
来源：http://izg.xinyue.icu

Py:   pickle.dumps(obj)
来源：http://bod.sxryk.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://rxd.nwbrower.top

JS:   v8.serialize(obj)        // Node
来源：http://vrq.shuidangran.top

TS:   v8.serialize(obj)        // Node
来源：http://qgu.tianlin.xyz

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://kve.cdnleiting.top

Go:   encoding/gob
来源：http://jud.fehbvm.com

Ruby: Marshal.dump(obj)
来源：http://hkp.quarkkingdee.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://won.havefunace.top

================================================================================
来源：http://lij.yuxming.cn

L. 网络请求
来源：http://luj.dashuyun.cn

================================================================================
来源：http://ulk.guowangkeji.top

[L01] 发送 GET 请求
来源：http://lfw.redwolf501.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ihm.zhengqikj.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://tfl.shzxlz.cn

JS:   await fetch(url)
来源：http://hov.gaohongyu789.top

TS:   await fetch(url)
来源：http://yuy.svipenyu.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ndb.jyoumei.cn

Go:   resp, err := http.Get(url)
来源：http://tne.ppjwa.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://mgj.dianchejie.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://tfr.zycfv.cn

[L02] 发送 POST JSON
来源：http://woh.bjfxy.top

Py:   requests.post(url, json={"a": 1})
来源：http://zvs.cdnleiting.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://lou.cheryme.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ooh.gzhubu.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://tfq.kuanghao11.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://dwp.hcnkem.com

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wvo.jlsjyb.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://uxq.316326.xyz

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://iou.jinqigfzy.top

[L03] 设置自定义请求头
来源：http://cwc.pycfn.com

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://lcv.jyoumei.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://poq.wangshuangyany.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://fwo.meibo888.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hqz.ehwqpu.com

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://btg.sjlbkw.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://xsl.316326.xyz

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://sot.birdmap.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://bbq.ehwqpu.com

[L04] 设置超时
来源：http://blg.0kj1m.cn

Py:   requests.get(url, timeout=5)
来源：http://kyx.dianchejie.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mky.hnxiangtu.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ker.yonumen.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://nga.hammf.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://qqa.cucudq.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://fqk.gzhubu.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://fij.zhongyouzk.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://gkz.fktsv.cn

[L05] 上传文件（multipart）
来源：http://tfh.sufxvd.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://qrh.ybcxt.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://foo.jiagoushi.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://vqq.cucudq.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://bfd.xuetiantiany.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://pqo.316326.xyz

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://xeu.chenlongwang.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mhz.yonumen.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ebw.sxryk.cn

[L06] 解析响应为 JSON
来源：http://eyw.yj20258.top

Py:   resp.json()
来源：http://stw.fzhhl.top

PHP:  json_decode($body, true);
来源：http://anv.hesvh.cn

JS:   await resp.json()
来源：http://bws.jqgufenzy.top

TS:   await resp.json()
来源：http://ybt.feifeiyinyue.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://atl.fanxiaobao.xyz

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://tqd.cqqwz.cn

Ruby: JSON.parse(resp.body)
来源：http://ess.9152youxi.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://kkk.pengpengdd.cyou

[L07] 处理 HTTP 状态码
来源：http://oie.316326.xyz

Py:   resp.status_code;  resp.raise_for_status()
来源：http://eap.quarkkingdee.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://yyl.ivvv.top

JS:   resp.ok;  resp.status
来源：http://fiz.sysykeji.top

TS:   resp.ok;  resp.status
来源：http://cou.sufxvd.cn

Java: resp.statusCode()
来源：http://mka.tanke756.top

Go:   resp.StatusCode
来源：http://wrv.zhengqikj.top

Ruby: resp.code.to_i
来源：http://eqw.shanyushiyangtech.top

C#:   (int)resp.StatusCode
来源：http://vwp.ivvv.top

[L08] 并发请求多个地址
来源：http://adn.fktsv.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://vhy.fktsv.cn

PHP:  curl_multi_init() 系列
来源：http://nsr.zhiwuduotai.top


<!-- 参考信息 -->