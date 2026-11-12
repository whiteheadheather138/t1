代发 wailian999

================================================================================
来源：http://vhc.guowangkeji.top

I. 正则表达式
来源：http://hnl.cdnleiting.top

================================================================================
来源：http://goz.wangdashe.top

[I01] 判断是否匹配
来源：http://qgl.xylfe.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://klm.aizwys.cn

PHP:  preg_match('/\d+/', $s);
来源：http://gqi.yj20258888.top

JS:   /\d+/.test(s)
来源：http://ahu.cheryme.top

TS:   /\d+/.test(s)
来源：http://ktw.cheryme.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://zsg.xingfuxueyuan.xyz

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://iuj.zhengqikj.top

Ruby: s.match?(/\d+/)
来源：http://ozl.ppjwa.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://lhy.shzxlz.cn

[I02] 提取所有匹配
来源：http://lwk.yueranfly.top

Py:   re.findall(r"\d+", s)
来源：http://slz.zhixingplan.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://tbq.pengpengdd.cyou

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://cmq.c1oappe.top

TS:   s.match(/\d+/g)
来源：http://ohc.havefunace.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://wrq.havefunace.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hdu.vqdsnc.cn

Ruby: s.scan(/\d+/)
来源：http://nvh.hcnkem.com

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://gsr.jlsjyb.cn

[I03] 提取捕获分组
来源：http://pyc.chenzaomai.com

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://uei.jqgufenzy.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://jgt.cheryme.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://efu.hysaishi.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://jeg.tarul.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://pfb.redwolf501.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://dhk.aibaodan.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ugn.shanyushiyangkeji.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://scz.jianghu66.top

[I04] 正则替换
来源：http://wzh.0kj1m.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://ezi.yj202588.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://pst.yueranfly.top

JS:   s.replace(/\d+/g, "#")
来源：http://gzj.aibaodan.cn

TS:   s.replace(/\d+/g, "#")
来源：http://oqz.gzhubu.top

Java: s.replaceAll("\\d+", "#")
来源：http://hll.ydjk.org.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://dkn.chenlongwang.top

Ruby: s.gsub(/\d+/, "#")
来源：http://dbu.hnxiangtu.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hey.cqqwz.cn

[I05] 按正则拆分
来源：http://wpa.quarkkingdee.top

Py:   re.split(r"\s*,\s*", s)
来源：http://kov.yuxming.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://qaf.chenlongwang.top

JS:   s.split(/\s*,\s*/)
来源：http://lri.ctjpmb.com

TS:   s.split(/\s*,\s*/)
来源：http://fwg.chenjidiqi.icu

Java: s.split("\\s*,\\s*")
来源：http://lqu.jiagoushi.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://qhd.zhengqikj.top

Ruby: s.split(/\s*,\s*/)
来源：http://pev.nwbrower.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://tuv.zhixingplan.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://pes.yanxiufei.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://phg.fengsongda.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://too.gaohongyu789.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://uiq.gaohongyu789.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://buh.sufxvd.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://cdy.jinqigfzy.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://eps.guowangkeji.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://qfl.hcnkem.com

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://uba.redwolf501.top

[I07] 忽略大小写与多行模式
来源：http://iqd.zdqjudy.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://vtu.shanyushiyangkeji.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://xek.jqgufenzy.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://whr.hammf.cn

TS:   /error/gim
来源：http://bki.nwbrower.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://syi.pengpengdd.cyou

Go:   regexp.MustCompile(`(?im)error`)
来源：http://gqy.mhx1999.top

Ruby: s.scan(/error/i)
来源：http://opy.nwbrower.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hqg.xziqi.cn

[I08] 贪婪与非贪婪匹配
来源：http://azi.hesvh.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://dfj.dianchejie.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ims.yuxming.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://iew.haohaochexian.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://zmc.tian-w.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://evv.gaohongyu789.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://eui.zhiwuduotai.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://uat.fehbvm.com

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ayk.quarkkingdee.top

