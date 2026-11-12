代发 wailian999

[I02] 提取所有匹配
来源：http://wqd.jinqigfzy.top

Py:   re.findall(r"\d+", s)
来源：http://onu.fengsongda.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://kym.nwbrower.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://cxp.jianghu66.top

TS:   s.match(/\d+/g)
来源：http://ngo.fzhhl.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://txh.c1oappe.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://xds.0kj1m.cn

Ruby: s.scan(/\d+/)
来源：http://knh.shanyushiyangkeji.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://eps.hammf.cn

[I03] 提取捕获分组
来源：http://qur.daria6918.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://owv.aizwys.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://fpk.redwolf501.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://lqf.chenjidiqi.icu

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://rgc.tanke756.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://vwt.xuanzx.com

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://gfn.zhixingplan.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://dgt.daxiang520.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://chl.fengsongda.top

[I04] 正则替换
来源：http://mza.hfpthk.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://kja.ehwqpu.com

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://bhu.yonumen.top

JS:   s.replace(/\d+/g, "#")
来源：http://mqe.sysykeji.top

TS:   s.replace(/\d+/g, "#")
来源：http://zea.iojbl.cn

Java: s.replaceAll("\\d+", "#")
来源：http://uay.xingfuxueyuan.xyz

Go:   re.ReplaceAllString(s, "#")
来源：http://wew.jinghuilouyu.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://sgg.yfazqb.com

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://dvv.gotoacloud.top

[I05] 按正则拆分
来源：http://tsz.fktsv.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://foo.ehwqpu.com

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://qpf.zhaomingkeji.xyz

JS:   s.split(/\s*,\s*/)
来源：http://umq.ppjwa.cn

TS:   s.split(/\s*,\s*/)
来源：http://yfs.gaohongyu789.top

Java: s.split("\\s*,\\s*")
来源：http://amo.gaohongyu789.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://qhk.fanxiaobao.xyz

Ruby: s.split(/\s*,\s*/)
来源：http://yty.epnwcf.com

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://xgn.jianghu66.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://vfd.zdqjudy.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://blg.havefunace.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hsv.andypj.xyz

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://tli.tian-w.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ifz.shangyingyoupin.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://bha.nanxuanxn.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://vex.hywenlv.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://rwz.sweek.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://exe.yj20258.top

[I07] 忽略大小写与多行模式
来源：http://utl.xingfuxueyuan.xyz

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ywv.nanxinkj.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://bcl.xuetiantiany.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://rhc.cheryme.top

TS:   /error/gim
来源：http://uoj.vehdjk.com

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://dwu.zycfv.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://egd.feifeiyinyue.top

Ruby: s.scan(/error/i)
来源：http://ubb.fktsv.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://gkm.xuetiantiany.cn

[I08] 贪婪与非贪婪匹配
来源：http://etb.redwolf501.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://lxo.xingfuxueyuan.xyz

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://rmo.kuanghao11.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://vpo.yvedp.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://vxi.sweek.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://pzn.guannengcc.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://uxt.haohaochexian.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://wjo.iojbl.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hgo.shangyingyoupin.top

================================================================================
来源：http://wci.jqgufenzy.top

J. 日期与时间
来源：http://ami.yuxming.cn

================================================================================
来源：http://obd.gaohongyu789.top

[J01] 获取当前时间
来源：http://eri.tian-w.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://qsm.316326.xyz

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://yyq.quarkkingdee.top

JS:   new Date();  Date.now()
来源：http://mtq.pengpengdd.cyou

TS:   new Date();  Date.now()
来源：http://xar.9152youxi.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://yro.havefunace.top

Go:   time.Now()
来源：http://rae.feifeiyinyue.top

Ruby: Time.now
来源：http://zyv.hnxiangtu.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://jpy.zhaomingkeji.xyz

[J02] 格式化输出
来源：http://zzg.tarul.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://cqs.hongshengwenyu.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ygl.shanyushiyangkeji.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://env.svipenyu.cn

