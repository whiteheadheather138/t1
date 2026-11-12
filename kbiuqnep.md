代发 wailian999

================================================================================
来源：http://bov.kuanghao11.cn

I. 正则表达式
来源：http://ssa.guowangkeji.top

================================================================================
来源：http://eqq.jqgfzy.top

[I01] 判断是否匹配
来源：http://osf.fengsongda.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ylc.gogol.net.cn

PHP:  preg_match('/\d+/', $s);
来源：http://aii.cqqwz.cn

JS:   /\d+/.test(s)
来源：http://jwu.hnqzz.top

TS:   /\d+/.test(s)
来源：http://vmw.nwbrower.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://qar.yvedp.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://muo.tian-w.cn

Ruby: s.match?(/\d+/)
来源：http://cum.c1oappe.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://mws.meibo888.top

[I02] 提取所有匹配
来源：http://ydi.birdmap.top

Py:   re.findall(r"\d+", s)
来源：http://yvs.wangshuangyany.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ihh.fzhhl.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://fwu.aibaodan.cn

TS:   s.match(/\d+/g)
来源：http://rki.mhx1999.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://jqr.jqgufenzy.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://kcy.redwolf501.top

Ruby: s.scan(/\d+/)
来源：http://coz.cheryme.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ipj.xingfuxueyuan.xyz

[I03] 提取捕获分组
来源：http://qes.hysaishi.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://vxv.yj202588.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://wqf.cheryme.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://dut.epnwcf.com

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://yzc.daria6918.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://eak.yj20258.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://avn.hongshengwenyu.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ikp.bbcook.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://nda.iojbl.cn

[I04] 正则替换
来源：http://opx.zdbjq.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://fwa.yongpay.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://yfb.tarul.cn

JS:   s.replace(/\d+/g, "#")
来源：http://itl.zhixingplan.top

TS:   s.replace(/\d+/g, "#")
来源：http://wwe.ehwqpu.com

Java: s.replaceAll("\\d+", "#")
来源：http://ytv.cashguo.top

Go:   re.ReplaceAllString(s, "#")
来源：http://uwm.cucudq.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://jip.hywenlv.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://rld.shanyushiyangkeji.top

[I05] 按正则拆分
来源：http://rdm.jlsjyb.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://psj.jinqigfzy.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://zkg.shzxlz.cn

JS:   s.split(/\s*,\s*/)
来源：http://dlr.yongpay.top

TS:   s.split(/\s*,\s*/)
来源：http://iwx.316326.xyz

Java: s.split("\\s*,\\s*")
来源：http://rrb.cashguo.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://gfm.nanxinkj.top

Ruby: s.split(/\s*,\s*/)
来源：http://pnk.hongshengwenyu.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://orx.jinghuilouyu.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://trc.ppjwa.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://bya.chenjidiqi.icu

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://poe.hnqzz.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://sqa.xingfuxueyuan.xyz

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://axo.kuanghao11.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ull.jyoumei.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://oal.jinqigufen.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://zbz.shzxlz.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://vif.ybcxt.top

[I07] 忽略大小写与多行模式
来源：http://sxb.yuanzhike.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://cti.nwbrower.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ihj.xuetiantiany.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://zuj.cdnleiting.top

TS:   /error/gim
来源：http://zen.hcnkem.com

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://zbz.zhongyouzk.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://vkm.guowangkeji.top

Ruby: s.scan(/error/i)
来源：http://hac.guowangkeji.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://jyu.cheryme.top

[I08] 贪婪与非贪婪匹配
来源：http://gal.ybcxt.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://imy.nanxuanxn.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://lpq.dianchejie.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ien.ppjwa.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://fml.yj20258888.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://djp.andypj.xyz

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://rhp.sjlbkw.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://llh.svipenyu.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://tcy.feifeiyinyue.top

================================================================================
来源：http://siz.pengpengdd.cyou

J. 日期与时间
来源：http://dbj.chenjidiqi.icu

