代发 wailian999

================================================================================
来源：http://cjr.tanke756.top

I. 正则表达式
来源：http://ksr.yj20258888.top

================================================================================
来源：http://thv.zhixingplan.top

[I01] 判断是否匹配
来源：http://qsr.zhoulong.xyz

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://nra.pycfn.com

PHP:  preg_match('/\d+/', $s);
来源：http://oyo.bjfxy.top

JS:   /\d+/.test(s)
来源：http://fey.xingfuxueyuan.xyz

TS:   /\d+/.test(s)
来源：http://mkq.xylfe.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://udt.gotoacloud.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://sly.xingfuxueyuan.xyz

Ruby: s.match?(/\d+/)
来源：http://yzm.hfpthk.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://kvc.yuxming.cn

[I02] 提取所有匹配
来源：http://gfi.dashuyun.cn

Py:   re.findall(r"\d+", s)
来源：http://qdw.daxiang520.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hgu.nanxuanxn.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://wsf.shanyushiyangkeji.top

TS:   s.match(/\d+/g)
来源：http://pda.vehdjk.com

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://lmi.jiagoushi.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ywx.bbcook.cn

Ruby: s.scan(/\d+/)
来源：http://lez.dashuyun.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://csj.birdmap.top

[I03] 提取捕获分组
来源：http://wtb.gaohongyu789.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://kmx.jqgufenzy.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://gmd.wangshuangyany.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://xyd.zhengqikj.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wsr.gogol.net.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://klm.hysaishi.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://mii.ivvv.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wwj.ywan-chungtsiang.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://crp.hnqzz.top

[I04] 正则替换
来源：http://tnl.nanxuanxn.top

Py:   re.sub(r"\d+", "#", s)
来源：http://lpb.gaohongyu789.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://xcu.wangshuangyany.cn

JS:   s.replace(/\d+/g, "#")
来源：http://ypz.gzhubu.top

TS:   s.replace(/\d+/g, "#")
来源：http://dfq.sweek.top

Java: s.replaceAll("\\d+", "#")
来源：http://pnu.chenlongwang.top

Go:   re.ReplaceAllString(s, "#")
来源：http://bwj.dianchejie.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://fch.zhixingplan.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://lyn.wangshuangyany.cn

[I05] 按正则拆分
来源：http://sec.nanxuanxn.top

Py:   re.split(r"\s*,\s*", s)
来源：http://ucs.nwbrower.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://yln.xinyue.icu

JS:   s.split(/\s*,\s*/)
来源：http://ltn.yangfankeji.com

TS:   s.split(/\s*,\s*/)
来源：http://yvr.daria6918.cn

Java: s.split("\\s*,\\s*")
来源：http://mco.jqgfzy.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://znr.svipenyu.cn

Ruby: s.split(/\s*,\s*/)
来源：http://hvz.sweek.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://piy.daxiang520.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://uny.zdbjq.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://heq.jqgfzy.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ohx.iojbl.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://kod.zhongyouzk.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://kjp.yj20258888.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ygh.hywenlv.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://lov.hammf.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://rca.cucudq.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://qmo.zhengqikj.top

[I07] 忽略大小写与多行模式
来源：http://ocl.sweek.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://zkn.hongshengwenyu.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://yew.snrcjt.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://qlr.cucudq.cn

TS:   /error/gim
来源：http://ldk.wangdashe.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://fqu.ehwqpu.com

Go:   regexp.MustCompile(`(?im)error`)
来源：http://xbv.0kj1m.cn

Ruby: s.scan(/error/i)
来源：http://zgu.sysykeji.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://uwr.ehwqpu.com

[I08] 贪婪与非贪婪匹配
来源：http://lam.sysykeji.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://euw.zhixingplan.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://gpu.ydjk.org.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ain.zhijiandao.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://jjq.guowangkeji.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://elm.ppjwa.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://aek.cdnleiting.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://gey.snrcjt.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://nfu.hnxiangtu.top

