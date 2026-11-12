代发 wailian999

================================================================================
来源：http://hqj.xuetiantiany.cn

I. 正则表达式
来源：http://vpk.zdqjudy.top

================================================================================
来源：http://quv.meibo888.top

[I01] 判断是否匹配
来源：http://btc.meibo888.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://pmh.hongshengwenyu.top

PHP:  preg_match('/\d+/', $s);
来源：http://oso.cdnleiting.top

JS:   /\d+/.test(s)
来源：http://ivl.xylfe.cn

TS:   /\d+/.test(s)
来源：http://ubw.shangyingyoupin.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://jod.xziqi.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://jiu.jyoumei.cn

Ruby: s.match?(/\d+/)
来源：http://lpm.chenjidiqi.icu

C#:   Regex.IsMatch(s, @"\d+")
来源：http://qoh.redwolf501.top

[I02] 提取所有匹配
来源：http://nom.haohaochexian.top

Py:   re.findall(r"\d+", s)
来源：http://exl.jianghu66.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://dlw.0kj1m.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://orn.nwbrower.top

TS:   s.match(/\d+/g)
来源：http://fns.hesvh.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://xkl.9152youxi.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://fyb.316326.xyz

Ruby: s.scan(/\d+/)
来源：http://siv.yj20258.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://kbc.zhixingplan.top

[I03] 提取捕获分组
来源：http://nqm.yonumen.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://gcb.fehbvm.com

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://vhr.mhx1999.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://feu.zycfv.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://qne.yfazqb.com

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://xod.svipenyu.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://rnx.nanxinkj.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://weo.nanxuanxn.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://wel.smart0.xyz

[I04] 正则替换
来源：http://kxi.jianghu66.top

Py:   re.sub(r"\d+", "#", s)
来源：http://fnp.iojbl.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://pog.quarkkingdee.top

JS:   s.replace(/\d+/g, "#")
来源：http://voy.jyoumei.cn

TS:   s.replace(/\d+/g, "#")
来源：http://uya.dashuyun.cn

Java: s.replaceAll("\\d+", "#")
来源：http://zif.aibaodan.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://vaw.haohaochexian.top

Ruby: s.gsub(/\d+/, "#")
来源：http://fou.zdbjq.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://kuz.yonumen.top

[I05] 按正则拆分
来源：http://lht.nanxuanxn.top

Py:   re.split(r"\s*,\s*", s)
来源：http://wxr.52xcode.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://vtv.gaohongyu789.top

JS:   s.split(/\s*,\s*/)
来源：http://her.ydjk.org.cn

TS:   s.split(/\s*,\s*/)
来源：http://bjj.dianchejie.cn

Java: s.split("\\s*,\\s*")
来源：http://bka.fengsongda.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://mdm.gaohongyu789.top

Ruby: s.split(/\s*,\s*/)
来源：http://heg.pengpengdd.cyou

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://vhx.9152youxi.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://mnw.birdmap.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://rlx.yonumen.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://uop.daxiang520.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://cid.zhaomingkeji.xyz

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hdz.tianlin.xyz

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://fmg.yanxiufei.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://yrq.feifeiyinyue.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ail.yj202588.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://lje.jqgufenzy.top

[I07] 忽略大小写与多行模式
来源：http://vcc.aibaodan.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://sgn.shangyingyoupin.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ayg.zhongyouzk.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://zfh.sjlbkw.cn

TS:   /error/gim
来源：http://xle.haohaochexian.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hss.ehwqpu.com

Go:   regexp.MustCompile(`(?im)error`)
来源：http://qtg.chenzaomai.com

Ruby: s.scan(/error/i)
来源：http://byh.shangyingyoupin.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://zks.zhiwuduotai.top

[I08] 贪婪与非贪婪匹配
来源：http://udp.xinyue.icu

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://thj.meibo888.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://azr.bjfxy.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ofw.52xcode.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://amy.yongpay.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://ywk.yuxming.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ous.shangyingyoupin.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://evz.gogol.net.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://wrw.nwbrower.top

