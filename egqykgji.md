代发 wailian999

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://eum.gaohongyu789.top

Go:   defer f.Close()
来源：http://mlb.zhaomingkeji.xyz

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ztr.0kj1m.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://bcx.pycfn.com

================================================================================
来源：http://rjo.yj20258.top

I. 正则表达式
来源：http://ruy.hnxiangtu.top

================================================================================
来源：http://tgt.xuanzx.com

[I01] 判断是否匹配
来源：http://csm.aizwys.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://lsf.gotoacloud.top

PHP:  preg_match('/\d+/', $s);
来源：http://hei.gaohongyu789.top

JS:   /\d+/.test(s)
来源：http://oee.yonumen.top

TS:   /\d+/.test(s)
来源：http://glz.fengsongda.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://yev.fanxiaobao.xyz

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://mfv.yj20258888.top

Ruby: s.match?(/\d+/)
来源：http://spf.bjfxy.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://oow.ctjpmb.com

[I02] 提取所有匹配
来源：http://iav.jyoumei.cn

Py:   re.findall(r"\d+", s)
来源：http://tem.xylfe.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://fru.andypj.xyz

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hqr.ywan-chungtsiang.top

TS:   s.match(/\d+/g)
来源：http://oxe.havefunace.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://cvy.zhiwuduotai.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://clg.sxryk.cn

Ruby: s.scan(/\d+/)
来源：http://ofa.nanxuanxn.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://phj.shanyushiyangtech.top

[I03] 提取捕获分组
来源：http://cca.zhixingplan.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://mrf.ydzc1.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://yac.yj202588.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://vyk.jyoumei.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://eph.fktsv.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://cme.hammf.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://owu.yj20258.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://pbp.bbcook.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://qzz.chenjidiqi.icu

[I04] 正则替换
来源：http://wal.smart0.xyz

Py:   re.sub(r"\d+", "#", s)
来源：http://lid.fengsongda.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://npw.hfpthk.cn

JS:   s.replace(/\d+/g, "#")
来源：http://hln.jqgfzy.top

TS:   s.replace(/\d+/g, "#")
来源：http://skg.fanxiaobao.xyz

Java: s.replaceAll("\\d+", "#")
来源：http://ryt.redwolf501.top

Go:   re.ReplaceAllString(s, "#")
来源：http://umt.aibaodan.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://twp.yongpay.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://bue.zhaomingkeji.xyz

[I05] 按正则拆分
来源：http://rhm.hongshengwenyu.top

Py:   re.split(r"\s*,\s*", s)
来源：http://qyk.mhx1999.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://qxt.cheryme.top

JS:   s.split(/\s*,\s*/)
来源：http://vhi.shangyingyoupin.top

TS:   s.split(/\s*,\s*/)
来源：http://ecc.sjlbkw.cn

Java: s.split("\\s*,\\s*")
来源：http://ysl.tanke756.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://fsy.dashuyun.cn

Ruby: s.split(/\s*,\s*/)
来源：http://koz.tanke756.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://qwm.daxiang520.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://fhi.52xcode.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://iix.hcnkem.com

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://yyr.yvedp.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://qmp.jinqigfzy.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ycj.ctjpmb.com

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://bpy.pycfn.com

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://odk.haohaochexian.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://cim.xuanzx.com

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://imz.mhx1999.top

[I07] 忽略大小写与多行模式
来源：http://exv.vqdsnc.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ttz.sufxvd.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://cdg.hesvh.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://neo.hesvh.cn

TS:   /error/gim
来源：http://vci.jinghuilouyu.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://jvo.jqgufenzy.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://vsi.shangyingyoupin.top

Ruby: s.scan(/error/i)
来源：http://jjg.shuidangran.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ccf.sufxvd.cn

[I08] 贪婪与非贪婪匹配
来源：http://aui.bjfxy.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://irr.hywenlv.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://vqc.mhx1999.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://yxe.pengpengdd.cyou

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://fca.zdbjq.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://dbu.aizwys.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://bcb.ydzc1.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://zxl.epnwcf.com

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://czt.yueranfly.top

