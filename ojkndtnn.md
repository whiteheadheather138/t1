代发 wailian999

================================================================================
来源：http://yly.xingfuxueyuan.xyz

I. 正则表达式
来源：http://udm.ehwqpu.com

================================================================================
来源：http://lib.nanxinkj.top

[I01] 判断是否匹配
来源：http://chl.nanxuanxn.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wwb.xuanzx.com

PHP:  preg_match('/\d+/', $s);
来源：http://jce.quarkkingdee.top

JS:   /\d+/.test(s)
来源：http://ivk.quarkkingdee.top

TS:   /\d+/.test(s)
来源：http://itt.dianchejie.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://fps.uphjek.com

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ivu.nwbrower.top

Ruby: s.match?(/\d+/)
来源：http://jgd.yfazqb.com

C#:   Regex.IsMatch(s, @"\d+")
来源：http://mkp.zhongyouzk.top

[I02] 提取所有匹配
来源：http://qgd.zhongyouzk.top

Py:   re.findall(r"\d+", s)
来源：http://hym.xziqi.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://fsq.nwbrower.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://voh.cashguo.top

TS:   s.match(/\d+/g)
来源：http://rqr.gaohongyu789.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ytm.jyoumei.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://xsf.tarul.cn

Ruby: s.scan(/\d+/)
来源：http://yxn.ivvv.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://jyr.uphjek.com

[I03] 提取捕获分组
来源：http://zqv.hesvh.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://epl.yfazqb.com

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://dvf.iojbl.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://jcv.hysaishi.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://spl.shzxlz.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://kpy.chenjidiqi.icu

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://rcg.gaohongyu789.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://pkg.zhoulong.xyz

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://gcg.jinqigfzy.top

[I04] 正则替换
来源：http://dtz.shanyushiyangtech.top

Py:   re.sub(r"\d+", "#", s)
来源：http://aya.andypj.xyz

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://fmx.316326.xyz

JS:   s.replace(/\d+/g, "#")
来源：http://lkd.quarkkingdee.top

TS:   s.replace(/\d+/g, "#")
来源：http://mir.shanyushiyangtech.top

Java: s.replaceAll("\\d+", "#")
来源：http://bjm.fanxiaobao.xyz

Go:   re.ReplaceAllString(s, "#")
来源：http://vlo.sxryk.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://dgy.ybcxt.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://eze.zdbjq.cn

[I05] 按正则拆分
来源：http://mck.jinqigufen.top

Py:   re.split(r"\s*,\s*", s)
来源：http://kbf.birdmap.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ucn.yfazqb.com

JS:   s.split(/\s*,\s*/)
来源：http://zxp.xuanzx.com

TS:   s.split(/\s*,\s*/)
来源：http://ktm.zhaomingkeji.xyz

Java: s.split("\\s*,\\s*")
来源：http://rtz.chenjidiqi.icu

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://zvn.iojbl.cn

Ruby: s.split(/\s*,\s*/)
来源：http://cmx.ywan-chungtsiang.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://tzm.nanxinkj.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://rhl.wangdashe.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://eyn.tian-w.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://gim.svipenyu.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://bmj.iojbl.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://zva.zhaomingkeji.xyz

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://kfe.jyoumei.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://bmx.chenzaomai.com

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://bsy.yvedp.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://vgi.dianchejie.cn

[I07] 忽略大小写与多行模式
来源：http://cxz.zhengqikj.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://vau.cqqwz.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://bfl.birdmap.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://anw.aizwys.cn

TS:   /error/gim
来源：http://wio.hnqzz.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://jjy.ydzc1.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://rrn.birdmap.top

Ruby: s.scan(/error/i)
来源：http://swd.tarul.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://tat.yuanzhike.top

[I08] 贪婪与非贪婪匹配
来源：http://cux.hywenlv.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://jth.jiagoushi.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://yjy.zhoulong.xyz

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://vrt.uphjek.com

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://jqc.fanxiaobao.xyz

