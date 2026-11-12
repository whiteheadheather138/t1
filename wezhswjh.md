代发 wailian999

================================================================================
来源：http://zaq.daxiang520.top

I. 正则表达式
来源：http://bfq.cucudq.cn

================================================================================
来源：http://vaz.yj202588.top

[I01] 判断是否匹配
来源：http://bbj.xziqi.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://tfk.bbcook.cn

PHP:  preg_match('/\d+/', $s);
来源：http://vqa.yj20258.top

JS:   /\d+/.test(s)
来源：http://kla.nanxinkj.top

TS:   /\d+/.test(s)
来源：http://ywx.hnqzz.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://wet.tianlin.xyz

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://adf.andypj.xyz

Ruby: s.match?(/\d+/)
来源：http://kpp.havefunace.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://lxn.jqgufenzy.top

[I02] 提取所有匹配
来源：http://prt.jinqigufen.top

Py:   re.findall(r"\d+", s)
来源：http://atm.sxryk.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hfs.xziqi.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://wlx.hfpthk.cn

TS:   s.match(/\d+/g)
来源：http://ofd.hesvh.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://cil.xuanzx.com

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://kaj.zdbjq.cn

Ruby: s.scan(/\d+/)
来源：http://mow.nanxinkj.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://tbp.gogol.net.cn

[I03] 提取捕获分组
来源：http://xge.sweek.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://zpq.0kj1m.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://etm.zhijiandao.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://qnn.vqdsnc.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://tdl.cheryme.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://nhf.ywan-chungtsiang.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://bgr.smart0.xyz

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://yiu.fzhhl.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://pej.aibaodan.cn

[I04] 正则替换
来源：http://osl.ywan-chungtsiang.top

Py:   re.sub(r"\d+", "#", s)
来源：http://hvt.xylfe.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ixt.tian-w.cn

JS:   s.replace(/\d+/g, "#")
来源：http://jof.zhongyouzk.top

TS:   s.replace(/\d+/g, "#")
来源：http://trb.sysykeji.top

Java: s.replaceAll("\\d+", "#")
来源：http://als.jqgfzy.top

Go:   re.ReplaceAllString(s, "#")
来源：http://zvm.xingfuxueyuan.xyz

Ruby: s.gsub(/\d+/, "#")
来源：http://qth.zdbjq.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://gob.gaohongyu789.top

[I05] 按正则拆分
来源：http://rka.vqdsnc.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://opi.tian-w.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://fml.yangfankeji.com

JS:   s.split(/\s*,\s*/)
来源：http://mdp.jinyuanbaomall.cn

TS:   s.split(/\s*,\s*/)
来源：http://jsf.cqqwz.cn

Java: s.split("\\s*,\\s*")
来源：http://iqt.ybcxt.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://lqm.fzhhl.top

Ruby: s.split(/\s*,\s*/)
来源：http://tno.xylfe.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://knf.epnwcf.com

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://vme.yangfankeji.com

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://cci.redwolf501.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://oyi.chenjidiqi.icu

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://rcs.snrcjt.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://zom.gzhubu.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://xiv.pycfn.com

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://mgf.chenlongwang.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://kex.jyoumei.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://tnk.xziqi.cn

[I07] 忽略大小写与多行模式
来源：http://jwa.guowangkeji.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://drh.yfazqb.com

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://wwg.jqgufenzy.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://vcm.gzhubu.top

TS:   /error/gim
来源：http://lnq.meibo888.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://nwe.gaohongyu789.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://bph.jinyuanbaomall.cn

Ruby: s.scan(/error/i)
来源：http://sgp.jqgfzy.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://mvr.zhaomingkeji.xyz

[I08] 贪婪与非贪婪匹配
来源：http://sso.shzxlz.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://wgh.jinghuilouyu.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://mzx.hysaishi.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://pqa.gogol.net.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://sew.ydjk.org.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://eup.aizwys.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://cat.cucudq.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://mps.jianghu66.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://nmh.zhengqikj.top

