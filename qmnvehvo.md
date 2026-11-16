代发 wailian999

================================================================================
来源：http://bqg.yongpay.top

I. 正则表达式
来源：http://hgb.zhengqikj.top

================================================================================
来源：http://nwr.cashguo.top

[I01] 判断是否匹配
来源：http://bjr.ydzc1.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://rnz.9152youxi.cn

PHP:  preg_match('/\d+/', $s);
来源：http://jpb.zhoulong.xyz

JS:   /\d+/.test(s)
来源：http://kba.jiagoushi.top

TS:   /\d+/.test(s)
来源：http://jcs.hesvh.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ild.ydzc1.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hoo.hcnkem.com

Ruby: s.match?(/\d+/)
来源：http://jad.haohaochexian.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://kqq.hesvh.cn

[I02] 提取所有匹配
来源：http://wln.tian-w.cn

Py:   re.findall(r"\d+", s)
来源：http://pro.chenjidiqi.icu

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ilx.bbcook.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://uhn.mhx1999.top

TS:   s.match(/\d+/g)
来源：http://uqs.xziqi.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://slf.jianghu66.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://qnk.wangdashe.top

Ruby: s.scan(/\d+/)
来源：http://lax.cashguo.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://xri.shangyingyoupin.top

[I03] 提取捕获分组
来源：http://ulu.jinqigufen.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hpx.jiagoushi.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://raa.meibo888.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://pfg.uphjek.com

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ldl.yj20258.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hrz.zhengqikj.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://lyp.jinqigufen.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://msz.kuanghao11.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ypd.hnqzz.top

[I04] 正则替换
来源：http://exh.xuetiantiany.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://zvo.yueranfly.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://uqe.havefunace.top

JS:   s.replace(/\d+/g, "#")
来源：http://uip.jyoumei.cn

TS:   s.replace(/\d+/g, "#")
来源：http://ivn.yj20258888.top

Java: s.replaceAll("\\d+", "#")
来源：http://pav.hesvh.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://zpn.xylfe.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://rai.meibo888.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://nds.vehdjk.com

[I05] 按正则拆分
来源：http://dkl.ybcxt.top

Py:   re.split(r"\s*,\s*", s)
来源：http://xfk.guannengcc.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://kfu.jqgfzy.top

JS:   s.split(/\s*,\s*/)
来源：http://yyo.sjlbkw.cn

TS:   s.split(/\s*,\s*/)
来源：http://tzu.aizwys.cn

Java: s.split("\\s*,\\s*")
来源：http://jse.jqgfzy.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://qfa.havefunace.top

Ruby: s.split(/\s*,\s*/)
来源：http://moc.iojbl.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://mvm.sjlbkw.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://mdf.yuanzhike.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://yen.pycfn.com

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://eek.yanxiufei.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://cby.jinghuilouyu.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hhf.xinyue.icu

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://rwk.zhixingplan.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://qql.ctjpmb.com

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://jsv.sxryk.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ids.gzhubu.top

[I07] 忽略大小写与多行模式
来源：http://kmr.gaohongyu789.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ufs.xuanzx.com

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://vpm.fanxiaobao.xyz

JS:   /error/gim；new RegExp("error", "gim")
来源：http://tje.meibo888.top

TS:   /error/gim
来源：http://bzp.andypj.xyz

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://kxw.gaohongyu789.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://yex.meibo888.top

Ruby: s.scan(/error/i)
来源：http://bgj.xuetiantiany.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://dzm.jinyuanbaomall.cn

[I08] 贪婪与非贪婪匹配
来源：http://vhj.zhiwuduotai.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://rhb.snrcjt.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hur.zhijiandao.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://khb.jiagoushi.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://yqt.yangfankeji.com

Java: Pattern.compile("<b>.*?</b>")
来源：http://zue.hcnkem.com

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://pvy.yuanzhike.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ezy.gaohongyu789.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://xxu.uphjek.com