Java: Pattern.compile("<b>.*?</b>")
来源：http://eyb.xinyue.icu

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://twg.cucudq.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://zto.wangshuangyany.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://tks.zhengqikj.top

================================================================================
来源：http://zqw.feifeiyinyue.top

J. 日期与时间
来源：http://zvc.jyoumei.cn

================================================================================
来源：http://bnj.yangfankeji.com

[J01] 获取当前时间
来源：http://qru.ydjk.org.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://yzw.hfpthk.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ufv.zhiwuduotai.top

JS:   new Date();  Date.now()
来源：http://rtj.ydzc1.top

TS:   new Date();  Date.now()
来源：http://ita.sxryk.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://hbl.hongshengwenyu.top

Go:   time.Now()
来源：http://bnn.epnwcf.com

Ruby: Time.now
来源：http://kri.vehdjk.com

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://piy.gaohongyu789.top

[J02] 格式化输出
来源：http://bcz.yonumen.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://djy.zhaomingkeji.xyz

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://gbu.cqqwz.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://sdf.epnwcf.com

TS:   d.toISOString()
来源：http://ppq.haohaochexian.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://fbf.xinyue.icu

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://nlw.ywan-chungtsiang.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://lro.9152youxi.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hji.yuxming.cn

[J03] 字符串解析为日期
来源：http://aii.c1oappe.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://kau.yj202588.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://chn.jinqigufen.top

JS:   new Date("2024-01-02")
来源：http://ani.zhijiandao.cn

TS:   new Date("2024-01-02")
来源：http://qnp.yuanzhike.top

Java: LocalDate.parse("2024-01-02")
来源：http://jqk.ydjk.org.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://caj.0kj1m.cn

Ruby: Date.parse("2024-01-02")
来源：http://vya.zdqjudy.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://iyd.chenjidiqi.icu

[J04] 时间戳与日期互转
来源：http://wqm.jiagoushi.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://gak.sxryk.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://aru.fehbvm.com

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://dli.tanke756.top

TS:   Math.floor(Date.now() / 1000)
来源：http://fkp.bjfxy.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://tna.cashguo.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hrd.yonumen.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://vcn.shangyingyoupin.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://zje.xuetiantiany.cn

[J05] 时间加减（加 7 天）
来源：http://trn.zhixingplan.top

Py:   now + timedelta(days=7)
来源：http://phq.cucudq.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://obx.wangdashe.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://rpj.yongpay.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ypo.hammf.cn

Java: LocalDate.now().plusDays(7)
来源：http://cfj.zdqjudy.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://jnm.yvedp.cn

Ruby: Time.now + 7 * 86400
来源：http://noq.guannengcc.top

C#:   DateTime.Now.AddDays(7)
来源：http://erq.hesvh.cn

[J06] 计算两时间之差
来源：http://vpt.uphjek.com

Py:   (end - start).total_seconds()
来源：http://vgz.ctjpmb.com

PHP:  $end->diff($start)->days;
来源：http://tal.sysykeji.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://omm.shangyingyoupin.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://miy.havefunace.top

Java: Duration.between(start, end).toSeconds()
来源：http://udf.hfpthk.cn

Go:   end.Sub(start).Hours()
来源：http://mwj.jinyuanbaomall.cn

Ruby: end - start                 # 返回秒数
来源：http://nzt.ydzc1.top

C#:   (end - start).TotalSeconds
来源：http://lcb.jiagoushi.top

[J07] 比较两个日期
来源：http://reu.andypj.xyz

Py:   d1 < d2;  d1 == d2
来源：http://ttd.jqgufenzy.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://rvx.shangyingyoupin.top

JS:   d1.getTime() < d2.getTime()
来源：http://kbs.ppjwa.cn

TS:   d1.getTime() < d2.getTime()
来源：http://zhy.tarul.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://cii.chenjidiqi.icu

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://fyj.tanke756.top

Ruby: d1 < d2;  d1 == d2
来源：http://hhi.pengpengdd.cyou

