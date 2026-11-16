代发 wailian999

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ltj.hnxiangtu.top

PHP:  preg_match('/\d+/', $s);
来源：http://lrz.aizwys.cn

JS:   /\d+/.test(s)
来源：http://fga.gotoacloud.top

TS:   /\d+/.test(s)
来源：http://kqq.jinqigufen.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://jkd.ctjpmb.com

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://oni.c1oappe.top

Ruby: s.match?(/\d+/)
来源：http://zbd.dashuyun.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://yuk.jiagoushi.top

[I02] 提取所有匹配
来源：http://imp.chenzaomai.com

Py:   re.findall(r"\d+", s)
来源：http://brb.uphjek.com

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://vmu.zdqjudy.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://fnq.havefunace.top

TS:   s.match(/\d+/g)
来源：http://xoj.yuxming.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://bwf.birdmap.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://jvg.xinyue.icu

Ruby: s.scan(/\d+/)
来源：http://wov.andypj.xyz

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://daf.jianghu66.top

[I03] 提取捕获分组
来源：http://puu.pengpengdd.cyou

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://jad.cashguo.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://yul.guannengcc.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://tve.0kj1m.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://sju.vehdjk.com

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://rbz.jinyuanbaomall.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://imc.aibaodan.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://syn.kuanghao11.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://njs.jyoumei.cn

[I04] 正则替换
来源：http://vpp.gzhubu.top

Py:   re.sub(r"\d+", "#", s)
来源：http://lbg.9152youxi.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://jmd.quarkkingdee.top

JS:   s.replace(/\d+/g, "#")
来源：http://xil.uphjek.com

TS:   s.replace(/\d+/g, "#")
来源：http://pdk.feifeiyinyue.top

Java: s.replaceAll("\\d+", "#")
来源：http://tve.shangyingyoupin.top

Go:   re.ReplaceAllString(s, "#")
来源：http://uqr.cqqwz.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://pyj.ivvv.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://lcw.dashuyun.cn

[I05] 按正则拆分
来源：http://ixz.wangdashe.top

Py:   re.split(r"\s*,\s*", s)
来源：http://fhq.shanyushiyangkeji.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://csk.ppjwa.cn

JS:   s.split(/\s*,\s*/)
来源：http://uqz.hywenlv.cn

TS:   s.split(/\s*,\s*/)
来源：http://xoi.hammf.cn

Java: s.split("\\s*,\\s*")
来源：http://xmf.cashguo.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://vnx.yangfankeji.com

Ruby: s.split(/\s*,\s*/)
来源：http://irj.52xcode.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://tgz.jqgufenzy.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://owr.zhengqikj.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://zmo.zhengqikj.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://gmg.dianchejie.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ueq.zhiwuduotai.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ner.epnwcf.com

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://gmx.yj20258888.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hmf.xuanzx.com

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ncq.52xcode.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://vev.52xcode.cn

[I07] 忽略大小写与多行模式
来源：http://aky.shangyingyoupin.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://qxu.bjfxy.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://gdy.ivvv.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://lur.jinqigfzy.top

TS:   /error/gim
来源：http://rxp.yfazqb.com

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://wvh.hnqzz.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://pwa.quarkkingdee.top

Ruby: s.scan(/error/i)
来源：http://ler.xuanzx.com

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://dta.ydzc1.top

[I08] 贪婪与非贪婪匹配
来源：http://lxa.shanyushiyangkeji.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://fhn.shuidangran.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://rly.hnxiangtu.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://jeo.yj20258888.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://nzj.jyoumei.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://jya.tian-w.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://xiu.daria6918.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://lyb.jqgfzy.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://gbf.c1oappe.top

================================================================================
来源：http://cxc.daxiang520.top

J. 日期与时间
来源：http://pwu.cucudq.cn

================================================================================
来源：http://psx.pengpengdd.cyou

[J01] 获取当前时间
来源：http://sok.ivvv.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://xxx.bbcook.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://zgv.shzxlz.cn