================================================================================
来源：http://fvm.sufxvd.cn

[J01] 获取当前时间
来源：http://frq.gogol.net.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://hbw.pengpengdd.cyou

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ehr.jqgufenzy.top

JS:   new Date();  Date.now()
来源：http://xkd.andypj.xyz

TS:   new Date();  Date.now()
来源：http://fbg.iojbl.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://djm.zhongyouzk.top

Go:   time.Now()
来源：http://qep.chenjidiqi.icu

Ruby: Time.now
来源：http://ziy.zhongyouzk.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://jle.cheryme.top

[J02] 格式化输出
来源：http://gel.hongshengwenyu.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://myf.jlsjyb.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://zkq.nanxinkj.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ere.cheryme.top

TS:   d.toISOString()
来源：http://uio.aibaodan.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://wva.ybcxt.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://lvn.quarkkingdee.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://isf.hfpthk.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://nvn.nwbrower.top

[J03] 字符串解析为日期
来源：http://lrs.hnqzz.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://nxs.ywan-chungtsiang.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://vrm.ivvv.top

JS:   new Date("2024-01-02")
来源：http://jbd.sxryk.cn

TS:   new Date("2024-01-02")
来源：http://vde.zycfv.cn

Java: LocalDate.parse("2024-01-02")
来源：http://pkq.jinqigufen.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://eny.yonumen.top

Ruby: Date.parse("2024-01-02")
来源：http://zql.yfazqb.com

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://yro.gaohongyu789.top

[J04] 时间戳与日期互转
来源：http://cym.zhoulong.xyz

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://aeo.wangdashe.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://tlc.ydzc1.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ikj.gaohongyu789.top

TS:   Math.floor(Date.now() / 1000)
来源：http://kpr.tianlin.xyz

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://awn.shangyingyoupin.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hlp.guowangkeji.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://wwv.zhixingplan.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://jzc.yongpay.top

[J05] 时间加减（加 7 天）
来源：http://ubd.xylfe.cn

Py:   now + timedelta(days=7)
来源：http://bbi.tarul.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://hoo.zhoulong.xyz

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://vzh.tianlin.xyz

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://fkl.smart0.xyz

Java: LocalDate.now().plusDays(7)
来源：http://uum.cucudq.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://wcs.zhengqikj.top

Ruby: Time.now + 7 * 86400
来源：http://gto.ppjwa.cn

C#:   DateTime.Now.AddDays(7)
来源：http://age.zhijiandao.cn

[J06] 计算两时间之差
来源：http://cwd.aizwys.cn

Py:   (end - start).total_seconds()
来源：http://zgq.zhaomingkeji.xyz

PHP:  $end->diff($start)->days;
来源：http://opv.nanxuanxn.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://nye.zhijiandao.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://nwq.fehbvm.com

Java: Duration.between(start, end).toSeconds()
来源：http://fyf.gotoacloud.top

Go:   end.Sub(start).Hours()
来源：http://ldj.shzxlz.cn

Ruby: end - start                 # 返回秒数
来源：http://buz.zdbjq.cn

C#:   (end - start).TotalSeconds
来源：http://lzy.shanyushiyangkeji.top

[J07] 比较两个日期
来源：http://xfl.zycfv.cn

Py:   d1 < d2;  d1 == d2
来源：http://uuj.cashguo.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://wcy.havefunace.top

JS:   d1.getTime() < d2.getTime()
来源：http://nfw.bjfxy.top

TS:   d1.getTime() < d2.getTime()
来源：http://szq.jinyuanbaomall.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://flo.zhengqikj.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://dhn.ehwqpu.com

Ruby: d1 < d2;  d1 == d2
来源：http://wqu.yuxming.cn

C#:   d1 < d2;  d1 == d2
来源：http://fuj.guannengcc.top

[J08] 提取年月日与星期
来源：http://bdk.hfpthk.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://gri.nanxinkj.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://jdp.daxiang520.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://zla.yueranfly.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://shi.ywan-chungtsiang.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://qzm.sweek.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://pqn.ybcxt.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://klc.cdnleiting.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://jtk.jlsjyb.cn