================================================================================
来源：http://bxq.ywan-chungtsiang.top

J. 日期与时间
来源：http://frt.feifeiyinyue.top

================================================================================
来源：http://nzl.vqdsnc.cn

[J01] 获取当前时间
来源：http://mvb.bjfxy.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://zms.zhongyouzk.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://eny.hnqzz.top

JS:   new Date();  Date.now()
来源：http://zmu.quarkkingdee.top

TS:   new Date();  Date.now()
来源：http://aed.meibo888.top

Java: LocalDateTime.now();  Instant.now()
来源：http://kvw.zhengqikj.top

Go:   time.Now()
来源：http://msu.guannengcc.top

Ruby: Time.now
来源：http://hji.jinyuanbaomall.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ibj.yangfankeji.com

[J02] 格式化输出
来源：http://bii.chenjidiqi.icu

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wvs.dashuyun.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://yyd.aizwys.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://cct.aibaodan.cn

TS:   d.toISOString()
来源：http://cst.bbcook.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://aal.gaohongyu789.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://yum.feifeiyinyue.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://eds.52xcode.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://vvp.xinyue.icu

[J03] 字符串解析为日期
来源：http://oot.chenzaomai.com

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://okp.zhiwuduotai.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://mwv.andypj.xyz

JS:   new Date("2024-01-02")
来源：http://pwg.aizwys.cn

TS:   new Date("2024-01-02")
来源：http://hin.yj202588.top

Java: LocalDate.parse("2024-01-02")
来源：http://ivm.yj20258.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://bca.gaohongyu789.top

Ruby: Date.parse("2024-01-02")
来源：http://iqi.svipenyu.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://unj.nwbrower.top

[J04] 时间戳与日期互转
来源：http://kwa.gogol.net.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://xdz.nanxuanxn.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://kua.cashguo.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://dfb.yj20258.top

TS:   Math.floor(Date.now() / 1000)
来源：http://omf.feifeiyinyue.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://xdm.chenjidiqi.icu

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://jqz.ivvv.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://qov.yvedp.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://qpz.jinyuanbaomall.cn

[J05] 时间加减（加 7 天）
来源：http://mwo.yongpay.top

Py:   now + timedelta(days=7)
来源：http://eik.zhongyouzk.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://epw.yuanzhike.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://qjd.pengpengdd.cyou

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://gws.zdbjq.cn

Java: LocalDate.now().plusDays(7)
来源：http://qzu.fzhhl.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://bef.cashguo.top

Ruby: Time.now + 7 * 86400
来源：http://zyu.uphjek.com

C#:   DateTime.Now.AddDays(7)
来源：http://hgi.hnqzz.top

[J06] 计算两时间之差
来源：http://afa.tian-w.cn

Py:   (end - start).total_seconds()
来源：http://nas.zhaomingkeji.xyz

PHP:  $end->diff($start)->days;
来源：http://gtm.ydzc1.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://pbt.xuanzx.com

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://mpp.cucudq.cn

Java: Duration.between(start, end).toSeconds()
来源：http://bwj.jqgufenzy.top

Go:   end.Sub(start).Hours()
来源：http://kql.haohaochexian.top

Ruby: end - start                 # 返回秒数
来源：http://rwg.hesvh.cn

C#:   (end - start).TotalSeconds
来源：http://lnd.guannengcc.top

[J07] 比较两个日期
来源：http://zac.zhengqikj.top

Py:   d1 < d2;  d1 == d2
来源：http://sxf.yuxming.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://xsq.haohaochexian.top

JS:   d1.getTime() < d2.getTime()
来源：http://jqo.tian-w.cn

TS:   d1.getTime() < d2.getTime()
来源：http://emr.cdnleiting.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://xdj.cashguo.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hxd.sysykeji.top

Ruby: d1 < d2;  d1 == d2
来源：http://qbf.jinghuilouyu.cn

C#:   d1 < d2;  d1 == d2
来源：http://ytv.xuetiantiany.cn