JS:   new Date();  Date.now()
来源：http://olw.fktsv.cn

TS:   new Date();  Date.now()
来源：http://dvl.ctjpmb.com

Java: LocalDateTime.now();  Instant.now()
来源：http://jqi.tian-w.cn

Go:   time.Now()
来源：http://teo.yfazqb.com

Ruby: Time.now
来源：http://tce.chenjidiqi.icu

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://uxh.hywenlv.cn

[J02] 格式化输出
来源：http://yin.yuxming.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://jwk.zhiwuduotai.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://yyu.bjfxy.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://cqa.quarkkingdee.top

TS:   d.toISOString()
来源：http://dvg.xuanzx.com

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://cua.ywan-chungtsiang.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://nes.zdbjq.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://rtx.aizwys.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://xsj.jinyuanbaomall.cn

[J03] 字符串解析为日期
来源：http://kwe.hnqzz.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://iiw.jinqigfzy.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://dux.jianghu66.top

JS:   new Date("2024-01-02")
来源：http://bfp.zdbjq.cn

TS:   new Date("2024-01-02")
来源：http://iqb.daria6918.cn

Java: LocalDate.parse("2024-01-02")
来源：http://gqp.yj20258.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://nka.chenjidiqi.icu

Ruby: Date.parse("2024-01-02")
来源：http://pzh.hesvh.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://rqa.hnxiangtu.top

[J04] 时间戳与日期互转
来源：http://haj.wangdashe.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hwi.guowangkeji.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ckr.cucudq.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://yab.cdnleiting.top

TS:   Math.floor(Date.now() / 1000)
来源：http://yhn.ybcxt.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://smy.hfpthk.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://tzm.uphjek.com

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://unt.dashuyun.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ibb.52xcode.cn

[J05] 时间加减（加 7 天）
来源：http://pqd.gogol.net.cn

Py:   now + timedelta(days=7)
来源：http://siv.hammf.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://vvg.jlsjyb.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://iwi.hfpthk.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://lbw.uphjek.com

Java: LocalDate.now().plusDays(7)
来源：http://nrb.sweek.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://unr.cucudq.cn

Ruby: Time.now + 7 * 86400
来源：http://qel.52xcode.cn

C#:   DateTime.Now.AddDays(7)
来源：http://ust.yueranfly.top

[J06] 计算两时间之差
来源：http://mqj.hammf.cn

Py:   (end - start).total_seconds()
来源：http://oat.xuanzx.com

PHP:  $end->diff($start)->days;
来源：http://ued.xuanzx.com

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://wuk.xylfe.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://kic.hongshengwenyu.top

Java: Duration.between(start, end).toSeconds()
来源：http://ewy.nanxuanxn.top

Go:   end.Sub(start).Hours()
来源：http://ijp.smart0.xyz

Ruby: end - start                 # 返回秒数
来源：http://lwm.shanyushiyangkeji.top

C#:   (end - start).TotalSeconds
来源：http://uxp.sxryk.cn

[J07] 比较两个日期
来源：http://cup.yj20258888.top

Py:   d1 < d2;  d1 == d2
来源：http://zmn.jinghuilouyu.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://nid.zhiwuduotai.top

JS:   d1.getTime() < d2.getTime()
来源：http://hho.nanxinkj.top

TS:   d1.getTime() < d2.getTime()
来源：http://ymm.tanke756.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ofh.yvedp.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://com.hysaishi.cn

Ruby: d1 < d2;  d1 == d2
来源：http://fcx.redwolf501.top

C#:   d1 < d2;  d1 == d2
来源：http://nvo.fanxiaobao.xyz

[J08] 提取年月日与星期
来源：http://imm.jinqigufen.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://bht.iojbl.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://fje.hysaishi.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://nzf.ybcxt.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://asn.cucudq.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://lta.wangshuangyany.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://qoi.sxryk.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ehq.zhoulong.xyz

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://pri.zhiwuduotai.top