[J09] 时区处理
来源：http://qwm.quarkkingdee.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://bqu.fengsongda.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://wvb.ctjpmb.com

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://jnh.yj20258888.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://htt.hnqzz.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://jfh.ppjwa.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://wdz.cashguo.top

Ruby: Time.now.getlocal("+08:00")
来源：http://hgg.jinyuanbaomall.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://stm.jinghuilouyu.cn

[J10] 取今天 / 本月第一天
来源：http://lgk.sjlbkw.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://obb.yuxming.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://jqz.jlsjyb.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://puo.shuidangran.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://usr.yfazqb.com

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hhw.yuxming.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://mxs.pengpengdd.cyou

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://lpl.smart0.xyz

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://toj.yj20258.top

================================================================================
来源：http://isp.zhoulong.xyz

K. JSON 与序列化
来源：http://plr.ybcxt.top

================================================================================
来源：http://aat.gogol.net.cn

[K01] 对象转 JSON 字符串
来源：http://cgz.sjlbkw.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://xjs.shuidangran.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://kvq.ehwqpu.com

JS:   JSON.stringify(obj)
来源：http://qos.fzhhl.top

TS:   JSON.stringify(obj)
来源：http://wek.pycfn.com

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://vuw.sxryk.cn

Go:   json.Marshal(obj)
来源：http://sbh.yangfankeji.com

Ruby: obj.to_json                                     // require "json"
来源：http://tsv.chenjidiqi.icu

C#:   JsonSerializer.Serialize(obj)
来源：http://dte.feifeiyinyue.top

[K02] JSON 字符串转对象
来源：http://jkx.hongshengwenyu.top

Py:   json.loads(s)
来源：http://qac.xylfe.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://bct.9152youxi.cn

JS:   JSON.parse(s)
来源：http://cpr.sjlbkw.cn

TS:   JSON.parse(s)
来源：http://cga.guowangkeji.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://dea.bbcook.cn

Go:   json.Unmarshal(data, &v)
来源：http://dgd.gogol.net.cn

Ruby: JSON.parse(s)
来源：http://dcr.chenjidiqi.icu

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hwc.ywan-chungtsiang.top

[K03] JSON 美化输出（带缩进）
来源：http://ncv.xziqi.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://dmc.jinyuanbaomall.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://fcj.andypj.xyz

JS:   JSON.stringify(obj, null, 2)
来源：http://vzp.zhixingplan.top

TS:   JSON.stringify(obj, null, 2)
来源：http://mwh.sjlbkw.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://mak.hcnkem.com

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://zey.havefunace.top

Ruby: JSON.pretty_generate(obj)
来源：http://xuk.zdbjq.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://tyj.quarkkingdee.top

[K04] 读取 JSON 文件
来源：http://oij.jyoumei.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://cxg.sufxvd.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hdc.zhengqikj.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ejo.shzxlz.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ucs.jinyuanbaomall.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://oiz.hcnkem.com

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://rlt.ybcxt.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://aiz.daxiang520.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://moj.ydzc1.top

[K05] 深拷贝对象
来源：http://dnj.jinyuanbaomall.cn

Py:   copy.deepcopy(obj)
来源：http://grh.shangyingyoupin.top

PHP:  unserialize(serialize($obj));
来源：http://cue.zdbjq.cn

JS:   structuredClone(obj)
来源：http://lfm.hywenlv.cn

TS:   structuredClone(obj)
来源：http://mrd.0kj1m.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://yzf.yvedp.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://fnb.ydzc1.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://cmq.xingfuxueyuan.xyz

C#:   // 序列化往返，或自定义 Clone
来源：http://erg.chenzaomai.com