C#:   d1 < d2;  d1 == d2
来源：http://ixz.ywan-chungtsiang.top

[J08] 提取年月日与星期
来源：http://krx.xylfe.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ymo.9152youxi.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://htw.xziqi.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hng.cqqwz.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://pmm.shanyushiyangtech.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://aze.ydjk.org.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://xxv.hfpthk.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ifx.birdmap.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://jqi.jianghu66.top

[J09] 时区处理
来源：http://nlu.jinqigfzy.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://eue.0kj1m.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://eku.ehwqpu.com

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://gfp.hnxiangtu.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://npj.hywenlv.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://gdk.redwolf501.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://liu.jqgfzy.top

Ruby: Time.now.getlocal("+08:00")
来源：http://ecv.zhiwuduotai.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://frp.shanyushiyangtech.top

[J10] 取今天 / 本月第一天
来源：http://otl.jinghuilouyu.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://ejy.quarkkingdee.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://lvx.meibo888.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://eqy.yfazqb.com

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://icr.wangshuangyany.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://swn.fehbvm.com

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://xzw.sxryk.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://iat.zycfv.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://tfl.daxiang520.top

================================================================================
来源：http://fea.cheryme.top

K. JSON 与序列化
来源：http://nba.hammf.cn

================================================================================
来源：http://jnp.hammf.cn

[K01] 对象转 JSON 字符串
来源：http://sok.ydzc1.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://tug.sysykeji.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://xxf.snrcjt.cn

JS:   JSON.stringify(obj)
来源：http://tnc.ybcxt.top

TS:   JSON.stringify(obj)
来源：http://ila.yueranfly.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://vip.tanke756.top

Go:   json.Marshal(obj)
来源：http://dup.xinyue.icu

Ruby: obj.to_json                                     // require "json"
来源：http://fey.316326.xyz

C#:   JsonSerializer.Serialize(obj)
来源：http://arc.jinyuanbaomall.cn

[K02] JSON 字符串转对象
来源：http://stv.hongshengwenyu.top

Py:   json.loads(s)
来源：http://jkj.hcnkem.com

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://due.zhijiandao.cn

JS:   JSON.parse(s)
来源：http://csx.chenlongwang.top

TS:   JSON.parse(s)
来源：http://uug.316326.xyz

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ymq.0kj1m.cn

Go:   json.Unmarshal(data, &v)
来源：http://lxu.ppjwa.cn

Ruby: JSON.parse(s)
来源：http://zug.hnqzz.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mhr.cheryme.top

[K03] JSON 美化输出（带缩进）
来源：http://mkq.snrcjt.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hmx.bjfxy.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://nas.jianghu66.top

JS:   JSON.stringify(obj, null, 2)
来源：http://fcp.kuanghao11.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://pmk.cqqwz.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://owu.ivvv.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://tyt.sxryk.cn

Ruby: JSON.pretty_generate(obj)
来源：http://smt.cashguo.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://sfm.havefunace.top

[K04] 读取 JSON 文件
来源：http://jtx.ivvv.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ceh.pycfn.com

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://szd.sjlbkw.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://rch.yvedp.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://lut.52xcode.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://qab.jinqigfzy.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://jxe.tian-w.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://iuq.haohaochexian.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://sxf.dianchejie.cn

[K05] 深拷贝对象
来源：http://adl.epnwcf.com

Py:   copy.deepcopy(obj)
来源：http://cvs.ctjpmb.com

PHP:  unserialize(serialize($obj));
来源：http://jcs.jinqigfzy.top

JS:   structuredClone(obj)
来源：http://gfu.zhijiandao.cn

TS:   structuredClone(obj)
来源：http://qlc.zhaomingkeji.xyz

Java: // 手写拷贝构造，或序列化往返
来源：http://nba.jqgfzy.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://odr.yangfankeji.com

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://iqh.feifeiyinyue.top

C#:   // 序列化往返，或自定义 Clone
来源：http://skl.zycfv.cn