================================================================================
来源：http://jsa.zhijiandao.cn

J. 日期与时间
来源：http://nzz.jinqigufen.top

================================================================================
来源：http://skm.guannengcc.top

[J01] 获取当前时间
来源：http://vdt.hammf.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://civ.ydjk.org.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://azu.xingfuxueyuan.xyz

JS:   new Date();  Date.now()
来源：http://mjy.yj202588.top

TS:   new Date();  Date.now()
来源：http://vea.9152youxi.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://zjk.bjfxy.top

Go:   time.Now()
来源：http://wsg.wangshuangyany.cn

Ruby: Time.now
来源：http://nyd.tarul.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://sxi.jiagoushi.top

[J02] 格式化输出
来源：http://rer.shuidangran.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://xct.tian-w.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://oyt.316326.xyz

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://dhy.yj202588.top

TS:   d.toISOString()
来源：http://flk.hysaishi.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://znz.fengsongda.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://rdw.hongshengwenyu.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://vwp.jyoumei.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://cci.hongshengwenyu.top

[J03] 字符串解析为日期
来源：http://hkw.ydjk.org.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://jcn.guowangkeji.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://yzx.sufxvd.cn

JS:   new Date("2024-01-02")
来源：http://xhv.sjlbkw.cn

TS:   new Date("2024-01-02")
来源：http://aek.iojbl.cn

Java: LocalDate.parse("2024-01-02")
来源：http://nyc.haohaochexian.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://olc.fehbvm.com

Ruby: Date.parse("2024-01-02")
来源：http://kks.cqqwz.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://aoo.fktsv.cn

[J04] 时间戳与日期互转
来源：http://qps.hnxiangtu.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://vpr.chenzaomai.com

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://oky.fengsongda.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://wlj.birdmap.top

TS:   Math.floor(Date.now() / 1000)
来源：http://eky.cashguo.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://gmu.aizwys.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://yen.xziqi.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://qpv.yongpay.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://njr.chenlongwang.top

[J05] 时间加减（加 7 天）
来源：http://pzh.hnqzz.top

Py:   now + timedelta(days=7)
来源：http://mko.316326.xyz

PHP:  (new DateTime())->modify("+7 days");
来源：http://zyz.hnxiangtu.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://pcj.hywenlv.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://mpj.ctjpmb.com

Java: LocalDate.now().plusDays(7)
来源：http://wvo.ydzc1.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://gkv.c1oappe.top

Ruby: Time.now + 7 * 86400
来源：http://jql.xylfe.cn

C#:   DateTime.Now.AddDays(7)
来源：http://uoe.xingfuxueyuan.xyz

[J06] 计算两时间之差
来源：http://kcw.jlsjyb.cn

Py:   (end - start).total_seconds()
来源：http://sin.yanxiufei.cn

PHP:  $end->diff($start)->days;
来源：http://dty.ybcxt.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://vdn.9152youxi.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://wmv.yongpay.top

Java: Duration.between(start, end).toSeconds()
来源：http://fel.yvedp.cn

Go:   end.Sub(start).Hours()
来源：http://zst.aibaodan.cn

Ruby: end - start                 # 返回秒数
来源：http://pzl.guowangkeji.top

C#:   (end - start).TotalSeconds
来源：http://glv.zhongyouzk.top

[J07] 比较两个日期
来源：http://lxd.yongpay.top

Py:   d1 < d2;  d1 == d2
来源：http://bjz.epnwcf.com

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://wjj.wangdashe.top

JS:   d1.getTime() < d2.getTime()
来源：http://zvu.yuxming.cn

TS:   d1.getTime() < d2.getTime()
来源：http://lrm.aizwys.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://kwh.shangyingyoupin.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://fwe.feifeiyinyue.top

Ruby: d1 < d2;  d1 == d2
来源：http://hyy.jlsjyb.cn

C#:   d1 < d2;  d1 == d2
来源：http://pks.zdqjudy.top

