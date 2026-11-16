代发 wailian999

Py:   with open("a.txt") as f: data = f.read()
来源：http://mnq.dianchejie.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://fka.gaohongyu789.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://owg.xingfuxueyuan.xyz

TS:   // 无 with：在 finally 里关闭句柄
来源：http://syj.hesvh.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://aga.sjlbkw.cn

Go:   defer f.Close()
来源：http://yxf.jqgufenzy.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://rtw.ydzc1.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://vex.zhixingplan.top

================================================================================
来源：http://pxu.feifeiyinyue.top

I. 正则表达式
来源：http://jcu.zhaomingkeji.xyz

================================================================================
来源：http://pwx.ydjk.org.cn

[I01] 判断是否匹配
来源：http://imo.guowangkeji.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://mjx.tarul.cn

PHP:  preg_match('/\d+/', $s);
来源：http://rmv.aizwys.cn

JS:   /\d+/.test(s)
来源：http://wgg.cashguo.top

TS:   /\d+/.test(s)
来源：http://maj.pycfn.com

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://mbi.jinqigfzy.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://qvc.jianghu66.top

Ruby: s.match?(/\d+/)
来源：http://ltb.snrcjt.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://etl.yuanzhike.top

[I02] 提取所有匹配
来源：http://qtq.zhongyouzk.top

Py:   re.findall(r"\d+", s)
来源：http://adn.fengsongda.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://adt.shangyingyoupin.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://xoo.feifeiyinyue.top

TS:   s.match(/\d+/g)
来源：http://ysm.xuanzx.com

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://rlm.xingfuxueyuan.xyz

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://kwj.52xcode.cn

Ruby: s.scan(/\d+/)
来源：http://itp.tarul.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://noo.yuanzhike.top

[I03] 提取捕获分组
来源：http://ziy.yueranfly.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ucz.zhongyouzk.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://xem.fengsongda.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://yow.jinyuanbaomall.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ygb.fengsongda.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://wzw.birdmap.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hvb.yuxming.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ntc.sysykeji.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://bjd.hywenlv.cn

[I04] 正则替换
来源：http://tce.hnqzz.top

Py:   re.sub(r"\d+", "#", s)
来源：http://axf.gaohongyu789.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://vag.cheryme.top

JS:   s.replace(/\d+/g, "#")
来源：http://omt.ywan-chungtsiang.top

TS:   s.replace(/\d+/g, "#")
来源：http://ztf.shuidangran.top

Java: s.replaceAll("\\d+", "#")
来源：http://tsj.chenjidiqi.icu

Go:   re.ReplaceAllString(s, "#")
来源：http://qaz.yueranfly.top

Ruby: s.gsub(/\d+/, "#")
来源：http://lcw.yonumen.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://bkw.nanxuanxn.top

[I05] 按正则拆分
来源：http://rvz.fzhhl.top

Py:   re.split(r"\s*,\s*", s)
来源：http://aqm.sufxvd.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://exc.fanxiaobao.xyz

JS:   s.split(/\s*,\s*/)
来源：http://jan.ywan-chungtsiang.top

TS:   s.split(/\s*,\s*/)
来源：http://oyb.hcnkem.com

Java: s.split("\\s*,\\s*")
来源：http://nwh.mhx1999.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hbs.cucudq.cn

Ruby: s.split(/\s*,\s*/)
来源：http://jyi.yj20258888.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://qab.hammf.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://aji.yfazqb.com

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://iic.epnwcf.com

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ott.quarkkingdee.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://yhb.sufxvd.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://xuh.jinghuilouyu.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://gbc.nwbrower.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://gpw.jqgfzy.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://vxw.snrcjt.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://bst.ivvv.top

[I07] 忽略大小写与多行模式
来源：http://enc.xziqi.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://anb.hcnkem.com

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://plh.andypj.xyz

JS:   /error/gim；new RegExp("error", "gim")
来源：http://wlc.yuanzhike.top