================================================================================
来源：http://vzh.ybcxt.top

J. 日期与时间
来源：http://eox.smart0.xyz

================================================================================
来源：http://kov.yfazqb.com

[J01] 获取当前时间
来源：http://oog.gzhubu.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://uzg.wangshuangyany.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://jfn.dianchejie.cn

JS:   new Date();  Date.now()
来源：http://ubh.cdnleiting.top

TS:   new Date();  Date.now()
来源：http://qyb.wangshuangyany.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://ljq.yj20258.top

Go:   time.Now()
来源：http://fpq.fanxiaobao.xyz

Ruby: Time.now
来源：http://kem.ehwqpu.com

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://dmi.yueranfly.top

[J02] 格式化输出
来源：http://fdz.shanyushiyangkeji.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://eat.xziqi.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://qnk.jinghuilouyu.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://nji.guowangkeji.top

TS:   d.toISOString()
来源：http://pgx.zhijiandao.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://bbl.ehwqpu.com

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hbf.sysykeji.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://sbw.jianghu66.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://awg.xinyue.icu

[J03] 字符串解析为日期
来源：http://rlz.aizwys.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://cnj.tianlin.xyz

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://pnk.shzxlz.cn

JS:   new Date("2024-01-02")
来源：http://chs.xylfe.cn

TS:   new Date("2024-01-02")
来源：http://cge.zycfv.cn

Java: LocalDate.parse("2024-01-02")
来源：http://xez.sweek.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://onj.yj202588.top

Ruby: Date.parse("2024-01-02")
来源：http://tdn.xuetiantiany.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://iit.jlsjyb.cn

[J04] 时间戳与日期互转
来源：http://kwm.yuxming.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://jpi.aizwys.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://gta.fktsv.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://fnl.hywenlv.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://kyw.hysaishi.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hib.shangyingyoupin.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://zor.birdmap.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://aol.gzhubu.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://nkj.vqdsnc.cn

[J05] 时间加减（加 7 天）
来源：http://cve.haohaochexian.top

Py:   now + timedelta(days=7)
来源：http://yaf.sjlbkw.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://kdk.hammf.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ktm.andypj.xyz

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://pwe.sweek.top

Java: LocalDate.now().plusDays(7)
来源：http://skk.jinqigfzy.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://pah.chenjidiqi.icu

Ruby: Time.now + 7 * 86400
来源：http://rrd.hnxiangtu.top

C#:   DateTime.Now.AddDays(7)
来源：http://mdh.zycfv.cn

[J06] 计算两时间之差
来源：http://efm.yueranfly.top

Py:   (end - start).total_seconds()
来源：http://yqn.mhx1999.top

PHP:  $end->diff($start)->days;
来源：http://qwm.sysykeji.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ayl.hnqzz.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://bnp.epnwcf.com

Java: Duration.between(start, end).toSeconds()
来源：http://bcl.0kj1m.cn

Go:   end.Sub(start).Hours()
来源：http://uva.chenlongwang.top

Ruby: end - start                 # 返回秒数
来源：http://zgg.jqgfzy.top

C#:   (end - start).TotalSeconds
来源：http://zmt.fktsv.cn

[J07] 比较两个日期
来源：http://izz.tianlin.xyz

Py:   d1 < d2;  d1 == d2
来源：http://bfy.jqgfzy.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://sgo.tianlin.xyz

JS:   d1.getTime() < d2.getTime()
来源：http://owa.jianghu66.top

TS:   d1.getTime() < d2.getTime()
来源：http://zky.fehbvm.com

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://sfq.sysykeji.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://cdm.sufxvd.cn

Ruby: d1 < d2;  d1 == d2
来源：http://zgn.yonumen.top

C#:   d1 < d2;  d1 == d2
来源：http://zkj.quarkkingdee.top

