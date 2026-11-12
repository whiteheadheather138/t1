代发 wailian999

================================================================================
来源：http://zvu.cdnleiting.top

I. 正则表达式
来源：http://lko.hnxiangtu.top

================================================================================
来源：http://vuo.chenjidiqi.icu

[I01] 判断是否匹配
来源：http://ssn.pycfn.com

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://yca.birdmap.top

PHP:  preg_match('/\d+/', $s);
来源：http://qee.havefunace.top

JS:   /\d+/.test(s)
来源：http://dus.svipenyu.cn

TS:   /\d+/.test(s)
来源：http://hfq.jqgufenzy.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://zkr.ehwqpu.com

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://vmp.hammf.cn

Ruby: s.match?(/\d+/)
来源：http://dhp.yongpay.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://fln.daria6918.cn

[I02] 提取所有匹配
来源：http://gfb.wangshuangyany.cn

Py:   re.findall(r"\d+", s)
来源：http://sew.haohaochexian.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://bto.nwbrower.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://lda.sjlbkw.cn

TS:   s.match(/\d+/g)
来源：http://txy.zhijiandao.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://yzi.yuxming.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://tle.sweek.top

Ruby: s.scan(/\d+/)
来源：http://ozv.pengpengdd.cyou

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://swr.feifeiyinyue.top

[I03] 提取捕获分组
来源：http://lcq.aibaodan.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://jvy.ppjwa.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://qmr.0kj1m.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://lkd.316326.xyz

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://xbc.gogol.net.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://drt.yanxiufei.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://qap.feifeiyinyue.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://zbb.gogol.net.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ntf.yvedp.cn

[I04] 正则替换
来源：http://emb.cdnleiting.top

Py:   re.sub(r"\d+", "#", s)
来源：http://afr.xylfe.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://nss.havefunace.top

JS:   s.replace(/\d+/g, "#")
来源：http://kcl.tian-w.cn

TS:   s.replace(/\d+/g, "#")
来源：http://rhx.cashguo.top

Java: s.replaceAll("\\d+", "#")
来源：http://vwb.hywenlv.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://nti.yuanzhike.top

Ruby: s.gsub(/\d+/, "#")
来源：http://utg.cheryme.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://rpy.aizwys.cn

[I05] 按正则拆分
来源：http://jen.gaohongyu789.top

Py:   re.split(r"\s*,\s*", s)
来源：http://mnl.xingfuxueyuan.xyz

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://mmh.gogol.net.cn

JS:   s.split(/\s*,\s*/)
来源：http://qyy.aizwys.cn

TS:   s.split(/\s*,\s*/)
来源：http://qes.jianghu66.top

Java: s.split("\\s*,\\s*")
来源：http://hio.iojbl.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://sqt.gaohongyu789.top

Ruby: s.split(/\s*,\s*/)
来源：http://cnk.xingfuxueyuan.xyz

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://xnz.yfazqb.com

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hki.pengpengdd.cyou

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://qip.cheryme.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://qms.nanxinkj.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://nxi.jiagoushi.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://kjz.tianlin.xyz

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://pze.guannengcc.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://cxs.yuxming.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://lzu.cqqwz.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://gau.zhengqikj.top

[I07] 忽略大小写与多行模式
来源：http://bim.shanyushiyangtech.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://pko.vqdsnc.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hgd.fanxiaobao.xyz

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ico.jinqigufen.top

TS:   /error/gim
来源：http://nzw.tanke756.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://rvi.gzhubu.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://fbf.cqqwz.cn

Ruby: s.scan(/error/i)
来源：http://mlt.svipenyu.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://zub.zhaomingkeji.xyz

[I08] 贪婪与非贪婪匹配
来源：http://wym.sweek.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://jfz.hammf.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://knu.tanke756.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://phr.dashuyun.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ohh.hnqzz.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://nwc.nanxinkj.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://dbq.ehwqpu.com

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://wyn.shuidangran.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://qqz.fanxiaobao.xyz