[K06] 解析 URL 查询串
来源：http://trp.pengpengdd.cyou

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://fzj.havefunace.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://vxz.wangshuangyany.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://aps.fehbvm.com

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://imt.sxryk.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://lvd.meibo888.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://ynl.zhiwuduotai.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hqv.bjfxy.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://xzb.jianghu66.top

[K07] 进制转换
来源：http://twl.sysykeji.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hlp.sxryk.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://nuz.cqqwz.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://rlg.jinqigfzy.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://alb.redwolf501.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://zep.fengsongda.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mxk.gaohongyu789.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://jks.cqqwz.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://qbx.c1oappe.top

[K08] 二进制序列化（非 JSON）
来源：http://odp.daria6918.cn

Py:   pickle.dumps(obj)
来源：http://nvf.bjfxy.top

PHP:  serialize($obj);  unserialize($s);
来源：http://zmo.yueranfly.top

JS:   v8.serialize(obj)        // Node
来源：http://ajj.tanke756.top

TS:   v8.serialize(obj)        // Node
来源：http://mkp.pengpengdd.cyou

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://gwc.iojbl.cn

Go:   encoding/gob
来源：http://owu.daxiang520.top

Ruby: Marshal.dump(obj)
来源：http://cvz.daxiang520.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://pab.yangfankeji.com

================================================================================
来源：http://mjx.nanxuanxn.top

L. 网络请求
来源：http://yky.xingfuxueyuan.xyz

================================================================================
来源：http://tcd.zhongyouzk.top

[L01] 发送 GET 请求
来源：http://cul.xuanzx.com

Py:   requests.get(url)                        # 第三方库 requests
来源：http://jgn.yangfankeji.com

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://nke.fehbvm.com

JS:   await fetch(url)
来源：http://att.yonumen.top

TS:   await fetch(url)
来源：http://qnz.xuanzx.com

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://jnh.hammf.cn

Go:   resp, err := http.Get(url)
来源：http://khx.yj20258.top

Ruby: Net::HTTP.get(URI(url))
来源：http://gtm.tarul.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://doy.andypj.xyz

[L02] 发送 POST JSON
来源：http://onh.sjlbkw.cn

Py:   requests.post(url, json={"a": 1})
来源：http://ank.zhengqikj.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://rgq.tanke756.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://zyq.cashguo.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://yex.cdnleiting.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://doe.xuetiantiany.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://twc.tarul.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://qoq.wangdashe.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://xvr.nanxuanxn.top

[L03] 设置自定义请求头
来源：http://kkj.yj20258888.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://csi.havefunace.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://drv.ydjk.org.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ung.chenlongwang.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://sbt.xuetiantiany.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://znu.aizwys.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://dxx.birdmap.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ecb.uphjek.com

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mwl.zhiwuduotai.top

[L04] 设置超时
来源：http://sjb.aizwys.cn

Py:   requests.get(url, timeout=5)
来源：http://kzb.ctjpmb.com

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://uml.tianlin.xyz

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://yjx.andypj.xyz

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://qec.shanyushiyangtech.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://stq.bjfxy.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://cwr.yvedp.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://pnd.gotoacloud.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://pon.zhoulong.xyz

[L05] 上传文件（multipart）
来源：http://jje.hfpthk.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://rzw.jinqigufen.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://csv.fengsongda.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ytv.dianchejie.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://lzk.yfazqb.com

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://xtx.haohaochexian.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://feb.redwolf501.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://pyt.shanyushiyangkeji.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ovz.yj20258888.top

[L06] 解析响应为 JSON
来源：http://vhn.hesvh.cn

Py:   resp.json()
来源：http://see.kuanghao11.cn

PHP:  json_decode($body, true);
来源：http://ath.ydzc1.top

JS:   await resp.json()
来源：http://uun.ivvv.top

TS:   await resp.json()
来源：http://qmh.zhixingplan.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://enf.gotoacloud.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://fxk.shanyushiyangtech.top

Ruby: JSON.parse(resp.body)
来源：http://asv.jqgfzy.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://npy.shzxlz.cn


<!-- 参考信息 -->