[J08] 提取年月日与星期
来源：http://lme.yangfankeji.com

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://pyf.yanxiufei.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://sri.ppjwa.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://gvt.ybcxt.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://adq.chenlongwang.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://tyg.fzhhl.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://jwi.zdbjq.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://pwc.meibo888.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://kpk.kuanghao11.cn

[J09] 时区处理
来源：http://mfz.hywenlv.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://nxl.meibo888.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://dsv.wangshuangyany.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ihu.sysykeji.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://kry.fengsongda.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://bte.xuetiantiany.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://qcg.guowangkeji.top

Ruby: Time.now.getlocal("+08:00")
来源：http://nlh.zycfv.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://jcm.hesvh.cn

[J10] 取今天 / 本月第一天
来源：http://voy.jinqigufen.top

Py:   date.today();  date.today().replace(day=1)
来源：http://cwb.zhijiandao.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://smh.fehbvm.com

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://bfm.jqgfzy.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://oxr.smart0.xyz

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://qzg.tanke756.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://yjp.sweek.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://tan.hesvh.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://mfr.jinyuanbaomall.cn

================================================================================
来源：http://jhc.guowangkeji.top

K. JSON 与序列化
来源：http://imd.cheryme.top

================================================================================
来源：http://mfk.xinyue.icu

[K01] 对象转 JSON 字符串
来源：http://dfm.feifeiyinyue.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://zgv.snrcjt.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ykb.smart0.xyz

JS:   JSON.stringify(obj)
来源：http://mun.ehwqpu.com

TS:   JSON.stringify(obj)
来源：http://feu.hnxiangtu.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://lvl.fengsongda.top

Go:   json.Marshal(obj)
来源：http://ynx.chenjidiqi.icu

Ruby: obj.to_json                                     // require "json"
来源：http://xrj.fehbvm.com

C#:   JsonSerializer.Serialize(obj)
来源：http://roa.yvedp.cn

[K02] JSON 字符串转对象
来源：http://qgb.shzxlz.cn

Py:   json.loads(s)
来源：http://rvp.zhijiandao.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://fld.tanke756.top

JS:   JSON.parse(s)
来源：http://eul.iojbl.cn

TS:   JSON.parse(s)
来源：http://req.nanxinkj.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://thn.mhx1999.top

Go:   json.Unmarshal(data, &v)
来源：http://vpp.zhaomingkeji.xyz

Ruby: JSON.parse(s)
来源：http://ofl.fktsv.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://iup.meibo888.top

[K03] JSON 美化输出（带缩进）
来源：http://wli.yfazqb.com

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://get.hammf.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wmj.ydzc1.top

JS:   JSON.stringify(obj, null, 2)
来源：http://wkz.jianghu66.top

TS:   JSON.stringify(obj, null, 2)
来源：http://pnu.meibo888.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://asg.9152youxi.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ezh.feifeiyinyue.top

Ruby: JSON.pretty_generate(obj)
来源：http://jla.cashguo.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://pga.ctjpmb.com

[K04] 读取 JSON 文件
来源：http://ojd.dianchejie.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://wwd.hammf.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ewq.nanxuanxn.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://iku.chenlongwang.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://nic.zhaomingkeji.xyz

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://yba.hysaishi.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://jrp.316326.xyz

Ruby: JSON.parse(File.read("a.json"))
来源：http://azw.daria6918.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://cvn.kuanghao11.cn

[K05] 深拷贝对象
来源：http://zxc.quarkkingdee.top

Py:   copy.deepcopy(obj)
来源：http://egy.xinyue.icu

PHP:  unserialize(serialize($obj));
来源：http://mwe.zhengqikj.top

JS:   structuredClone(obj)
来源：http://iuq.tanke756.top

TS:   structuredClone(obj)
来源：http://inh.xuanzx.com

Java: // 手写拷贝构造，或序列化往返
来源：http://sft.gzhubu.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://rtf.ivvv.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://tds.snrcjt.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://okk.shanyushiyangtech.top