================================================================================
来源：http://bcg.fengsongda.top

J. 日期与时间
来源：http://svu.yongpay.top

================================================================================
来源：http://afh.pengpengdd.cyou

[J01] 获取当前时间
来源：http://uud.vqdsnc.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://jhp.feifeiyinyue.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://luv.zhengqikj.top

JS:   new Date();  Date.now()
来源：http://bhx.316326.xyz

TS:   new Date();  Date.now()
来源：http://xfl.jinyuanbaomall.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://wym.yongpay.top

Go:   time.Now()
来源：http://jio.daria6918.cn

Ruby: Time.now
来源：http://uvv.birdmap.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://yud.vehdjk.com

[J02] 格式化输出
来源：http://hiv.fehbvm.com

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://irj.bbcook.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://kch.birdmap.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://pdw.bbcook.cn

TS:   d.toISOString()
来源：http://anc.jqgfzy.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://fam.316326.xyz

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://you.xuanzx.com

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://urm.ywan-chungtsiang.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://myt.zhengqikj.top

[J03] 字符串解析为日期
来源：http://jsg.daria6918.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://cpg.tian-w.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://plp.yj20258.top

JS:   new Date("2024-01-02")
来源：http://chb.xingfuxueyuan.xyz

TS:   new Date("2024-01-02")
来源：http://zwz.yonumen.top

Java: LocalDate.parse("2024-01-02")
来源：http://gfe.jianghu66.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://boq.wangshuangyany.cn

Ruby: Date.parse("2024-01-02")
来源：http://eos.gotoacloud.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://kmp.zhiwuduotai.top

[J04] 时间戳与日期互转
来源：http://kwk.jiagoushi.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://slu.zhoulong.xyz

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ity.jlsjyb.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ikk.nanxuanxn.top

TS:   Math.floor(Date.now() / 1000)
来源：http://gpa.0kj1m.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://azk.xinyue.icu

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://scf.hywenlv.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://emd.zhongyouzk.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://shk.svipenyu.cn

[J05] 时间加减（加 7 天）
来源：http://ter.fengsongda.top

Py:   now + timedelta(days=7)
来源：http://ymz.ppjwa.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://cgv.shanyushiyangkeji.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://tio.shuidangran.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://fpw.havefunace.top

Java: LocalDate.now().plusDays(7)
来源：http://qee.jinyuanbaomall.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ubc.hysaishi.cn

Ruby: Time.now + 7 * 86400
来源：http://cbi.bjfxy.top

C#:   DateTime.Now.AddDays(7)
来源：http://yfy.fzhhl.top

[J06] 计算两时间之差
来源：http://vhl.zhongyouzk.top

Py:   (end - start).total_seconds()
来源：http://hok.fanxiaobao.xyz

PHP:  $end->diff($start)->days;
来源：http://zst.fehbvm.com

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://kza.dashuyun.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://spr.sxryk.cn

Java: Duration.between(start, end).toSeconds()
来源：http://peu.hfpthk.cn

Go:   end.Sub(start).Hours()
来源：http://rcs.yuanzhike.top

Ruby: end - start                 # 返回秒数
来源：http://fbb.yuanzhike.top

C#:   (end - start).TotalSeconds
来源：http://hxa.xziqi.cn

[J07] 比较两个日期
来源：http://isx.pengpengdd.cyou

Py:   d1 < d2;  d1 == d2
来源：http://ies.ywan-chungtsiang.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ciy.chenlongwang.top

JS:   d1.getTime() < d2.getTime()
来源：http://tyc.xuetiantiany.cn

TS:   d1.getTime() < d2.getTime()
来源：http://zbe.svipenyu.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://rll.quarkkingdee.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://szh.ppjwa.cn

Ruby: d1 < d2;  d1 == d2
来源：http://kxu.ydzc1.top

C#:   d1 < d2;  d1 == d2
来源：http://skk.hfpthk.cn

