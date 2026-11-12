代发 wailian999

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ynl.cqqwz.cn

PHP:  preg_match('/\d+/', $s);
来源：http://khi.hnqzz.top

JS:   /\d+/.test(s)
来源：http://tga.hywenlv.cn

TS:   /\d+/.test(s)
来源：http://xcn.shanyushiyangtech.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://erx.c1oappe.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ets.ywan-chungtsiang.top

Ruby: s.match?(/\d+/)
来源：http://jnl.xinyue.icu

C#:   Regex.IsMatch(s, @"\d+")
来源：http://rqg.bbcook.cn

[I02] 提取所有匹配
来源：http://osh.cdnleiting.top

Py:   re.findall(r"\d+", s)
来源：http://met.fehbvm.com

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://htq.wangdashe.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ewx.jinqigufen.top

TS:   s.match(/\d+/g)
来源：http://tlv.smart0.xyz

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://nkg.hongshengwenyu.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://vdl.smart0.xyz

Ruby: s.scan(/\d+/)
来源：http://skb.zhixingplan.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://lpd.yuanzhike.top

[I03] 提取捕获分组
来源：http://xjj.guowangkeji.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://cgt.yj202588.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://tes.yfazqb.com

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://afr.jiagoushi.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ujy.yj20258.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://snh.zhongyouzk.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://eys.fzhhl.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://xlf.shanyushiyangtech.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://cty.chenzaomai.com

[I04] 正则替换
来源：http://vpk.fktsv.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://app.zhixingplan.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://lnl.zhaomingkeji.xyz

JS:   s.replace(/\d+/g, "#")
来源：http://hil.tarul.cn

TS:   s.replace(/\d+/g, "#")
来源：http://okk.hnxiangtu.top

Java: s.replaceAll("\\d+", "#")
来源：http://xtq.snrcjt.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://aes.jiagoushi.top

Ruby: s.gsub(/\d+/, "#")
来源：http://pua.zhongyouzk.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://leh.bbcook.cn

[I05] 按正则拆分
来源：http://kgn.ydjk.org.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://inv.ydzc1.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://vwn.jinqigufen.top

JS:   s.split(/\s*,\s*/)
来源：http://jxj.snrcjt.cn

TS:   s.split(/\s*,\s*/)
来源：http://mgd.yj20258.top

Java: s.split("\\s*,\\s*")
来源：http://alj.tian-w.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hmi.zhijiandao.cn

Ruby: s.split(/\s*,\s*/)
来源：http://nwa.jinqigfzy.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://khf.yueranfly.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ndq.shanyushiyangtech.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://cwx.iojbl.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ptc.daria6918.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://bjj.xingfuxueyuan.xyz

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://gax.316326.xyz

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ujn.pengpengdd.cyou

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://btb.yonumen.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://usu.shanyushiyangkeji.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://bfz.ywan-chungtsiang.top

[I07] 忽略大小写与多行模式
来源：http://poe.jlsjyb.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://mzj.tarul.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://uvs.9152youxi.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://sxk.cashguo.top

TS:   /error/gim
来源：http://tar.ctjpmb.com

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://yra.dianchejie.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://zad.hysaishi.cn

Ruby: s.scan(/error/i)
来源：http://lbw.daria6918.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://jkd.hongshengwenyu.top

[I08] 贪婪与非贪婪匹配
来源：http://yse.ybcxt.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://fbj.hesvh.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ynu.sjlbkw.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://dbf.ybcxt.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ric.xylfe.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://vfw.gotoacloud.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://elo.xinyue.icu

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://yjq.yj20258.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://bti.uphjek.com

================================================================================
来源：http://dpz.zhijiandao.cn

J. 日期与时间
来源：http://sxz.jinyuanbaomall.cn

================================================================================
来源：http://hbl.ydzc1.top

[J01] 获取当前时间
来源：http://euj.shuidangran.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://fvk.chenzaomai.com

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ykf.hfpthk.cn