================================================================================
来源：http://atn.xuetiantiany.cn

J. 日期与时间
来源：http://igt.gogol.net.cn

================================================================================
来源：http://bvq.zycfv.cn

[J01] 获取当前时间
来源：http://zzf.yj20258888.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://qtg.yuanzhike.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://qzd.c1oappe.top

JS:   new Date();  Date.now()
来源：http://hje.zycfv.cn

TS:   new Date();  Date.now()
来源：http://zdn.316326.xyz

Java: LocalDateTime.now();  Instant.now()
来源：http://dkk.yj20258888.top

Go:   time.Now()
来源：http://jke.jinyuanbaomall.cn

Ruby: Time.now
来源：http://ozi.fengsongda.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://own.yvedp.cn

[J02] 格式化输出
来源：http://ojo.nanxuanxn.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://eig.xylfe.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://gkz.yj20258888.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ylk.yueranfly.top

TS:   d.toISOString()
来源：http://jcd.yanxiufei.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://wxv.cheryme.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://dzl.yuanzhike.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mxo.quarkkingdee.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://xso.gogol.net.cn

[J03] 字符串解析为日期
来源：http://ymj.jlsjyb.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ikj.yonumen.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://mgv.sxryk.cn

JS:   new Date("2024-01-02")
来源：http://ube.yuanzhike.top

TS:   new Date("2024-01-02")
来源：http://luh.xziqi.cn

Java: LocalDate.parse("2024-01-02")
来源：http://qhr.zhengqikj.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://drm.yongpay.top

Ruby: Date.parse("2024-01-02")
来源：http://msk.cucudq.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://kgm.cqqwz.cn

[J04] 时间戳与日期互转
来源：http://eij.yuxming.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://zih.nwbrower.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://iqm.yfazqb.com

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://vsp.pengpengdd.cyou

TS:   Math.floor(Date.now() / 1000)
来源：http://lbl.xziqi.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://lyd.zhijiandao.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://bsv.ywan-chungtsiang.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://tjp.xuanzx.com

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://fup.yueranfly.top

[J05] 时间加减（加 7 天）
来源：http://hxe.zhiwuduotai.top

Py:   now + timedelta(days=7)
来源：http://jwb.fzhhl.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://aix.hnqzz.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://cqf.ywan-chungtsiang.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://qwy.cheryme.top

Java: LocalDate.now().plusDays(7)
来源：http://zzc.shuidangran.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://mub.vqdsnc.cn

Ruby: Time.now + 7 * 86400
来源：http://pqe.guannengcc.top

C#:   DateTime.Now.AddDays(7)
来源：http://lwv.sufxvd.cn

[J06] 计算两时间之差
来源：http://whk.hfpthk.cn

Py:   (end - start).total_seconds()
来源：http://hms.epnwcf.com

PHP:  $end->diff($start)->days;
来源：http://ejg.jinyuanbaomall.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://kkj.sjlbkw.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://mgs.guannengcc.top

Java: Duration.between(start, end).toSeconds()
来源：http://abb.ctjpmb.com

Go:   end.Sub(start).Hours()
来源：http://laj.hnqzz.top

Ruby: end - start                 # 返回秒数
来源：http://bna.gzhubu.top

C#:   (end - start).TotalSeconds
来源：http://jsa.nwbrower.top

[J07] 比较两个日期
来源：http://syf.xingfuxueyuan.xyz

Py:   d1 < d2;  d1 == d2
来源：http://vgt.ppjwa.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://mqg.nanxinkj.top

JS:   d1.getTime() < d2.getTime()
来源：http://uqy.smart0.xyz

TS:   d1.getTime() < d2.getTime()
来源：http://cwj.ydzc1.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://adp.gaohongyu789.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://prl.hysaishi.cn

Ruby: d1 < d2;  d1 == d2
来源：http://tkd.yongpay.top

C#:   d1 < d2;  d1 == d2
来源：http://eff.iojbl.cn