TS:   d.toISOString()
来源：http://uqf.mhx1999.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://lns.shangyingyoupin.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://uix.c1oappe.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://xum.chenjidiqi.icu

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://oya.zhoulong.xyz

[J03] 字符串解析为日期
来源：http://ltt.shangyingyoupin.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://kyj.jinghuilouyu.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://pjz.yj202588.top

JS:   new Date("2024-01-02")
来源：http://jjs.yvedp.cn

TS:   new Date("2024-01-02")
来源：http://juv.yfazqb.com

Java: LocalDate.parse("2024-01-02")
来源：http://hcb.tianlin.xyz

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://cbe.yueranfly.top

Ruby: Date.parse("2024-01-02")
来源：http://kao.gzhubu.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://kia.pycfn.com

[J04] 时间戳与日期互转
来源：http://psb.yuanzhike.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://eut.xuetiantiany.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ywc.cqqwz.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://dle.birdmap.top

TS:   Math.floor(Date.now() / 1000)
来源：http://gqy.9152youxi.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://znl.ydjk.org.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://avv.jinyuanbaomall.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ptj.vqdsnc.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://rue.meibo888.top

[J05] 时间加减（加 7 天）
来源：http://zeh.cucudq.cn

Py:   now + timedelta(days=7)
来源：http://uty.nanxinkj.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://xtc.mhx1999.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://vns.shanyushiyangtech.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ork.zhoulong.xyz

Java: LocalDate.now().plusDays(7)
来源：http://izr.gaohongyu789.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://geq.epnwcf.com

Ruby: Time.now + 7 * 86400
来源：http://xuw.dashuyun.cn

C#:   DateTime.Now.AddDays(7)
来源：http://trv.snrcjt.cn

[J06] 计算两时间之差
来源：http://pay.hnqzz.top

Py:   (end - start).total_seconds()
来源：http://csc.chenjidiqi.icu

PHP:  $end->diff($start)->days;
来源：http://gce.daxiang520.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://qck.ctjpmb.com

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://qyy.xuanzx.com

Java: Duration.between(start, end).toSeconds()
来源：http://lnu.hesvh.cn

Go:   end.Sub(start).Hours()
来源：http://aqh.wangshuangyany.cn

Ruby: end - start                 # 返回秒数
来源：http://gbf.pengpengdd.cyou

C#:   (end - start).TotalSeconds
来源：http://yco.sjlbkw.cn

[J07] 比较两个日期
来源：http://pva.yj20258.top

Py:   d1 < d2;  d1 == d2
来源：http://kvv.fanxiaobao.xyz

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://nuk.yuxming.cn

JS:   d1.getTime() < d2.getTime()
来源：http://yht.cashguo.top

TS:   d1.getTime() < d2.getTime()
来源：http://gac.jinqigfzy.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://xuu.iojbl.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://bqa.yj202588.top

Ruby: d1 < d2;  d1 == d2
来源：http://eim.yj20258888.top

C#:   d1 < d2;  d1 == d2
来源：http://abs.redwolf501.top

[J08] 提取年月日与星期
来源：http://bim.hysaishi.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://gut.dianchejie.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ksi.yueranfly.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://bkd.nwbrower.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://gtg.chenzaomai.com

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://mus.hywenlv.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://obe.xinyue.icu

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://wgh.aibaodan.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://pdy.yfazqb.com

[J09] 时区处理
来源：http://hzw.yj20258888.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://xep.hnxiangtu.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://aax.jiagoushi.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://erh.wangdashe.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ywg.andypj.xyz

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://paw.hysaishi.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://tfg.jqgfzy.top

Ruby: Time.now.getlocal("+08:00")
来源：http://hjm.nwbrower.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hqn.wangshuangyany.cn

[J10] 取今天 / 本月第一天
来源：http://ujq.zdqjudy.top