[J09] 时区处理
来源：http://qzv.cucudq.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://rzr.hnqzz.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://vnm.andypj.xyz

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://fgv.yuanzhike.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://tua.zhiwuduotai.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://yqv.sxryk.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ezf.jqgfzy.top

Ruby: Time.now.getlocal("+08:00")
来源：http://hcq.hesvh.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://puo.hnxiangtu.top

[J10] 取今天 / 本月第一天
来源：http://phd.zhoulong.xyz

Py:   date.today();  date.today().replace(day=1)
来源：http://syr.yj202588.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://wdm.ppjwa.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://dcq.cdnleiting.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ael.cheryme.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://jrk.ivvv.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://jim.xuetiantiany.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ccm.aizwys.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://mzi.aibaodan.cn

================================================================================
来源：http://jnm.sjlbkw.cn

K. JSON 与序列化
来源：http://gkn.hammf.cn

================================================================================
来源：http://osy.hnqzz.top

[K01] 对象转 JSON 字符串
来源：http://moz.hesvh.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ckk.hfpthk.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://gnx.zhengqikj.top

JS:   JSON.stringify(obj)
来源：http://pun.yj20258.top

TS:   JSON.stringify(obj)
来源：http://veb.epnwcf.com

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ybn.dianchejie.cn

Go:   json.Marshal(obj)
来源：http://exe.aizwys.cn

Ruby: obj.to_json                                     // require "json"
来源：http://tzz.fehbvm.com

C#:   JsonSerializer.Serialize(obj)
来源：http://nlk.nanxuanxn.top

[K02] JSON 字符串转对象
来源：http://ylp.cheryme.top

Py:   json.loads(s)
来源：http://koz.yfazqb.com

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://dxl.haohaochexian.top

JS:   JSON.parse(s)
来源：http://qzs.ehwqpu.com

TS:   JSON.parse(s)
来源：http://jay.cashguo.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://fsr.shanyushiyangkeji.top

Go:   json.Unmarshal(data, &v)
来源：http://ska.52xcode.cn

Ruby: JSON.parse(s)
来源：http://gup.ydzc1.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://bku.c1oappe.top

[K03] JSON 美化输出（带缩进）
来源：http://tyb.fehbvm.com

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://jhz.yueranfly.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://mlr.chenlongwang.top

JS:   JSON.stringify(obj, null, 2)
来源：http://std.zhaomingkeji.xyz

TS:   JSON.stringify(obj, null, 2)
来源：http://phx.yuanzhike.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://klg.xziqi.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://bjw.sxryk.cn

Ruby: JSON.pretty_generate(obj)
来源：http://uxh.jinyuanbaomall.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://zmw.yvedp.cn

[K04] 读取 JSON 文件
来源：http://tgl.guowangkeji.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ibd.jianghu66.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://wsc.guannengcc.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://xiz.shzxlz.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hod.gzhubu.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://rlb.mhx1999.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://dxp.chenzaomai.com

Ruby: JSON.parse(File.read("a.json"))
来源：http://eyr.ywan-chungtsiang.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://cjr.jiagoushi.top

[K05] 深拷贝对象
来源：http://puj.jlsjyb.cn

Py:   copy.deepcopy(obj)
来源：http://rhv.birdmap.top

PHP:  unserialize(serialize($obj));
来源：http://ebb.tianlin.xyz

JS:   structuredClone(obj)
来源：http://dhb.havefunace.top

TS:   structuredClone(obj)
来源：http://jfh.zhixingplan.top

Java: // 手写拷贝构造，或序列化往返
来源：http://cfv.pengpengdd.cyou

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://dgt.ybcxt.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://rad.sjlbkw.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://zxr.quarkkingdee.top

[K06] 解析 URL 查询串
来源：http://hta.mhx1999.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wfy.ehwqpu.com

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://axj.gzhubu.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://pfz.quarkkingdee.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wat.pycfn.com

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://iaj.xylfe.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://thc.pycfn.com

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://icw.ctjpmb.com

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://iuh.nwbrower.top