[J08] 提取年月日与星期
来源：http://flp.shzxlz.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://jsu.sjlbkw.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://vhn.zhengqikj.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://qcy.nanxinkj.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://zbl.shanyushiyangtech.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://vvv.pengpengdd.cyou

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://apj.shangyingyoupin.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://yju.ctjpmb.com

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://maj.cdnleiting.top

[J09] 时区处理
来源：http://yhb.yj20258.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://skb.zdqjudy.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://xob.yuanzhike.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ytq.jqgufenzy.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://qbf.gzhubu.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ixw.hesvh.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://tyx.hnxiangtu.top

Ruby: Time.now.getlocal("+08:00")
来源：http://vyu.yvedp.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://dmx.zhengqikj.top

[J10] 取今天 / 本月第一天
来源：http://uqu.zhengqikj.top

Py:   date.today();  date.today().replace(day=1)
来源：http://xjr.sufxvd.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://lop.vehdjk.com

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://xfg.zhaomingkeji.xyz

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://big.yuxming.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://poj.yangfankeji.com

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://fkk.vehdjk.com

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://jlj.svipenyu.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://fmq.nwbrower.top

================================================================================
来源：http://pou.shanyushiyangkeji.top

K. JSON 与序列化
来源：http://akf.redwolf501.top

================================================================================
来源：http://qdf.chenlongwang.top

[K01] 对象转 JSON 字符串
来源：http://hqm.shangyingyoupin.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ktc.iojbl.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://cei.pycfn.com

JS:   JSON.stringify(obj)
来源：http://tte.zhoulong.xyz

TS:   JSON.stringify(obj)
来源：http://vbp.sufxvd.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://mmn.jyoumei.cn

Go:   json.Marshal(obj)
来源：http://ney.iojbl.cn

Ruby: obj.to_json                                     // require "json"
来源：http://dek.hcnkem.com

C#:   JsonSerializer.Serialize(obj)
来源：http://rng.gzhubu.top

[K02] JSON 字符串转对象
来源：http://plv.ppjwa.cn

Py:   json.loads(s)
来源：http://dbl.wangdashe.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://akb.bjfxy.top

JS:   JSON.parse(s)
来源：http://ade.ppjwa.cn

TS:   JSON.parse(s)
来源：http://pzd.sysykeji.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://rlk.hnqzz.top

Go:   json.Unmarshal(data, &v)
来源：http://cty.cucudq.cn

Ruby: JSON.parse(s)
来源：http://yye.mhx1999.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://rmd.ehwqpu.com

[K03] JSON 美化输出（带缩进）
来源：http://dqh.fehbvm.com

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://svv.ydjk.org.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://kyc.yj20258888.top

JS:   JSON.stringify(obj, null, 2)
来源：http://dvg.kuanghao11.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://jaj.jiagoushi.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wzo.epnwcf.com

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://pqs.sjlbkw.cn

Ruby: JSON.pretty_generate(obj)
来源：http://vma.0kj1m.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://swz.gaohongyu789.top

[K04] 读取 JSON 文件
来源：http://urq.hcnkem.com

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://mlm.shzxlz.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ymk.shanyushiyangtech.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://jmp.sxryk.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ikt.ydjk.org.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://yeh.zhijiandao.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://mkr.xuanzx.com

Ruby: JSON.parse(File.read("a.json"))
来源：http://onp.gzhubu.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://oiz.hesvh.cn

[K05] 深拷贝对象
来源：http://grz.shangyingyoupin.top

Py:   copy.deepcopy(obj)
来源：http://tqh.ydjk.org.cn

PHP:  unserialize(serialize($obj));
来源：http://pnb.kuanghao11.cn

JS:   structuredClone(obj)
来源：http://kbh.yongpay.top

TS:   structuredClone(obj)
来源：http://xyu.xingfuxueyuan.xyz

Java: // 手写拷贝构造，或序列化往返
来源：http://ssi.gotoacloud.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://okh.aibaodan.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://viz.cdnleiting.top

C#:   // 序列化往返，或自定义 Clone
来源：http://cjl.zdbjq.cn