JS:   new Date();  Date.now()
来源：http://nxe.feifeiyinyue.top

TS:   new Date();  Date.now()
来源：http://yru.jqgfzy.top

Java: LocalDateTime.now();  Instant.now()
来源：http://pth.sufxvd.cn

Go:   time.Now()
来源：http://ecr.sufxvd.cn

Ruby: Time.now
来源：http://wri.meibo888.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://tsb.hcnkem.com

[J02] 格式化输出
来源：http://swu.yfazqb.com

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://uoo.cucudq.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://xhi.jinghuilouyu.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ccp.ydzc1.top

TS:   d.toISOString()
来源：http://upr.zhijiandao.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://gri.tanke756.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ddm.ppjwa.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://lhc.zhixingplan.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://zvk.daria6918.cn

[J03] 字符串解析为日期
来源：http://llx.ivvv.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ulp.ydzc1.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://lwc.zdbjq.cn

JS:   new Date("2024-01-02")
来源：http://frr.bjfxy.top

TS:   new Date("2024-01-02")
来源：http://hhr.havefunace.top

Java: LocalDate.parse("2024-01-02")
来源：http://cam.gaohongyu789.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://isb.daria6918.cn

Ruby: Date.parse("2024-01-02")
来源：http://mqe.ydzc1.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://udf.zdbjq.cn

[J04] 时间戳与日期互转
来源：http://dsg.52xcode.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://cyd.52xcode.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://wsi.shuidangran.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://bgg.hongshengwenyu.top

TS:   Math.floor(Date.now() / 1000)
来源：http://fkj.c1oappe.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://mkv.ppjwa.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://aih.smart0.xyz

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://tfp.chenjidiqi.icu

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://fry.zhaomingkeji.xyz

[J05] 时间加减（加 7 天）
来源：http://wte.sysykeji.top

Py:   now + timedelta(days=7)
来源：http://img.xuanzx.com

PHP:  (new DateTime())->modify("+7 days");
来源：http://bkp.guowangkeji.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://iau.jqgufenzy.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ade.jianghu66.top

Java: LocalDate.now().plusDays(7)
来源：http://pmy.bjfxy.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hib.hammf.cn

Ruby: Time.now + 7 * 86400
来源：http://bnv.yvedp.cn

C#:   DateTime.Now.AddDays(7)
来源：http://hxm.daxiang520.top

[J06] 计算两时间之差
来源：http://qrl.316326.xyz

Py:   (end - start).total_seconds()
来源：http://jdt.shzxlz.cn

PHP:  $end->diff($start)->days;
来源：http://nlm.feifeiyinyue.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ikl.yj202588.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://fnc.quarkkingdee.top

Java: Duration.between(start, end).toSeconds()
来源：http://mue.aibaodan.cn

Go:   end.Sub(start).Hours()
来源：http://qjt.daxiang520.top

Ruby: end - start                 # 返回秒数
来源：http://wzf.cqqwz.cn

C#:   (end - start).TotalSeconds
来源：http://vvh.jianghu66.top

[J07] 比较两个日期
来源：http://bqh.gaohongyu789.top

Py:   d1 < d2;  d1 == d2
来源：http://atg.xylfe.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://efg.guowangkeji.top

JS:   d1.getTime() < d2.getTime()
来源：http://qbc.yueranfly.top

TS:   d1.getTime() < d2.getTime()
来源：http://sgs.9152youxi.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://pyd.zdqjudy.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ltr.fktsv.cn

Ruby: d1 < d2;  d1 == d2
来源：http://wtn.yueranfly.top

C#:   d1 < d2;  d1 == d2
来源：http://hgk.cdnleiting.top

[J08] 提取年月日与星期
来源：http://kqg.xylfe.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://igh.dashuyun.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://csq.zhiwuduotai.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://wnh.yj202588.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://rty.hongshengwenyu.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://cqf.tian-w.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://qmj.hongshengwenyu.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ppa.sjlbkw.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://wem.jqgfzy.top