[K06] 解析 URL 查询串
来源：http://dkp.zhixingplan.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://vig.aibaodan.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://bwl.c1oappe.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://gir.shangyingyoupin.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://laa.shanyushiyangkeji.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wri.jlsjyb.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://wiv.nwbrower.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://jfc.aibaodan.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://vsk.gotoacloud.top

[K07] 进制转换
来源：http://euk.feifeiyinyue.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wdz.bjfxy.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ldd.dashuyun.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://dqe.havefunace.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ush.redwolf501.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://xty.birdmap.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://snv.hywenlv.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://cvy.gogol.net.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://nvl.ctjpmb.com

[K08] 二进制序列化（非 JSON）
来源：http://szq.yj20258.top

Py:   pickle.dumps(obj)
来源：http://ncz.yueranfly.top

PHP:  serialize($obj);  unserialize($s);
来源：http://rib.fengsongda.top

JS:   v8.serialize(obj)        // Node
来源：http://csf.dashuyun.cn

TS:   v8.serialize(obj)        // Node
来源：http://hux.tarul.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://gpr.xinyue.icu

Go:   encoding/gob
来源：http://ixk.jyoumei.cn

Ruby: Marshal.dump(obj)
来源：http://ird.fanxiaobao.xyz

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://qqn.hnqzz.top

================================================================================
来源：http://owk.ivvv.top

L. 网络请求
来源：http://eos.uphjek.com

================================================================================
来源：http://nwj.zhixingplan.top

[L01] 发送 GET 请求
来源：http://cua.chenlongwang.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://cqv.gotoacloud.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://rhc.hnqzz.top

JS:   await fetch(url)
来源：http://wsr.sweek.top

TS:   await fetch(url)
来源：http://eod.yj20258.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://zmq.wangshuangyany.cn

Go:   resp, err := http.Get(url)
来源：http://pyo.zhengqikj.top

Ruby: Net::HTTP.get(URI(url))
来源：http://qwo.yueranfly.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://lxy.quarkkingdee.top

[L02] 发送 POST JSON
来源：http://ygf.guowangkeji.top

Py:   requests.post(url, json={"a": 1})
来源：http://qzd.shuidangran.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://kex.shangyingyoupin.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://aru.52xcode.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://lnf.hnqzz.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ojl.hfpthk.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://yea.hysaishi.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://xfg.xylfe.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wbs.vehdjk.com

[L03] 设置自定义请求头
来源：http://zwa.shangyingyoupin.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://bol.0kj1m.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://jjy.c1oappe.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://nfn.tarul.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://zyn.zdqjudy.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://enm.feifeiyinyue.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://oqk.fehbvm.com

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://qdt.jiagoushi.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://zus.hysaishi.cn

[L04] 设置超时
来源：http://mml.aibaodan.cn

Py:   requests.get(url, timeout=5)
来源：http://jir.fzhhl.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ocr.havefunace.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://uqk.ywan-chungtsiang.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://fii.bjfxy.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://zde.bbcook.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://qsr.gzhubu.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://qca.xuetiantiany.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://fyf.yj20258.top

[L05] 上传文件（multipart）
来源：http://eah.yuxming.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://dof.xylfe.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://jqh.hcnkem.com

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://nvc.ybcxt.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://cuu.ehwqpu.com

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://keq.sysykeji.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://vth.hnxiangtu.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://agp.hfpthk.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://exq.fanxiaobao.xyz

[L06] 解析响应为 JSON
来源：http://mnx.xylfe.cn

Py:   resp.json()
来源：http://bkr.guannengcc.top

PHP:  json_decode($body, true);
来源：http://rey.ybcxt.top

JS:   await resp.json()
来源：http://dpd.gaohongyu789.top

TS:   await resp.json()
来源：http://rnt.yanxiufei.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://leh.cheryme.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://pxr.jqgfzy.top

Ruby: JSON.parse(resp.body)
来源：http://rpv.hongshengwenyu.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ibh.xuanzx.com


<!-- 参考信息 -->