================================================================================
来源：http://lws.dashuyun.cn

J. 日期与时间
来源：http://eiq.hesvh.cn

================================================================================
来源：http://tcl.fzhhl.top

[J01] 获取当前时间
来源：http://mcc.ctjpmb.com

Py:   datetime.now();  datetime.now(UTC)
来源：http://ytq.birdmap.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://elo.tanke756.top

JS:   new Date();  Date.now()
来源：http://kiv.zhiwuduotai.top

TS:   new Date();  Date.now()
来源：http://fmx.cqqwz.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://par.sweek.top

Go:   time.Now()
来源：http://vgy.hammf.cn

Ruby: Time.now
来源：http://bmj.pengpengdd.cyou

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://cuy.chenzaomai.com

[J02] 格式化输出
来源：http://wyr.chenjidiqi.icu

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://zul.jqgufenzy.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://iqx.hcnkem.com

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://nhn.nanxinkj.top

TS:   d.toISOString()
来源：http://ifd.jqgfzy.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://kwf.smart0.xyz

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://pbg.tian-w.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mjj.daxiang520.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://lwf.xinyue.icu

[J03] 字符串解析为日期
来源：http://scu.chenzaomai.com

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://lbb.snrcjt.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://xot.9152youxi.cn

JS:   new Date("2024-01-02")
来源：http://lat.jinghuilouyu.cn

TS:   new Date("2024-01-02")
来源：http://mdt.c1oappe.top

Java: LocalDate.parse("2024-01-02")
来源：http://mkv.yueranfly.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://cgl.fehbvm.com

Ruby: Date.parse("2024-01-02")
来源：http://zws.tarul.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://pwx.52xcode.cn

[J04] 时间戳与日期互转
来源：http://ppr.hcnkem.com

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://pme.zhaomingkeji.xyz

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://dpr.yj20258.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hln.fanxiaobao.xyz

TS:   Math.floor(Date.now() / 1000)
来源：http://yvj.snrcjt.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ulz.shzxlz.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://lbz.shangyingyoupin.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://kgo.fzhhl.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://vzs.ybcxt.top

[J05] 时间加减（加 7 天）
来源：http://lrw.andypj.xyz

Py:   now + timedelta(days=7)
来源：http://xsp.jqgufenzy.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://hkg.daxiang520.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://bmr.meibo888.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://sgv.tian-w.cn

Java: LocalDate.now().plusDays(7)
来源：http://dvy.gotoacloud.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://gyk.snrcjt.cn

Ruby: Time.now + 7 * 86400
来源：http://cvz.bjfxy.top

C#:   DateTime.Now.AddDays(7)
来源：http://adg.cheryme.top

[J06] 计算两时间之差
来源：http://yqg.jinqigufen.top

Py:   (end - start).total_seconds()
来源：http://unx.ydjk.org.cn

PHP:  $end->diff($start)->days;
来源：http://obi.zhoulong.xyz

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://kok.yj20258.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://djz.cdnleiting.top

Java: Duration.between(start, end).toSeconds()
来源：http://mpk.yonumen.top

Go:   end.Sub(start).Hours()
来源：http://dbg.316326.xyz

Ruby: end - start                 # 返回秒数
来源：http://ekj.svipenyu.cn

C#:   (end - start).TotalSeconds
来源：http://ccj.yuanzhike.top

[J07] 比较两个日期
来源：http://qvs.xylfe.cn

Py:   d1 < d2;  d1 == d2
来源：http://meb.kuanghao11.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://sor.zdbjq.cn

JS:   d1.getTime() < d2.getTime()
来源：http://ken.aibaodan.cn

TS:   d1.getTime() < d2.getTime()
来源：http://sqy.nanxinkj.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://bow.yuxming.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://bwu.jqgfzy.top

Ruby: d1 < d2;  d1 == d2
来源：http://yob.shanyushiyangtech.top

C#:   d1 < d2;  d1 == d2
来源：http://aqq.xuanzx.com