================================================================================
来源：http://uxj.ybcxt.top

J. 日期与时间
来源：http://rey.zhixingplan.top

================================================================================
来源：http://nfq.hnxiangtu.top

[J01] 获取当前时间
来源：http://vry.chenjidiqi.icu

Py:   datetime.now();  datetime.now(UTC)
来源：http://ekr.uphjek.com

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ofl.haohaochexian.top

JS:   new Date();  Date.now()
来源：http://rax.yj202588.top

TS:   new Date();  Date.now()
来源：http://xib.yangfankeji.com

Java: LocalDateTime.now();  Instant.now()
来源：http://fhq.jinghuilouyu.cn

Go:   time.Now()
来源：http://mih.gaohongyu789.top

Ruby: Time.now
来源：http://afq.zhoulong.xyz

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://yda.kuanghao11.cn

[J02] 格式化输出
来源：http://nuf.chenlongwang.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://tbl.jianghu66.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://nqi.shanyushiyangtech.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://fun.gzhubu.top

TS:   d.toISOString()
来源：http://aof.yongpay.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://mxg.andypj.xyz

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://uiw.chenlongwang.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://pgb.epnwcf.com

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://xnb.zhiwuduotai.top

[J03] 字符串解析为日期
来源：http://imc.fengsongda.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://qdg.dianchejie.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://tch.jianghu66.top

JS:   new Date("2024-01-02")
来源：http://thx.sjlbkw.cn

TS:   new Date("2024-01-02")
来源：http://oeq.gotoacloud.top

Java: LocalDate.parse("2024-01-02")
来源：http://bsf.sxryk.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://nym.bjfxy.top

Ruby: Date.parse("2024-01-02")
来源：http://mbm.fzhhl.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://vnq.yj20258888.top

[J04] 时间戳与日期互转
来源：http://ejv.epnwcf.com

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://imi.hcnkem.com

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://lnf.hcnkem.com

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://yjh.zdbjq.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://xqh.fengsongda.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://mzm.hywenlv.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://jyi.iojbl.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://cyb.ydjk.org.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://mqt.jianghu66.top

[J05] 时间加减（加 7 天）
来源：http://zfw.guannengcc.top

Py:   now + timedelta(days=7)
来源：http://qlx.nanxuanxn.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://vba.guannengcc.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://syi.feifeiyinyue.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://gmm.zhoulong.xyz

Java: LocalDate.now().plusDays(7)
来源：http://fzt.cdnleiting.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://guz.jlsjyb.cn

Ruby: Time.now + 7 * 86400
来源：http://tqv.yvedp.cn

C#:   DateTime.Now.AddDays(7)
来源：http://vuc.xingfuxueyuan.xyz

[J06] 计算两时间之差
来源：http://xcg.redwolf501.top

Py:   (end - start).total_seconds()
来源：http://opw.kuanghao11.cn

PHP:  $end->diff($start)->days;
来源：http://tel.zdqjudy.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://sna.gaohongyu789.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://szz.birdmap.top

Java: Duration.between(start, end).toSeconds()
来源：http://vjp.guowangkeji.top

Go:   end.Sub(start).Hours()
来源：http://lxw.jianghu66.top

Ruby: end - start                 # 返回秒数
来源：http://suc.yangfankeji.com

C#:   (end - start).TotalSeconds
来源：http://sxw.vehdjk.com

[J07] 比较两个日期
来源：http://ndo.52xcode.cn

Py:   d1 < d2;  d1 == d2
来源：http://yff.shanyushiyangtech.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://yic.fehbvm.com

JS:   d1.getTime() < d2.getTime()
来源：http://lll.fktsv.cn

TS:   d1.getTime() < d2.getTime()
来源：http://ecb.aibaodan.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://gnm.zdbjq.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://jic.sxryk.cn

Ruby: d1 < d2;  d1 == d2
来源：http://lwg.cqqwz.cn

C#:   d1 < d2;  d1 == d2
来源：http://zkt.hysaishi.cn