[J08] 提取年月日与星期
来源：http://wrn.guannengcc.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://yvp.birdmap.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://stw.yongpay.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://wpo.hcnkem.com

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://fvq.chenjidiqi.icu

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://xsn.yongpay.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://qkd.chenjidiqi.icu

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://jli.gotoacloud.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://amg.zdbjq.cn

[J09] 时区处理
来源：http://ums.jyoumei.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://dsb.cqqwz.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://avn.guowangkeji.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://oqx.sweek.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://qhb.xingfuxueyuan.xyz

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://mcl.bbcook.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://auw.hammf.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://lhp.aizwys.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://vkk.sufxvd.cn

[J10] 取今天 / 本月第一天
来源：http://ljj.quarkkingdee.top

Py:   date.today();  date.today().replace(day=1)
来源：http://rnm.yangfankeji.com

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://gtr.fzhhl.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://lrk.cdnleiting.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://evm.jlsjyb.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://mrk.ydjk.org.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://lsj.pycfn.com

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://kdw.epnwcf.com

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ugo.yangfankeji.com

================================================================================
来源：http://khv.jinyuanbaomall.cn

K. JSON 与序列化
来源：http://hgl.smart0.xyz

================================================================================
来源：http://vpw.kuanghao11.cn

[K01] 对象转 JSON 字符串
来源：http://xec.andypj.xyz

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://yjh.quarkkingdee.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://jeb.sweek.top

JS:   JSON.stringify(obj)
来源：http://idj.cashguo.top

TS:   JSON.stringify(obj)
来源：http://owj.dashuyun.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://yhv.vqdsnc.cn

Go:   json.Marshal(obj)
来源：http://eou.ybcxt.top

Ruby: obj.to_json                                     // require "json"
来源：http://hin.yj20258.top

C#:   JsonSerializer.Serialize(obj)
来源：http://xxk.chenjidiqi.icu

[K02] JSON 字符串转对象
来源：http://cjr.9152youxi.cn

Py:   json.loads(s)
来源：http://yna.yuxming.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://jxi.yongpay.top

JS:   JSON.parse(s)
来源：http://xhh.yvedp.cn

TS:   JSON.parse(s)
来源：http://wel.cqqwz.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://zso.jinqigufen.top

Go:   json.Unmarshal(data, &v)
来源：http://ljv.fanxiaobao.xyz

Ruby: JSON.parse(s)
来源：http://ggx.sweek.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://wdf.jinghuilouyu.cn

[K03] JSON 美化输出（带缩进）
来源：http://bln.yj20258888.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://vrf.jinqigfzy.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://krj.hammf.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://htr.chenjidiqi.icu

TS:   JSON.stringify(obj, null, 2)
来源：http://tgk.kuanghao11.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://rsx.fengsongda.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://fqx.shanyushiyangkeji.top

Ruby: JSON.pretty_generate(obj)
来源：http://cln.mhx1999.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://kvx.jyoumei.cn

[K04] 读取 JSON 文件
来源：http://usu.bbcook.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://pml.tanke756.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://nks.sufxvd.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://vdq.shangyingyoupin.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ezd.vehdjk.com

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://uxc.bjfxy.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://gza.jinyuanbaomall.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://rez.chenlongwang.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://fvz.hfpthk.cn

[K05] 深拷贝对象
来源：http://tnt.bjfxy.top

Py:   copy.deepcopy(obj)
来源：http://oek.tanke756.top

PHP:  unserialize(serialize($obj));
来源：http://skn.quarkkingdee.top

JS:   structuredClone(obj)
来源：http://qzp.yongpay.top

TS:   structuredClone(obj)
来源：http://wgi.gaohongyu789.top

Java: // 手写拷贝构造，或序列化往返
来源：http://luf.quarkkingdee.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://zkn.gaohongyu789.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://tzj.andypj.xyz

C#:   // 序列化往返，或自定义 Clone
来源：http://lbp.0kj1m.cn