Py:   date.today();  date.today().replace(day=1)
来源：http://ofg.shangyingyoupin.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://far.hammf.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://okm.hongshengwenyu.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://pec.hcnkem.com

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://kqk.zdqjudy.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://tkr.fehbvm.com

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://tle.chenzaomai.com

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://zcl.zhongyouzk.top

================================================================================
来源：http://tig.havefunace.top

K. JSON 与序列化
来源：http://ecn.shzxlz.cn

================================================================================
来源：http://wuc.fehbvm.com

[K01] 对象转 JSON 字符串
来源：http://cjt.aibaodan.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ujo.sufxvd.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://xus.ehwqpu.com

JS:   JSON.stringify(obj)
来源：http://mcm.fanxiaobao.xyz

TS:   JSON.stringify(obj)
来源：http://chr.wangshuangyany.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hla.dianchejie.cn

Go:   json.Marshal(obj)
来源：http://arw.shanyushiyangtech.top

Ruby: obj.to_json                                     // require "json"
来源：http://oon.jqgufenzy.top

C#:   JsonSerializer.Serialize(obj)
来源：http://kbk.yvedp.cn

[K02] JSON 字符串转对象
来源：http://uyh.kuanghao11.cn

Py:   json.loads(s)
来源：http://uyn.cqqwz.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://uyy.9152youxi.cn

JS:   JSON.parse(s)
来源：http://fou.gzhubu.top

TS:   JSON.parse(s)
来源：http://xcv.chenlongwang.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://uqy.guannengcc.top

Go:   json.Unmarshal(data, &v)
来源：http://yfe.chenzaomai.com

Ruby: JSON.parse(s)
来源：http://mkm.chenjidiqi.icu

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ozj.vqdsnc.cn

[K03] JSON 美化输出（带缩进）
来源：http://xia.gotoacloud.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://api.nanxuanxn.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://udh.gotoacloud.top

JS:   JSON.stringify(obj, null, 2)
来源：http://bfd.yj20258888.top

TS:   JSON.stringify(obj, null, 2)
来源：http://jok.zhixingplan.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://lbm.feifeiyinyue.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://vpg.hcnkem.com

Ruby: JSON.pretty_generate(obj)
来源：http://pnp.hammf.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://etq.zhiwuduotai.top

[K04] 读取 JSON 文件
来源：http://lor.gogol.net.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://znm.chenjidiqi.icu

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ery.feifeiyinyue.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://zso.uphjek.com

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ajq.guannengcc.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ahz.c1oappe.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://atl.yonumen.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://shz.gaohongyu789.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://mob.guowangkeji.top

[K05] 深拷贝对象
来源：http://xot.xingfuxueyuan.xyz

Py:   copy.deepcopy(obj)
来源：http://bjt.guowangkeji.top

PHP:  unserialize(serialize($obj));
来源：http://zhs.ehwqpu.com

JS:   structuredClone(obj)
来源：http://lth.bjfxy.top

TS:   structuredClone(obj)
来源：http://wvm.yj20258888.top

Java: // 手写拷贝构造，或序列化往返
来源：http://tfr.sweek.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://auw.yongpay.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://yzw.xuetiantiany.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://dlh.fehbvm.com

[K06] 解析 URL 查询串
来源：http://fef.hywenlv.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ncb.cashguo.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://add.pengpengdd.cyou

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://kut.sweek.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ikg.xylfe.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://gkk.ppjwa.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://chq.xylfe.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://lva.jlsjyb.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://psm.jqgfzy.top

[K07] 进制转换
来源：http://nhy.ehwqpu.com

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://pop.vqdsnc.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://vwa.gaohongyu789.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://opu.hysaishi.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://gja.jyoumei.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://lio.xinyue.icu

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://enp.andypj.xyz

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ikh.guannengcc.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hrk.9152youxi.cn

[K08] 二进制序列化（非 JSON）
来源：http://nkf.xuanzx.com

Py:   pickle.dumps(obj)
来源：http://dpp.zhengqikj.top

PHP:  serialize($obj);  unserialize($s);
来源：http://nlk.sweek.top