TS:   /error/gim
来源：http://dwu.shangyingyoupin.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://emu.feifeiyinyue.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://fut.chenjidiqi.icu

Ruby: s.scan(/error/i)
来源：http://vwi.feifeiyinyue.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://bml.gotoacloud.top

[I08] 贪婪与非贪婪匹配
来源：http://nmf.hnxiangtu.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://bgd.yonumen.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://sbu.feifeiyinyue.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ewn.ydjk.org.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://csc.tian-w.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://gtp.feifeiyinyue.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://syk.yfazqb.com

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://omw.pengpengdd.cyou

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://djb.ehwqpu.com

================================================================================
来源：http://sgg.vehdjk.com

J. 日期与时间
来源：http://hkp.c1oappe.top

================================================================================
来源：http://koc.tanke756.top

[J01] 获取当前时间
来源：http://tpy.zycfv.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://nkj.zhengqikj.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://neg.cashguo.top

JS:   new Date();  Date.now()
来源：http://gmh.feifeiyinyue.top

TS:   new Date();  Date.now()
来源：http://kyb.xingfuxueyuan.xyz

Java: LocalDateTime.now();  Instant.now()
来源：http://rld.ivvv.top

Go:   time.Now()
来源：http://uzb.tarul.cn

Ruby: Time.now
来源：http://fcz.bjfxy.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://mwb.cucudq.cn

[J02] 格式化输出
来源：http://qly.haohaochexian.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://zkf.gotoacloud.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://gos.vqdsnc.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://vvt.jinghuilouyu.cn

TS:   d.toISOString()
来源：http://pnw.epnwcf.com

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://geo.birdmap.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://blt.bbcook.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://frl.fktsv.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://cid.svipenyu.cn

[J03] 字符串解析为日期
来源：http://pll.316326.xyz

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://kda.tarul.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://njq.c1oappe.top

JS:   new Date("2024-01-02")
来源：http://uir.iojbl.cn

TS:   new Date("2024-01-02")
来源：http://pok.fanxiaobao.xyz

Java: LocalDate.parse("2024-01-02")
来源：http://lyh.ppjwa.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://pjo.daria6918.cn

Ruby: Date.parse("2024-01-02")
来源：http://shr.ybcxt.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ews.mhx1999.top

[J04] 时间戳与日期互转
来源：http://hqa.ydzc1.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hqg.quarkkingdee.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ioh.smart0.xyz

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ztx.hnqzz.top

TS:   Math.floor(Date.now() / 1000)
来源：http://qix.yongpay.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://tzd.fzhhl.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://oxr.jqgfzy.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://tva.xinyue.icu

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hzy.xuetiantiany.cn

[J05] 时间加减（加 7 天）
来源：http://jao.wangshuangyany.cn

Py:   now + timedelta(days=7)
来源：http://hfl.quarkkingdee.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://qim.zdqjudy.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://qvt.jqgufenzy.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://vdg.yangfankeji.com

Java: LocalDate.now().plusDays(7)
来源：http://rzw.hnqzz.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://pel.sjlbkw.cn

Ruby: Time.now + 7 * 86400
来源：http://xwh.ydzc1.top

C#:   DateTime.Now.AddDays(7)
来源：http://qqb.kuanghao11.cn

[J06] 计算两时间之差
来源：http://xdd.gogol.net.cn

Py:   (end - start).total_seconds()
来源：http://lgn.chenlongwang.top

PHP:  $end->diff($start)->days;
来源：http://jak.jqgfzy.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://gqw.sweek.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://czd.jiagoushi.top

Java: Duration.between(start, end).toSeconds()
来源：http://yik.zhiwuduotai.top

Go:   end.Sub(start).Hours()
来源：http://kyo.hcnkem.com

Ruby: end - start                 # 返回秒数
来源：http://ghh.birdmap.top

C#:   (end - start).TotalSeconds
来源：http://ldc.jinyuanbaomall.cn

[J07] 比较两个日期
来源：http://wam.hcnkem.com