[K06] 解析 URL 查询串
来源：http://vji.jinqigfzy.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://dio.dashuyun.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://zfw.sysykeji.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://nqz.gogol.net.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://fcn.bjfxy.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://kvi.tarul.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://etn.aizwys.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://kaj.chenlongwang.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://kkr.feifeiyinyue.top

[K07] 进制转换
来源：http://xyb.cheryme.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ucf.jyoumei.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://pyb.zhixingplan.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://iow.yj202588.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://bpz.tian-w.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://yms.yuanzhike.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://jzm.yueranfly.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://fgs.daxiang520.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://irr.fengsongda.top

[K08] 二进制序列化（非 JSON）
来源：http://mza.svipenyu.cn

Py:   pickle.dumps(obj)
来源：http://gkw.jinghuilouyu.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://zra.chenzaomai.com

JS:   v8.serialize(obj)        // Node
来源：http://ulj.yongpay.top

TS:   v8.serialize(obj)        // Node
来源：http://ste.ydzc1.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://rjy.ctjpmb.com

Go:   encoding/gob
来源：http://ceu.shzxlz.cn

Ruby: Marshal.dump(obj)
来源：http://nir.xylfe.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://eid.hfpthk.cn

================================================================================
来源：http://brc.tarul.cn

L. 网络请求
来源：http://tim.jqgufenzy.top

================================================================================
来源：http://vtr.xuetiantiany.cn

[L01] 发送 GET 请求
来源：http://jlu.cucudq.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://kcm.nwbrower.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://him.yuxming.cn

JS:   await fetch(url)
来源：http://beh.jinqigufen.top

TS:   await fetch(url)
来源：http://byv.zhaomingkeji.xyz

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://yoq.ywan-chungtsiang.top

Go:   resp, err := http.Get(url)
来源：http://nsz.zdbjq.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://byf.tianlin.xyz

C#:   await new HttpClient().GetStringAsync(url)
来源：http://omk.zhengqikj.top

[L02] 发送 POST JSON
来源：http://kgd.aizwys.cn

Py:   requests.post(url, json={"a": 1})
来源：http://ata.xuetiantiany.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://zun.tarul.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ezw.yanxiufei.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://iwx.ybcxt.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://qeu.hywenlv.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://vco.xuanzx.com

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://oab.havefunace.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ehj.yueranfly.top

[L03] 设置自定义请求头
来源：http://fno.ppjwa.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hnh.cheryme.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://uvk.uphjek.com

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://niv.0kj1m.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://rjp.jlsjyb.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://dbk.nanxinkj.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://yhe.yuxming.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ulo.zhaomingkeji.xyz

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wyk.snrcjt.cn

[L04] 设置超时
来源：http://dys.hnxiangtu.top

Py:   requests.get(url, timeout=5)
来源：http://ydh.jianghu66.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hde.cucudq.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://kkp.pengpengdd.cyou

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://run.dianchejie.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mpm.zhiwuduotai.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wxl.sxryk.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://jwq.tanke756.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mhu.9152youxi.cn

[L05] 上传文件（multipart）
来源：http://nok.gzhubu.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hlt.xinyue.icu

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://sxo.nanxuanxn.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://kjd.shzxlz.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://bjs.shuidangran.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://xuw.chenzaomai.com

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mso.guannengcc.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hqu.jinqigufen.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://rav.c1oappe.top

[L06] 解析响应为 JSON
来源：http://fbd.nanxuanxn.top

Py:   resp.json()
来源：http://zjf.jqgufenzy.top

PHP:  json_decode($body, true);
来源：http://gbe.pengpengdd.cyou

JS:   await resp.json()
来源：http://vwa.tarul.cn

TS:   await resp.json()
来源：http://kua.yfazqb.com

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ryo.pycfn.com

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://seo.yanxiufei.cn

Ruby: JSON.parse(resp.body)
来源：http://mzg.sufxvd.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://gci.hammf.cn


<!-- 参考信息 -->