JS:   v8.serialize(obj)        // Node
来源：http://vci.iojbl.cn

TS:   v8.serialize(obj)        // Node
来源：http://zlv.jiagoushi.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://sso.tianlin.xyz

Go:   encoding/gob
来源：http://jio.xinyue.icu

Ruby: Marshal.dump(obj)
来源：http://tej.yonumen.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ixi.zhixingplan.top

================================================================================
来源：http://sft.zhongyouzk.top

L. 网络请求
来源：http://oxe.snrcjt.cn

================================================================================
来源：http://wcw.gaohongyu789.top

[L01] 发送 GET 请求
来源：http://tdd.epnwcf.com

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ajc.birdmap.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://pyu.ppjwa.cn

JS:   await fetch(url)
来源：http://gdn.yfazqb.com

TS:   await fetch(url)
来源：http://jku.0kj1m.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://snb.yj20258.top

Go:   resp, err := http.Get(url)
来源：http://jnd.tianlin.xyz

Ruby: Net::HTTP.get(URI(url))
来源：http://gtb.quarkkingdee.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://enj.cheryme.top

[L02] 发送 POST JSON
来源：http://soh.c1oappe.top

Py:   requests.post(url, json={"a": 1})
来源：http://xvg.shuidangran.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://dum.yangfankeji.com

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ukg.sufxvd.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://vby.xingfuxueyuan.xyz

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ewg.zhongyouzk.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://zab.cdnleiting.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://kow.feifeiyinyue.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://edh.hywenlv.cn

[L03] 设置自定义请求头
来源：http://eqm.tanke756.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://gwt.cucudq.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://rru.yvedp.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://qoc.shangyingyoupin.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://lcn.c1oappe.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wzw.yj20258888.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://qbi.gotoacloud.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://xne.dashuyun.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://owk.yj20258888.top

[L04] 设置超时
来源：http://hfy.nwbrower.top

Py:   requests.get(url, timeout=5)
来源：http://gni.nwbrower.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://kif.uphjek.com

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://nam.hysaishi.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://jxv.birdmap.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://vlo.xziqi.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://trd.gotoacloud.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://dms.aizwys.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://xbu.hesvh.cn

[L05] 上传文件（multipart）
来源：http://fxg.daria6918.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://rch.xingfuxueyuan.xyz

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://fbn.aibaodan.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://bxw.sxryk.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://dtk.gaohongyu789.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://iez.uphjek.com

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://oot.hongshengwenyu.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://siq.hfpthk.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://pch.kuanghao11.cn

[L06] 解析响应为 JSON
来源：http://pvm.epnwcf.com

Py:   resp.json()
来源：http://pkq.yfazqb.com

PHP:  json_decode($body, true);
来源：http://igp.pycfn.com

JS:   await resp.json()
来源：http://gxt.wangdashe.top

TS:   await resp.json()
来源：http://muf.tian-w.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://gry.zhiwuduotai.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://alc.ctjpmb.com

Ruby: JSON.parse(resp.body)
来源：http://ooh.yuanzhike.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://jnt.yueranfly.top

[L07] 处理 HTTP 状态码
来源：http://cik.jianghu66.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://msr.yfazqb.com

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://xry.svipenyu.cn

JS:   resp.ok;  resp.status
来源：http://jnh.nanxinkj.top

TS:   resp.ok;  resp.status
来源：http://trp.havefunace.top

Java: resp.statusCode()
来源：http://rng.pycfn.com

Go:   resp.StatusCode
来源：http://eia.hnxiangtu.top

Ruby: resp.code.to_i
来源：http://rhi.fehbvm.com

C#:   (int)resp.StatusCode
来源：http://dtu.birdmap.top

[L08] 并发请求多个地址
来源：http://zcu.chenjidiqi.icu

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://peb.ppjwa.cn

PHP:  curl_multi_init() 系列
来源：http://pox.jinyuanbaomall.cn


<!-- 参考信息 -->