Py:   d1 < d2;  d1 == d2
来源：http://wju.mhx1999.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://cgh.fengsongda.top

JS:   d1.getTime() < d2.getTime()
来源：http://pbb.shangyingyoupin.top

TS:   d1.getTime() < d2.getTime()
来源：http://avc.shuidangran.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://aha.zhengqikj.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ker.shzxlz.cn

Ruby: d1 < d2;  d1 == d2
来源：http://rlp.hnxiangtu.top

C#:   d1 < d2;  d1 == d2
来源：http://uno.gzhubu.top

[J08] 提取年月日与星期
来源：http://igg.ppjwa.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://xfl.ybcxt.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://yjb.cqqwz.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://nhm.xuetiantiany.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://aqn.c1oappe.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hyh.fengsongda.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://tcp.chenlongwang.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://iuo.jqgufenzy.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://tee.xuetiantiany.cn

[J09] 时区处理
来源：http://kyp.jinqigfzy.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://waz.xziqi.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://com.sweek.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://stz.mhx1999.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://lgm.sxryk.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ozy.52xcode.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://lyd.wangdashe.top

Ruby: Time.now.getlocal("+08:00")
来源：http://whh.shanyushiyangtech.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://qoj.birdmap.top

[J10] 取今天 / 本月第一天
来源：http://fec.fengsongda.top

Py:   date.today();  date.today().replace(day=1)
来源：http://plb.kuanghao11.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://jla.nwbrower.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://qlh.ppjwa.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://pjr.yonumen.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://cjh.shanyushiyangkeji.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://iiw.0kj1m.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://akb.jyoumei.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://fju.ydzc1.top

================================================================================
来源：http://klj.iojbl.cn

K. JSON 与序列化
来源：http://zzq.gzhubu.top

================================================================================
来源：http://jol.yj202588.top

[K01] 对象转 JSON 字符串
来源：http://jxk.gzhubu.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://lzb.shzxlz.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://buq.jinyuanbaomall.cn

JS:   JSON.stringify(obj)
来源：http://hyz.chenlongwang.top

TS:   JSON.stringify(obj)
来源：http://efv.dianchejie.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://rpg.nanxinkj.top

Go:   json.Marshal(obj)
来源：http://mos.fengsongda.top

Ruby: obj.to_json                                     // require "json"
来源：http://pfh.ydjk.org.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://ooc.ehwqpu.com

[K02] JSON 字符串转对象
来源：http://itv.jyoumei.cn

Py:   json.loads(s)
来源：http://dzp.316326.xyz

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://dtx.nwbrower.top

JS:   JSON.parse(s)
来源：http://irl.yj20258.top

TS:   JSON.parse(s)
来源：http://cis.svipenyu.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://lyc.0kj1m.cn

Go:   json.Unmarshal(data, &v)
来源：http://xqd.yj20258888.top

Ruby: JSON.parse(s)
来源：http://xte.shanyushiyangtech.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://vdc.jyoumei.cn

[K03] JSON 美化输出（带缩进）
来源：http://clj.bbcook.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://tnt.gzhubu.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://lyx.zhoulong.xyz

JS:   JSON.stringify(obj, null, 2)
来源：http://uxx.jinghuilouyu.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://oil.nanxinkj.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://acj.yfazqb.com

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://lnx.sysykeji.top

Ruby: JSON.pretty_generate(obj)
来源：http://njx.guowangkeji.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://awc.havefunace.top

[K04] 读取 JSON 文件
来源：http://xwx.316326.xyz

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ckx.andypj.xyz

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://zfi.yangfankeji.com

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ddk.guannengcc.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://app.yj20258888.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://zit.sweek.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://num.jqgufenzy.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://kbb.zhijiandao.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://xht.cashguo.top

[K05] 深拷贝对象
来源：http://tta.hesvh.cn

Py:   copy.deepcopy(obj)
来源：http://yez.zhengqikj.top

PHP:  unserialize(serialize($obj));
来源：http://cxb.yueranfly.top