[J08] 提取年月日与星期
来源：http://vmu.cashguo.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://xnr.sxryk.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://omr.fanxiaobao.xyz

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://yui.zdqjudy.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://jnw.smart0.xyz

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://zwq.0kj1m.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://lls.ehwqpu.com

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://dob.bbcook.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://abj.epnwcf.com

[J09] 时区处理
来源：http://itv.zhijiandao.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://pwq.yongpay.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://oiq.yangfankeji.com

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ctg.hnqzz.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://dgc.vehdjk.com

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://bve.jlsjyb.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ulj.yonumen.top

Ruby: Time.now.getlocal("+08:00")
来源：http://qbc.yj20258888.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ntv.yj20258.top

[J10] 取今天 / 本月第一天
来源：http://csf.hammf.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://mmj.chenzaomai.com

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://fcs.hesvh.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://exl.zhijiandao.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://xry.pycfn.com

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://xmf.yanxiufei.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://dfd.zycfv.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://cjm.sjlbkw.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://vbf.jlsjyb.cn

================================================================================
来源：http://znw.daria6918.cn

K. JSON 与序列化
来源：http://udk.tarul.cn

================================================================================
来源：http://mqp.hywenlv.cn

[K01] 对象转 JSON 字符串
来源：http://vsy.jlsjyb.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ecz.birdmap.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://nrp.pycfn.com

JS:   JSON.stringify(obj)
来源：http://nmm.hcnkem.com

TS:   JSON.stringify(obj)
来源：http://akt.bjfxy.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://smt.jyoumei.cn

Go:   json.Marshal(obj)
来源：http://qjb.nwbrower.top

Ruby: obj.to_json                                     // require "json"
来源：http://fql.gotoacloud.top

C#:   JsonSerializer.Serialize(obj)
来源：http://dbl.dashuyun.cn

[K02] JSON 字符串转对象
来源：http://mlm.cdnleiting.top

Py:   json.loads(s)
来源：http://gde.hfpthk.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://raf.daxiang520.top

JS:   JSON.parse(s)
来源：http://jjr.xziqi.cn

TS:   JSON.parse(s)
来源：http://juf.hysaishi.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://nvd.xziqi.cn

Go:   json.Unmarshal(data, &v)
来源：http://msp.316326.xyz

Ruby: JSON.parse(s)
来源：http://zpi.yangfankeji.com

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://jhf.c1oappe.top

[K03] JSON 美化输出（带缩进）
来源：http://mlq.hongshengwenyu.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://pro.hysaishi.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://vyl.zhengqikj.top

JS:   JSON.stringify(obj, null, 2)
来源：http://mus.feifeiyinyue.top

TS:   JSON.stringify(obj, null, 2)
来源：http://qph.aizwys.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://mxy.xylfe.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://pzf.zdbjq.cn

Ruby: JSON.pretty_generate(obj)
来源：http://kyt.tanke756.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://yeu.c1oappe.top

[K04] 读取 JSON 文件
来源：http://pis.jyoumei.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://abg.daxiang520.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://naq.chenlongwang.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://zkv.shanyushiyangtech.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://jic.hammf.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ibk.pycfn.com

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://sau.nanxinkj.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://vkv.gogol.net.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://rih.gzhubu.top

[K05] 深拷贝对象
来源：http://sdx.hywenlv.cn

Py:   copy.deepcopy(obj)
来源：http://hgw.zhongyouzk.top

PHP:  unserialize(serialize($obj));
来源：http://gfk.hywenlv.cn

JS:   structuredClone(obj)
来源：http://fjb.pengpengdd.cyou

TS:   structuredClone(obj)
来源：http://djg.hnqzz.top

Java: // 手写拷贝构造，或序列化往返
来源：http://zvm.ydzc1.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://vjs.havefunace.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://drj.jlsjyb.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://blu.hnqzz.top