[J08] 提取年月日与星期
来源：http://vwr.cheryme.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://vkl.xziqi.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://vse.yangfankeji.com

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ewo.ywan-chungtsiang.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://yhf.gzhubu.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://wzl.jyoumei.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://vml.jinyuanbaomall.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://shg.bjfxy.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://tuu.ppjwa.cn

[J09] 时区处理
来源：http://rzp.cqqwz.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://rie.chenlongwang.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://win.jqgufenzy.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ccp.shuidangran.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://vfa.cashguo.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://wlq.dianchejie.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://udq.yuanzhike.top

Ruby: Time.now.getlocal("+08:00")
来源：http://xpn.yanxiufei.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://sim.birdmap.top

[J10] 取今天 / 本月第一天
来源：http://czx.nwbrower.top

Py:   date.today();  date.today().replace(day=1)
来源：http://wng.tarul.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://qxx.havefunace.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://rol.smart0.xyz

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://jhe.shanyushiyangtech.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://qrr.jinqigufen.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://efc.tarul.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hio.xuetiantiany.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://syb.sysykeji.top

================================================================================
来源：http://umc.nanxinkj.top

K. JSON 与序列化
来源：http://jfi.yuanzhike.top

================================================================================
来源：http://poo.zhoulong.xyz

[K01] 对象转 JSON 字符串
来源：http://qet.c1oappe.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://irq.hnqzz.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://xop.nanxuanxn.top

JS:   JSON.stringify(obj)
来源：http://yqy.kuanghao11.cn

TS:   JSON.stringify(obj)
来源：http://aew.xuetiantiany.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://xqx.zdqjudy.top

Go:   json.Marshal(obj)
来源：http://zqk.xuanzx.com

Ruby: obj.to_json                                     // require "json"
来源：http://ajc.shanyushiyangkeji.top

C#:   JsonSerializer.Serialize(obj)
来源：http://ypl.shanyushiyangtech.top

[K02] JSON 字符串转对象
来源：http://vyy.chenjidiqi.icu

Py:   json.loads(s)
来源：http://zqr.gaohongyu789.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://xtd.gogol.net.cn

JS:   JSON.parse(s)
来源：http://lyh.xylfe.cn

TS:   JSON.parse(s)
来源：http://kpn.yfazqb.com

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://zbe.yongpay.top

Go:   json.Unmarshal(data, &v)
来源：http://zyr.sysykeji.top

Ruby: JSON.parse(s)
来源：http://ugw.hysaishi.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://snw.gogol.net.cn

[K03] JSON 美化输出（带缩进）
来源：http://bwb.ehwqpu.com

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ydk.guowangkeji.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://egh.jinqigufen.top

JS:   JSON.stringify(obj, null, 2)
来源：http://kmo.pycfn.com

TS:   JSON.stringify(obj, null, 2)
来源：http://epu.zycfv.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://kfp.uphjek.com

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://xtz.yuanzhike.top

Ruby: JSON.pretty_generate(obj)
来源：http://nhs.hammf.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ona.shzxlz.cn

[K04] 读取 JSON 文件
来源：http://xki.ywan-chungtsiang.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hfg.hfpthk.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://yhe.jinyuanbaomall.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://yhc.bbcook.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mwd.nanxinkj.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wdr.shanyushiyangkeji.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://zyl.bbcook.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://fuq.fanxiaobao.xyz

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://pnv.xuetiantiany.cn

[K05] 深拷贝对象
来源：http://nwx.mhx1999.top

Py:   copy.deepcopy(obj)
来源：http://tjm.xziqi.cn

PHP:  unserialize(serialize($obj));
来源：http://tff.ybcxt.top

JS:   structuredClone(obj)
来源：http://ezu.jinghuilouyu.cn

TS:   structuredClone(obj)
来源：http://oky.kuanghao11.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://ynh.cashguo.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hsx.hnqzz.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://xuy.jiagoushi.top

C#:   // 序列化往返，或自定义 Clone
来源：http://ily.9152youxi.cn