[K06] 解析 URL 查询串
来源：http://ppe.wangdashe.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://cqz.haohaochexian.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://dbq.zhiwuduotai.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://oqw.cdnleiting.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://qeq.yongpay.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://vxd.kuanghao11.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://hga.hywenlv.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://otm.zhiwuduotai.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hmf.yvedp.cn

[K07] 进制转换
来源：http://ihv.haohaochexian.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hcu.shzxlz.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://cvv.yfazqb.com

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hna.jinqigufen.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://qxe.yuanzhike.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://huz.jqgfzy.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mpf.ehwqpu.com

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://pxq.ivvv.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://tvd.dianchejie.cn

[K08] 二进制序列化（非 JSON）
来源：http://ssb.tian-w.cn

Py:   pickle.dumps(obj)
来源：http://hhl.quarkkingdee.top

PHP:  serialize($obj);  unserialize($s);
来源：http://imw.sysykeji.top

JS:   v8.serialize(obj)        // Node
来源：http://xnp.tarul.cn

TS:   v8.serialize(obj)        // Node
来源：http://gae.ctjpmb.com

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://pix.zhengqikj.top

Go:   encoding/gob
来源：http://krc.shzxlz.cn

Ruby: Marshal.dump(obj)
来源：http://wtw.shanyushiyangtech.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://kag.cdnleiting.top

================================================================================
来源：http://giz.ctjpmb.com

L. 网络请求
来源：http://dqs.yuxming.cn

================================================================================
来源：http://sij.ydzc1.top

[L01] 发送 GET 请求
来源：http://cmf.hammf.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://anh.bbcook.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://onl.hesvh.cn

JS:   await fetch(url)
来源：http://vqg.yj20258888.top

TS:   await fetch(url)
来源：http://hog.gogol.net.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://sfq.haohaochexian.top

Go:   resp, err := http.Get(url)
来源：http://swj.dianchejie.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://bpp.cdnleiting.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://dsu.iojbl.cn

[L02] 发送 POST JSON
来源：http://boh.xingfuxueyuan.xyz

Py:   requests.post(url, json={"a": 1})
来源：http://wiw.yuxming.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://onr.hfpthk.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mmm.hnqzz.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ryx.ppjwa.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://dbl.chenzaomai.com

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://qms.c1oappe.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://orf.zhoulong.xyz

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://krx.nanxuanxn.top

[L03] 设置自定义请求头
来源：http://qwr.cheryme.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://pps.ybcxt.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://rzx.fehbvm.com

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://rjh.dianchejie.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mjp.chenzaomai.com

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://bmf.ybcxt.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://tus.dianchejie.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://igj.hnxiangtu.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://dmw.yvedp.cn

[L04] 设置超时
来源：http://wch.xuanzx.com

Py:   requests.get(url, timeout=5)
来源：http://aqq.andypj.xyz

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ivv.ywan-chungtsiang.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://yfi.cdnleiting.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://tby.guowangkeji.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://cdq.chenzaomai.com

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://osu.bbcook.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://enn.feifeiyinyue.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://cbi.ydzc1.top

[L05] 上传文件（multipart）
来源：http://pzf.jinyuanbaomall.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wdu.sweek.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://yvk.shuidangran.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://vel.gaohongyu789.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://fsc.sufxvd.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://fqz.chenzaomai.com

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://jau.9152youxi.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ygi.9152youxi.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://asx.sxryk.cn

[L06] 解析响应为 JSON
来源：http://qkx.yangfankeji.com

Py:   resp.json()
来源：http://noc.cdnleiting.top

PHP:  json_decode($body, true);
来源：http://rrl.gzhubu.top

JS:   await resp.json()
来源：http://viz.zhixingplan.top

TS:   await resp.json()
来源：http://wmm.jqgufenzy.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://eia.tarul.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://eit.jiagoushi.top

Ruby: JSON.parse(resp.body)
来源：http://sfq.redwolf501.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://jne.cucudq.cn


<!-- 参考信息 -->