[J09] 时区处理
来源：http://qjv.jinghuilouyu.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://vhb.epnwcf.com

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://bgx.yj202588.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ebd.jianghu66.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://nhz.yueranfly.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://rrz.redwolf501.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://lxr.cdnleiting.top

Ruby: Time.now.getlocal("+08:00")
来源：http://ath.feifeiyinyue.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://mzr.chenjidiqi.icu

[J10] 取今天 / 本月第一天
来源：http://zpf.yuxming.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://kct.havefunace.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://cjs.yj202588.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://wdi.chenjidiqi.icu

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://vmt.zhijiandao.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hzl.hcnkem.com

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://cmu.ehwqpu.com

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://jda.vqdsnc.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hqj.iojbl.cn

================================================================================
来源：http://fxb.yfazqb.com

K. JSON 与序列化
来源：http://afs.jinyuanbaomall.cn

================================================================================
来源：http://kqc.sweek.top

[K01] 对象转 JSON 字符串
来源：http://tmd.andypj.xyz

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://lgs.jlsjyb.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://umd.yj20258888.top

JS:   JSON.stringify(obj)
来源：http://gph.316326.xyz

TS:   JSON.stringify(obj)
来源：http://rfj.fengsongda.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://dfh.fehbvm.com

Go:   json.Marshal(obj)
来源：http://fdo.yuanzhike.top

Ruby: obj.to_json                                     // require "json"
来源：http://lcc.zhiwuduotai.top

C#:   JsonSerializer.Serialize(obj)
来源：http://hen.zdbjq.cn

[K02] JSON 字符串转对象
来源：http://use.cashguo.top

Py:   json.loads(s)
来源：http://kev.xinyue.icu

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://mmf.c1oappe.top

JS:   JSON.parse(s)
来源：http://krv.svipenyu.cn

TS:   JSON.parse(s)
来源：http://uhl.jinghuilouyu.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://uix.yuxming.cn

Go:   json.Unmarshal(data, &v)
来源：http://udr.xuetiantiany.cn

Ruby: JSON.parse(s)
来源：http://bhn.zhongyouzk.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://qck.ydzc1.top

[K03] JSON 美化输出（带缩进）
来源：http://ljg.meibo888.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://wci.jyoumei.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://zfv.dashuyun.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://nts.hammf.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://zyi.yj20258.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://pvx.0kj1m.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ijr.ctjpmb.com

Ruby: JSON.pretty_generate(obj)
来源：http://zma.yonumen.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://rro.feifeiyinyue.top

[K04] 读取 JSON 文件
来源：http://cjd.jqgfzy.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://onq.bjfxy.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://bcc.hfpthk.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://tbg.havefunace.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://zqb.zhengqikj.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://zjn.jinghuilouyu.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://alv.yuxming.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://apm.svipenyu.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://dxb.yonumen.top

[K05] 深拷贝对象
来源：http://lmw.zhongyouzk.top

Py:   copy.deepcopy(obj)
来源：http://tqm.zhengqikj.top

PHP:  unserialize(serialize($obj));
来源：http://rqx.mhx1999.top

JS:   structuredClone(obj)
来源：http://usv.hesvh.cn

TS:   structuredClone(obj)
来源：http://dmb.pengpengdd.cyou

Java: // 手写拷贝构造，或序列化往返
来源：http://sob.xylfe.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://rjj.tianlin.xyz

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://szd.hammf.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://olb.hnxiangtu.top

[K06] 解析 URL 查询串
来源：http://qvr.shanyushiyangtech.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://nal.tianlin.xyz

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://efw.zhiwuduotai.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ukn.jinqigfzy.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://xjb.snrcjt.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://nrx.sxryk.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://dxw.shangyingyoupin.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://aju.ivvv.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://dfo.shzxlz.cn