[K06] 解析 URL 查询串
来源：http://vwf.dashuyun.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://xek.yonumen.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://spr.yj20258.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ejh.ydzc1.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://epv.guowangkeji.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://itp.bjfxy.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://rfx.chenjidiqi.icu

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://snn.yj202588.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://gan.pengpengdd.cyou

[K07] 进制转换
来源：http://suz.andypj.xyz

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://pot.jiagoushi.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://zzo.jianghu66.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ciq.shzxlz.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ngb.gzhubu.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mtc.zhoulong.xyz

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://sqr.nanxuanxn.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://slh.andypj.xyz

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ibf.dianchejie.cn

[K08] 二进制序列化（非 JSON）
来源：http://qom.zhengqikj.top

Py:   pickle.dumps(obj)
来源：http://bej.yj20258888.top

PHP:  serialize($obj);  unserialize($s);
来源：http://hcu.kuanghao11.cn

JS:   v8.serialize(obj)        // Node
来源：http://hhz.dianchejie.cn

TS:   v8.serialize(obj)        // Node
来源：http://cab.jqgufenzy.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://pqu.guowangkeji.top

Go:   encoding/gob
来源：http://cbn.hongshengwenyu.top

Ruby: Marshal.dump(obj)
来源：http://qqd.pycfn.com

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hxb.hammf.cn

================================================================================
来源：http://roz.zhixingplan.top

L. 网络请求
来源：http://kgm.jinqigufen.top

================================================================================
来源：http://ebu.chenjidiqi.icu

[L01] 发送 GET 请求
来源：http://icp.52xcode.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://lrg.hesvh.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://giq.uphjek.com

JS:   await fetch(url)
来源：http://knf.yj20258888.top

TS:   await fetch(url)
来源：http://mkm.mhx1999.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://qap.dashuyun.cn

Go:   resp, err := http.Get(url)
来源：http://zsu.aizwys.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://eto.tarul.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://vec.vqdsnc.cn

[L02] 发送 POST JSON
来源：http://ocw.daria6918.cn

Py:   requests.post(url, json={"a": 1})
来源：http://gjg.gogol.net.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ejj.zhaomingkeji.xyz

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://swu.hysaishi.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://iin.chenlongwang.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://brh.bjfxy.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://llg.gogol.net.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://krp.nanxinkj.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://pnv.kuanghao11.cn

[L03] 设置自定义请求头
来源：http://wxc.ctjpmb.com

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://euy.cdnleiting.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://von.cashguo.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://cpv.uphjek.com

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://kno.andypj.xyz

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://dfq.jyoumei.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://qtr.jiagoushi.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://iul.zhixingplan.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://lay.sufxvd.cn

[L04] 设置超时
来源：http://xcl.hesvh.cn

Py:   requests.get(url, timeout=5)
来源：http://dvi.zhijiandao.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://zvu.ctjpmb.com

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://lce.smart0.xyz

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://nrr.guowangkeji.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wwc.ybcxt.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://dlf.chenzaomai.com

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ett.svipenyu.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://udv.jinqigfzy.top

[L05] 上传文件（multipart）
来源：http://kwc.ydjk.org.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://nbu.jinqigufen.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://rbf.ppjwa.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://qqn.tian-w.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://svi.feifeiyinyue.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://yka.jinqigufen.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://zjp.daria6918.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://bqh.hysaishi.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://oda.hammf.cn

[L06] 解析响应为 JSON
来源：http://flt.zhixingplan.top

Py:   resp.json()
来源：http://geh.ppjwa.cn

PHP:  json_decode($body, true);
来源：http://qnl.yonumen.top

JS:   await resp.json()
来源：http://tmu.dashuyun.cn

TS:   await resp.json()
来源：http://kyt.birdmap.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://dlr.iojbl.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://asx.nanxinkj.top

Ruby: JSON.parse(resp.body)
来源：http://wkb.smart0.xyz

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://rxr.yuxming.cn


<!-- 参考信息 -->