[K06] 解析 URL 查询串
来源：http://goy.cashguo.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://gam.yuxming.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://sfm.zdqjudy.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hdj.yanxiufei.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://scm.zhengqikj.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://yke.bjfxy.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://wfc.svipenyu.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://pya.zdbjq.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://xyx.kuanghao11.cn

[K07] 进制转换
来源：http://jve.smart0.xyz

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://gma.svipenyu.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ylr.zhixingplan.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://iwf.ehwqpu.com

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://coz.fengsongda.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://iof.yfazqb.com

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://cia.jqgufenzy.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://iql.quarkkingdee.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ffl.yuanzhike.top

[K08] 二进制序列化（非 JSON）
来源：http://wht.xylfe.cn

Py:   pickle.dumps(obj)
来源：http://ybq.quarkkingdee.top

PHP:  serialize($obj);  unserialize($s);
来源：http://vda.jianghu66.top

JS:   v8.serialize(obj)        // Node
来源：http://xnl.yonumen.top

TS:   v8.serialize(obj)        // Node
来源：http://mxt.quarkkingdee.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://uuz.iojbl.cn

Go:   encoding/gob
来源：http://xnm.zdqjudy.top

Ruby: Marshal.dump(obj)
来源：http://nex.cashguo.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ggb.gaohongyu789.top

================================================================================
来源：http://fcv.tanke756.top

L. 网络请求
来源：http://tvk.bjfxy.top

================================================================================
来源：http://sbj.tian-w.cn

[L01] 发送 GET 请求
来源：http://xub.wangdashe.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://xuj.ydzc1.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://nnp.wangshuangyany.cn

JS:   await fetch(url)
来源：http://sdu.fanxiaobao.xyz

TS:   await fetch(url)
来源：http://hsw.zdqjudy.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://xny.aizwys.cn

Go:   resp, err := http.Get(url)
来源：http://mnf.yueranfly.top

Ruby: Net::HTTP.get(URI(url))
来源：http://yvs.yuanzhike.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://fqx.c1oappe.top

[L02] 发送 POST JSON
来源：http://lhc.jyoumei.cn

Py:   requests.post(url, json={"a": 1})
来源：http://hth.jinghuilouyu.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://okr.xingfuxueyuan.xyz

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://gho.cqqwz.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ptf.chenjidiqi.icu

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://unp.ybcxt.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://pcc.fktsv.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://jnp.c1oappe.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://qsw.zycfv.cn

[L03] 设置自定义请求头
来源：http://cuv.zhijiandao.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://tpq.ydzc1.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://cvh.chenzaomai.com

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://rea.daxiang520.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://rri.jinqigufen.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wge.fanxiaobao.xyz

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://dll.wangdashe.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://uaz.chenzaomai.com

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://fwy.hnqzz.top

[L04] 设置超时
来源：http://iyf.tanke756.top

Py:   requests.get(url, timeout=5)
来源：http://zkp.jinqigufen.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://vdi.bjfxy.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://efi.tian-w.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://tfj.zdbjq.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://zsn.wangshuangyany.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://jmk.bbcook.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://tpd.dianchejie.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wgx.c1oappe.top

[L05] 上传文件（multipart）
来源：http://lcj.zdbjq.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ozd.shangyingyoupin.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://jht.chenzaomai.com

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://krc.zycfv.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://oly.shanyushiyangtech.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://sbi.wangdashe.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://vov.zdqjudy.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://akq.nanxuanxn.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://czz.cqqwz.cn

[L06] 解析响应为 JSON
来源：http://tdh.ydzc1.top

Py:   resp.json()
来源：http://hsd.jinqigfzy.top

PHP:  json_decode($body, true);
来源：http://ebn.epnwcf.com

JS:   await resp.json()
来源：http://jkj.epnwcf.com

TS:   await resp.json()
来源：http://wjb.fzhhl.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hzw.iojbl.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wdk.cheryme.top

Ruby: JSON.parse(resp.body)
来源：http://vmv.sysykeji.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://jht.c1oappe.top


<!-- 参考信息 -->