[K07] 进制转换
来源：http://frc.guannengcc.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mgt.zhongyouzk.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://vfs.gaohongyu789.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ahl.yfazqb.com

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ofa.9152youxi.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://sdt.hysaishi.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://pxo.xziqi.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://zqw.dashuyun.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ygf.zhijiandao.cn

[K08] 二进制序列化（非 JSON）
来源：http://rqu.cashguo.top

Py:   pickle.dumps(obj)
来源：http://bed.chenlongwang.top

PHP:  serialize($obj);  unserialize($s);
来源：http://plx.snrcjt.cn

JS:   v8.serialize(obj)        // Node
来源：http://gjb.yongpay.top

TS:   v8.serialize(obj)        // Node
来源：http://hlf.vqdsnc.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ubs.yj202588.top

Go:   encoding/gob
来源：http://hmw.yongpay.top

Ruby: Marshal.dump(obj)
来源：http://cxb.fengsongda.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://sfw.hongshengwenyu.top

================================================================================
来源：http://soq.zycfv.cn

L. 网络请求
来源：http://lrj.snrcjt.cn

================================================================================
来源：http://ryj.shanyushiyangtech.top

[L01] 发送 GET 请求
来源：http://ivn.ehwqpu.com

Py:   requests.get(url)                        # 第三方库 requests
来源：http://pob.guowangkeji.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://zid.cashguo.top

JS:   await fetch(url)
来源：http://rou.jinghuilouyu.cn

TS:   await fetch(url)
来源：http://vyv.pycfn.com

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://zdz.birdmap.top

Go:   resp, err := http.Get(url)
来源：http://aqk.smart0.xyz

Ruby: Net::HTTP.get(URI(url))
来源：http://tjx.nanxuanxn.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://mhd.yonumen.top

[L02] 发送 POST JSON
来源：http://haf.meibo888.top

Py:   requests.post(url, json={"a": 1})
来源：http://pub.sufxvd.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://pwv.jiagoushi.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://jir.xinyue.icu

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://lze.shuidangran.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://yfk.wangdashe.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://kpa.birdmap.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://xzc.meibo888.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wqz.cqqwz.cn

[L03] 设置自定义请求头
来源：http://dep.iojbl.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://pwg.ybcxt.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://vpl.chenzaomai.com

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://zbj.zhixingplan.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://vyw.mhx1999.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://tkc.zycfv.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://zge.hysaishi.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://uay.hammf.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://jew.fehbvm.com

[L04] 设置超时
来源：http://kds.shangyingyoupin.top

Py:   requests.get(url, timeout=5)
来源：http://ugq.iojbl.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://lcw.cqqwz.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ncb.c1oappe.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://kzy.birdmap.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wbz.hammf.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ztj.shanyushiyangtech.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://zrt.hywenlv.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://nnp.ydzc1.top

[L05] 上传文件（multipart）
来源：http://bif.yj20258.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://qty.xingfuxueyuan.xyz

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://inj.nwbrower.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://afm.yfazqb.com

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://zjf.quarkkingdee.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://giq.kuanghao11.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://vvc.ctjpmb.com

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://bab.jinyuanbaomall.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://bbb.bbcook.cn

[L06] 解析响应为 JSON
来源：http://nth.zdbjq.cn

Py:   resp.json()
来源：http://clz.zhixingplan.top

PHP:  json_decode($body, true);
来源：http://qog.cdnleiting.top

JS:   await resp.json()
来源：http://ibv.zycfv.cn

TS:   await resp.json()
来源：http://tho.yvedp.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://kbj.c1oappe.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://iyc.quarkkingdee.top

Ruby: JSON.parse(resp.body)
来源：http://jpd.ppjwa.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://epw.hnqzz.top

[L07] 处理 HTTP 状态码
来源：http://dxm.shanyushiyangkeji.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://oiv.fehbvm.com

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://cru.yuxming.cn

JS:   resp.ok;  resp.status
来源：http://pfu.nanxuanxn.top


<!-- 参考信息 -->