[J08] 提取年月日与星期
来源：http://cns.nanxuanxn.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hft.daria6918.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://tim.nanxinkj.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://dpt.sweek.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://qcr.dianchejie.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ory.yvedp.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://sex.xylfe.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://qbb.svipenyu.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://css.tanke756.top

[J09] 时区处理
来源：http://qqv.316326.xyz

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://htd.xylfe.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://sbc.yongpay.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://oar.uphjek.com

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://nym.shangyingyoupin.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://eeb.zhoulong.xyz

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://yhd.hfpthk.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://szm.fktsv.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://kwh.ivvv.top

[J10] 取今天 / 本月第一天
来源：http://nxt.snrcjt.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://xap.52xcode.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://gxq.52xcode.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://pqf.meibo888.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://htb.9152youxi.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://acx.ydzc1.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://daz.shanyushiyangtech.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://uvk.jinghuilouyu.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hny.shuidangran.top

================================================================================
来源：http://pfn.zdbjq.cn

K. JSON 与序列化
来源：http://grt.yonumen.top

================================================================================
来源：http://heb.jyoumei.cn

[K01] 对象转 JSON 字符串
来源：http://xry.zdbjq.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://kad.redwolf501.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://osq.epnwcf.com

JS:   JSON.stringify(obj)
来源：http://fly.gogol.net.cn

TS:   JSON.stringify(obj)
来源：http://iou.sufxvd.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://etb.nwbrower.top

Go:   json.Marshal(obj)
来源：http://kvc.zhijiandao.cn

Ruby: obj.to_json                                     // require "json"
来源：http://syk.tian-w.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://flw.ybcxt.top

[K02] JSON 字符串转对象
来源：http://way.xinyue.icu

Py:   json.loads(s)
来源：http://dpt.jinqigfzy.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://xay.zdqjudy.top

JS:   JSON.parse(s)
来源：http://sbf.yonumen.top

TS:   JSON.parse(s)
来源：http://fps.zhengqikj.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://bif.wangshuangyany.cn

Go:   json.Unmarshal(data, &v)
来源：http://qnz.zhaomingkeji.xyz

Ruby: JSON.parse(s)
来源：http://xow.gaohongyu789.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://epr.zdqjudy.top

[K03] JSON 美化输出（带缩进）
来源：http://uwy.ybcxt.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://lmr.yj20258.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://afc.guannengcc.top

JS:   JSON.stringify(obj, null, 2)
来源：http://yif.tanke756.top

TS:   JSON.stringify(obj, null, 2)
来源：http://rco.jyoumei.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://jec.xingfuxueyuan.xyz

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://adi.pengpengdd.cyou

Ruby: JSON.pretty_generate(obj)
来源：http://quf.yfazqb.com

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://egc.meibo888.top

[K04] 读取 JSON 文件
来源：http://ibl.52xcode.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ucz.guannengcc.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://tgu.gzhubu.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wkq.chenzaomai.com

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://tah.cdnleiting.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://qfv.ybcxt.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://emv.shanyushiyangkeji.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://kvp.316326.xyz

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://jyo.hongshengwenyu.top

[K05] 深拷贝对象
来源：http://gom.ybcxt.top

Py:   copy.deepcopy(obj)
来源：http://rol.nanxinkj.top

PHP:  unserialize(serialize($obj));
来源：http://kgb.hesvh.cn

JS:   structuredClone(obj)
来源：http://qwx.chenlongwang.top

TS:   structuredClone(obj)
来源：http://teu.sweek.top

Java: // 手写拷贝构造，或序列化往返
来源：http://jzw.ehwqpu.com

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://btv.c1oappe.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://vij.zhoulong.xyz

C#:   // 序列化往返，或自定义 Clone
来源：http://bdb.hywenlv.cn

[K06] 解析 URL 查询串
来源：http://kon.hcnkem.com

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://cjc.zdbjq.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://seg.jinyuanbaomall.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://des.bbcook.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://nwb.hammf.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ets.daxiang520.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://trf.uphjek.com

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://kso.yonumen.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://bbs.xingfuxueyuan.xyz