[J08] 提取年月日与星期
来源：http://cvn.sjlbkw.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hfp.aibaodan.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://nwf.yangfankeji.com

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://was.ydzc1.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://huw.yvedp.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://emt.ywan-chungtsiang.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://psu.gzhubu.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://osu.vqdsnc.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://jrk.hammf.cn

[J09] 时区处理
来源：http://xsz.sjlbkw.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://wmw.bbcook.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://fwa.jlsjyb.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://uiw.shuidangran.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://gbd.ydjk.org.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://vpz.yj202588.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://dkx.ybcxt.top

Ruby: Time.now.getlocal("+08:00")
来源：http://zmw.xylfe.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://qmz.yonumen.top

[J10] 取今天 / 本月第一天
来源：http://oat.jinghuilouyu.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://avm.shanyushiyangkeji.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ozu.birdmap.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://oxg.cucudq.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://uey.meibo888.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://qjk.quarkkingdee.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://uou.yonumen.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://fos.smart0.xyz

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ink.jiagoushi.top

================================================================================
来源：http://myu.redwolf501.top

K. JSON 与序列化
来源：http://zav.daria6918.cn

================================================================================
来源：http://upw.jyoumei.cn

[K01] 对象转 JSON 字符串
来源：http://hyl.xylfe.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://kvg.tarul.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://odo.xuetiantiany.cn

JS:   JSON.stringify(obj)
来源：http://zvo.bbcook.cn

TS:   JSON.stringify(obj)
来源：http://lwi.gaohongyu789.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://dfd.sxryk.cn

Go:   json.Marshal(obj)
来源：http://ftb.nwbrower.top

Ruby: obj.to_json                                     // require "json"
来源：http://evu.shangyingyoupin.top

C#:   JsonSerializer.Serialize(obj)
来源：http://jtp.yuxming.cn

[K02] JSON 字符串转对象
来源：http://ntg.gogol.net.cn

Py:   json.loads(s)
来源：http://kal.jlsjyb.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://nxe.guowangkeji.top

JS:   JSON.parse(s)
来源：http://gxz.fzhhl.top

TS:   JSON.parse(s)
来源：http://okm.haohaochexian.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://tes.zhijiandao.cn

Go:   json.Unmarshal(data, &v)
来源：http://yzo.birdmap.top

Ruby: JSON.parse(s)
来源：http://lam.dashuyun.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://prp.sxryk.cn

[K03] JSON 美化输出（带缩进）
来源：http://zya.andypj.xyz

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://otu.bjfxy.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ziz.sweek.top

JS:   JSON.stringify(obj, null, 2)
来源：http://cqk.gogol.net.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://xpm.zdbjq.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://bpp.nanxinkj.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://kjm.yuxming.cn

Ruby: JSON.pretty_generate(obj)
来源：http://ibn.ywan-chungtsiang.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://iwk.hnxiangtu.top

[K04] 读取 JSON 文件
来源：http://qnf.daxiang520.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://rwx.chenzaomai.com

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://kbv.ydzc1.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://jsf.xziqi.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://swr.pycfn.com

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ynq.cashguo.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://zio.hongshengwenyu.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://njp.chenzaomai.com

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://jew.yongpay.top

[K05] 深拷贝对象
来源：http://jhl.c1oappe.top

Py:   copy.deepcopy(obj)
来源：http://cex.dashuyun.cn

PHP:  unserialize(serialize($obj));
来源：http://imh.fzhhl.top

JS:   structuredClone(obj)
来源：http://vcd.jinqigufen.top

TS:   structuredClone(obj)
来源：http://cvr.nanxinkj.top

Java: // 手写拷贝构造，或序列化往返
来源：http://ugc.jlsjyb.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://acc.quarkkingdee.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://iqc.jianghu66.top

C#:   // 序列化往返，或自定义 Clone
来源：http://oza.nwbrower.top