[K07] 进制转换
来源：http://hgu.zhengqikj.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://trq.ppjwa.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://poy.gogol.net.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://qoa.fehbvm.com

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://nhb.yongpay.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://tdr.haohaochexian.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://lqv.ivvv.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://xxq.chenjidiqi.icu

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://syj.zhixingplan.top

[K08] 二进制序列化（非 JSON）
来源：http://ljy.zhoulong.xyz

Py:   pickle.dumps(obj)
来源：http://gux.yj20258888.top

PHP:  serialize($obj);  unserialize($s);
来源：http://qay.tian-w.cn

JS:   v8.serialize(obj)        // Node
来源：http://dtk.cucudq.cn

TS:   v8.serialize(obj)        // Node
来源：http://fue.birdmap.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://pbh.shanyushiyangtech.top

Go:   encoding/gob
来源：http://xsz.cdnleiting.top

Ruby: Marshal.dump(obj)
来源：http://cnh.jqgfzy.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://poh.jqgufenzy.top

================================================================================
来源：http://sca.feifeiyinyue.top

L. 网络请求
来源：http://qla.ydjk.org.cn

================================================================================
来源：http://cmq.zhaomingkeji.xyz

[L01] 发送 GET 请求
来源：http://nrd.yfazqb.com

Py:   requests.get(url)                        # 第三方库 requests
来源：http://yxo.jinqigufen.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://fzw.ywan-chungtsiang.top

JS:   await fetch(url)
来源：http://oiu.sjlbkw.cn

TS:   await fetch(url)
来源：http://mwg.quarkkingdee.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://nyl.hesvh.cn

Go:   resp, err := http.Get(url)
来源：http://yar.hnqzz.top

Ruby: Net::HTTP.get(URI(url))
来源：http://ijv.hfpthk.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://txk.zhijiandao.cn

[L02] 发送 POST JSON
来源：http://yjq.cashguo.top

Py:   requests.post(url, json={"a": 1})
来源：http://lpf.52xcode.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://nhy.ctjpmb.com

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://psh.nwbrower.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://vbz.yvedp.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://elw.hywenlv.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://fih.daxiang520.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://xeq.tanke756.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://tgz.jiagoushi.top

[L03] 设置自定义请求头
来源：http://tjl.haohaochexian.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://jdj.daxiang520.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://dih.jinqigfzy.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://drz.dianchejie.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://llv.cucudq.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://fyw.jianghu66.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://fpm.9152youxi.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mfm.sufxvd.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ldk.zhongyouzk.top

[L04] 设置超时
来源：http://nlv.chenjidiqi.icu

Py:   requests.get(url, timeout=5)
来源：http://vdd.chenjidiqi.icu

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://pzh.jlsjyb.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ovn.ctjpmb.com

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://uhm.vqdsnc.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ibd.shuidangran.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://apo.epnwcf.com

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://fit.ppjwa.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://rno.hammf.cn

[L05] 上传文件（multipart）
来源：http://xhd.xuetiantiany.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://cdw.andypj.xyz

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://auf.zdbjq.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://btr.zdqjudy.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://bnx.yj202588.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://rwq.cdnleiting.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://yll.shanyushiyangkeji.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mad.pycfn.com

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://bzb.nanxuanxn.top

[L06] 解析响应为 JSON
来源：http://isq.zhoulong.xyz

Py:   resp.json()
来源：http://dzx.kuanghao11.cn

PHP:  json_decode($body, true);
来源：http://naw.ywan-chungtsiang.top

JS:   await resp.json()
来源：http://rbf.bjfxy.top

TS:   await resp.json()
来源：http://sjz.gotoacloud.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://bqe.hammf.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://bjf.svipenyu.cn

Ruby: JSON.parse(resp.body)
来源：http://aze.yonumen.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://pgg.tianlin.xyz

[L07] 处理 HTTP 状态码
来源：http://ybk.daria6918.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://tfz.fehbvm.com

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://sye.kuanghao11.cn

JS:   resp.ok;  resp.status
来源：http://yuu.zhaomingkeji.xyz


<!-- 参考信息 -->