[K07] 进制转换
来源：http://rvb.fengsongda.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://luf.feifeiyinyue.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://zjf.52xcode.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://pid.redwolf501.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://sbf.shzxlz.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://znm.zhixingplan.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://tfl.vqdsnc.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mvy.mhx1999.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hwr.fzhhl.top

[K08] 二进制序列化（非 JSON）
来源：http://jfj.hnxiangtu.top

Py:   pickle.dumps(obj)
来源：http://igc.tianlin.xyz

PHP:  serialize($obj);  unserialize($s);
来源：http://ulj.yj20258.top

JS:   v8.serialize(obj)        // Node
来源：http://fzv.andypj.xyz

TS:   v8.serialize(obj)        // Node
来源：http://ron.hfpthk.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://jff.yuanzhike.top

Go:   encoding/gob
来源：http://xua.cheryme.top

Ruby: Marshal.dump(obj)
来源：http://tqb.fanxiaobao.xyz

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ipi.daria6918.cn

================================================================================
来源：http://zim.chenjidiqi.icu

L. 网络请求
来源：http://cve.hfpthk.cn

================================================================================
来源：http://kjj.fanxiaobao.xyz

[L01] 发送 GET 请求
来源：http://yuo.fehbvm.com

Py:   requests.get(url)                        # 第三方库 requests
来源：http://qcv.fengsongda.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://xnm.wangshuangyany.cn

JS:   await fetch(url)
来源：http://slq.ehwqpu.com

TS:   await fetch(url)
来源：http://bcg.smart0.xyz

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://fnv.zycfv.cn

Go:   resp, err := http.Get(url)
来源：http://sue.ywan-chungtsiang.top

Ruby: Net::HTTP.get(URI(url))
来源：http://nyb.ydzc1.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://sus.fktsv.cn

[L02] 发送 POST JSON
来源：http://tro.cqqwz.cn

Py:   requests.post(url, json={"a": 1})
来源：http://cpb.0kj1m.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://txq.meibo888.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://qsm.nanxinkj.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://dbj.gotoacloud.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://uit.jqgufenzy.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://elh.gogol.net.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://kxx.ywan-chungtsiang.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://evi.smart0.xyz

[L03] 设置自定义请求头
来源：http://ozh.bjfxy.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://avm.vehdjk.com

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://fui.nanxuanxn.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://adt.hywenlv.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mqq.snrcjt.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wxf.xuanzx.com

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://qnp.svipenyu.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ffm.zycfv.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://unw.zhaomingkeji.xyz

[L04] 设置超时
来源：http://bif.jlsjyb.cn

Py:   requests.get(url, timeout=5)
来源：http://zdt.shanyushiyangtech.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://kju.hysaishi.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ugo.zhongyouzk.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://qpd.ydzc1.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wzb.zhiwuduotai.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://btv.chenzaomai.com

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://duh.xingfuxueyuan.xyz

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://fli.yongpay.top

[L05] 上传文件（multipart）
来源：http://mni.yanxiufei.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://dsd.shzxlz.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ium.yuxming.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://kyg.jinyuanbaomall.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ofi.yfazqb.com

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wfh.yfazqb.com

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://xtq.nanxuanxn.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://xrq.ywan-chungtsiang.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://xwd.dianchejie.cn

[L06] 解析响应为 JSON
来源：http://qaa.daria6918.cn

Py:   resp.json()
来源：http://vbu.guowangkeji.top

PHP:  json_decode($body, true);
来源：http://qss.vqdsnc.cn

JS:   await resp.json()
来源：http://ymh.hysaishi.cn

TS:   await resp.json()
来源：http://lvw.wangshuangyany.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://xnn.ivvv.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://zui.ivvv.top

Ruby: JSON.parse(resp.body)
来源：http://kas.nanxinkj.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mfb.xingfuxueyuan.xyz


<!-- 参考信息 -->