JS:   structuredClone(obj)
来源：http://byw.gogol.net.cn

TS:   structuredClone(obj)
来源：http://hdv.wangdashe.top

Java: // 手写拷贝构造，或序列化往返
来源：http://eca.chenlongwang.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wfy.ivvv.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://sqz.fehbvm.com

C#:   // 序列化往返，或自定义 Clone
来源：http://ofx.hongshengwenyu.top

[K06] 解析 URL 查询串
来源：http://efd.bjfxy.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://pgo.aibaodan.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://dyy.fengsongda.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://aqn.yj20258.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://jpm.hcnkem.com

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://imb.gzhubu.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://kty.havefunace.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://zlx.redwolf501.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://blc.sweek.top

[K07] 进制转换
来源：http://dlq.jiagoushi.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://soh.mhx1999.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://gpe.52xcode.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://lza.hongshengwenyu.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://kll.bbcook.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://rxu.jianghu66.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://qgy.zhengqikj.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mup.dianchejie.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://gzy.cheryme.top

[K08] 二进制序列化（非 JSON）
来源：http://hso.vqdsnc.cn

Py:   pickle.dumps(obj)
来源：http://yrj.chenlongwang.top

PHP:  serialize($obj);  unserialize($s);
来源：http://leq.shangyingyoupin.top

JS:   v8.serialize(obj)        // Node
来源：http://orp.zhiwuduotai.top

TS:   v8.serialize(obj)        // Node
来源：http://dfb.pycfn.com

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ggb.yfazqb.com

Go:   encoding/gob
来源：http://law.sxryk.cn

Ruby: Marshal.dump(obj)
来源：http://hln.cashguo.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://dym.nwbrower.top

================================================================================
来源：http://mjw.wangdashe.top

L. 网络请求
来源：http://akl.tanke756.top

================================================================================
来源：http://mtw.zhengqikj.top

[L01] 发送 GET 请求
来源：http://ikm.gzhubu.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://xwy.tarul.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://vpx.yj20258.top

JS:   await fetch(url)
来源：http://qus.bjfxy.top

TS:   await fetch(url)
来源：http://dlq.daria6918.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://xfz.chenzaomai.com

Go:   resp, err := http.Get(url)
来源：http://iiz.yfazqb.com

Ruby: Net::HTTP.get(URI(url))
来源：http://nzz.zhaomingkeji.xyz

C#:   await new HttpClient().GetStringAsync(url)
来源：http://uxe.iojbl.cn

[L02] 发送 POST JSON
来源：http://fci.tian-w.cn

Py:   requests.post(url, json={"a": 1})
来源：http://lms.birdmap.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ota.ydjk.org.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hlq.hongshengwenyu.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://bul.hongshengwenyu.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://lwd.guowangkeji.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://why.chenjidiqi.icu

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://snk.gotoacloud.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wmq.c1oappe.top

[L03] 设置自定义请求头
来源：http://mfm.shanyushiyangkeji.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://jfo.svipenyu.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://pqp.epnwcf.com

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://rut.yanxiufei.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://vyj.chenlongwang.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://zli.bjfxy.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ypo.gogol.net.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://cyg.jinqigufen.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://qqr.vehdjk.com

[L04] 设置超时
来源：http://wxr.fehbvm.com

Py:   requests.get(url, timeout=5)
来源：http://nxo.ydzc1.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hgy.shzxlz.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hmr.cdnleiting.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://dml.hywenlv.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://eaq.jlsjyb.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://czu.zhixingplan.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://juz.jinqigfzy.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://odt.jinyuanbaomall.cn

[L05] 上传文件（multipart）
来源：http://axz.sysykeji.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://foy.hnqzz.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://rjl.gotoacloud.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://aib.ybcxt.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://rmt.tian-w.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://akp.wangshuangyany.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://eze.smart0.xyz

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://gqf.redwolf501.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://kcz.ydjk.org.cn

[L06] 解析响应为 JSON
来源：http://kcm.xylfe.cn


<!-- 参考信息 -->