[K06] 解析 URL 查询串
来源：http://iyv.zhixingplan.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wbe.yj20258.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://gli.yuxming.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ahf.bbcook.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://klt.hywenlv.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://vhp.yuanzhike.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://sle.zhijiandao.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wlq.vehdjk.com

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://yey.ydjk.org.cn

[K07] 进制转换
来源：http://lbd.yj20258888.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://oxo.yonumen.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://nrr.chenzaomai.com

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://adh.yuanzhike.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://imh.birdmap.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hny.guannengcc.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://zjz.hfpthk.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ost.jyoumei.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ooq.yvedp.cn

[K08] 二进制序列化（非 JSON）
来源：http://jgs.fktsv.cn

Py:   pickle.dumps(obj)
来源：http://mzv.chenzaomai.com

PHP:  serialize($obj);  unserialize($s);
来源：http://mks.jinqigufen.top

JS:   v8.serialize(obj)        // Node
来源：http://lsh.yongpay.top

TS:   v8.serialize(obj)        // Node
来源：http://akq.pengpengdd.cyou

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hjg.fehbvm.com

Go:   encoding/gob
来源：http://idy.yj202588.top

Ruby: Marshal.dump(obj)
来源：http://ksz.pycfn.com

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mnk.ivvv.top

================================================================================
来源：http://ibu.yanxiufei.cn

L. 网络请求
来源：http://jra.sjlbkw.cn

================================================================================
来源：http://fpl.zhiwuduotai.top

[L01] 发送 GET 请求
来源：http://mue.chenzaomai.com

Py:   requests.get(url)                        # 第三方库 requests
来源：http://piy.bbcook.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ssi.yonumen.top

JS:   await fetch(url)
来源：http://emd.ehwqpu.com

TS:   await fetch(url)
来源：http://wog.cashguo.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://axf.jlsjyb.cn

Go:   resp, err := http.Get(url)
来源：http://tdd.gotoacloud.top

Ruby: Net::HTTP.get(URI(url))
来源：http://dmr.bbcook.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://koj.hammf.cn

[L02] 发送 POST JSON
来源：http://nmc.haohaochexian.top

Py:   requests.post(url, json={"a": 1})
来源：http://tjy.shzxlz.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://gea.hysaishi.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://snt.jinqigfzy.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://feu.shuidangran.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://tom.guowangkeji.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://jmv.mhx1999.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ryg.ybcxt.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://bfc.52xcode.cn

[L03] 设置自定义请求头
来源：http://tca.sweek.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ihq.ydjk.org.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://jvl.pengpengdd.cyou

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://atb.svipenyu.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://zew.ctjpmb.com

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://xjz.sweek.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ede.jinqigfzy.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://bsk.jiagoushi.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://rwb.vqdsnc.cn

[L04] 设置超时
来源：http://zon.gzhubu.top

Py:   requests.get(url, timeout=5)
来源：http://pwf.aibaodan.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ztd.jinghuilouyu.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://psd.gotoacloud.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://uma.jianghu66.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://xvq.smart0.xyz

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://zhi.kuanghao11.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hbq.mhx1999.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mzy.chenjidiqi.icu

[L05] 上传文件（multipart）
来源：http://ncb.guannengcc.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://uvx.shzxlz.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://dbo.zhoulong.xyz

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://sff.hnqzz.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://oxx.havefunace.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://jul.zhoulong.xyz

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://uzj.guannengcc.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://yuj.nanxuanxn.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://rtp.hcnkem.com

[L06] 解析响应为 JSON
来源：http://ovl.zhengqikj.top

Py:   resp.json()
来源：http://orv.yj20258888.top

PHP:  json_decode($body, true);
来源：http://npi.gzhubu.top

JS:   await resp.json()
来源：http://prc.yj202588.top

TS:   await resp.json()
来源：http://yiw.jiagoushi.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://nod.nanxinkj.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mvf.yanxiufei.cn

Ruby: JSON.parse(resp.body)
来源：http://nyz.epnwcf.com

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wzq.guowangkeji.top


<!-- 参考信息 -->