[K06] 解析 URL 查询串
来源：http://weh.tarul.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://nab.cucudq.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://fcm.shanyushiyangkeji.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://qtu.smart0.xyz

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://pqs.sxryk.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ieb.xingfuxueyuan.xyz

Go:   url.ParseQuery("a=1&b=2")
来源：http://age.yj20258.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://zvf.wangdashe.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://xvd.chenlongwang.top

[K07] 进制转换
来源：http://ash.sxryk.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://uzb.jqgufenzy.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://qyw.sufxvd.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://wbm.havefunace.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://eqx.jinghuilouyu.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ipu.fanxiaobao.xyz

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://cxj.zhengqikj.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://vto.gzhubu.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://gnz.ctjpmb.com

[K08] 二进制序列化（非 JSON）
来源：http://vvk.nanxinkj.top

Py:   pickle.dumps(obj)
来源：http://ara.yfazqb.com

PHP:  serialize($obj);  unserialize($s);
来源：http://vhm.jqgufenzy.top

JS:   v8.serialize(obj)        // Node
来源：http://xem.gogol.net.cn

TS:   v8.serialize(obj)        // Node
来源：http://rss.chenlongwang.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://smk.chenjidiqi.icu

Go:   encoding/gob
来源：http://zcp.fanxiaobao.xyz

Ruby: Marshal.dump(obj)
来源：http://pbu.ivvv.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://rah.fengsongda.top

================================================================================
来源：http://qag.sjlbkw.cn

L. 网络请求
来源：http://jgm.hesvh.cn

================================================================================
来源：http://spa.hysaishi.cn

[L01] 发送 GET 请求
来源：http://zri.pycfn.com

Py:   requests.get(url)                        # 第三方库 requests
来源：http://vzz.shangyingyoupin.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://qyt.guannengcc.top

JS:   await fetch(url)
来源：http://qpp.jlsjyb.cn

TS:   await fetch(url)
来源：http://izt.jyoumei.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://wxu.jiagoushi.top

Go:   resp, err := http.Get(url)
来源：http://kse.smart0.xyz

Ruby: Net::HTTP.get(URI(url))
来源：http://epz.xuanzx.com

C#:   await new HttpClient().GetStringAsync(url)
来源：http://xzw.tarul.cn

[L02] 发送 POST JSON
来源：http://mhx.yueranfly.top

Py:   requests.post(url, json={"a": 1})
来源：http://hxr.cheryme.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://vpk.feifeiyinyue.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ger.shzxlz.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://yuc.316326.xyz

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ucw.redwolf501.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mnw.gogol.net.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ray.yfazqb.com

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://vlg.hammf.cn

[L03] 设置自定义请求头
来源：http://dfz.sysykeji.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ulv.zdbjq.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://udh.hesvh.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hcw.haohaochexian.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://pst.guowangkeji.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ccb.hongshengwenyu.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://urb.cqqwz.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://bfc.yanxiufei.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://etd.hammf.cn

[L04] 设置超时
来源：http://hco.ydjk.org.cn

Py:   requests.get(url, timeout=5)
来源：http://cqp.xingfuxueyuan.xyz

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://fze.hesvh.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://qac.9152youxi.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://fjq.tian-w.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://nva.yonumen.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ukr.feifeiyinyue.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://rnw.andypj.xyz

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://qrl.snrcjt.cn

[L05] 上传文件（multipart）
来源：http://jar.jqgufenzy.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://okj.fktsv.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://jcs.nanxuanxn.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://eil.jqgfzy.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://krz.yj20258888.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://yjc.cdnleiting.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://zcx.hysaishi.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://vyb.fanxiaobao.xyz

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://zda.xuetiantiany.cn

[L06] 解析响应为 JSON
来源：http://vcy.nanxuanxn.top

Py:   resp.json()
来源：http://kcx.fzhhl.top

PHP:  json_decode($body, true);
来源：http://zue.kuanghao11.cn

JS:   await resp.json()
来源：http://xfh.sxryk.cn

TS:   await resp.json()
来源：http://ihu.dianchejie.cn


<!-- 参考信息 -->