代发 wailian999

Py:   with open("a.txt") as f: data = f.read()
来源：http://guk.fanxiaobao.xyz

PHP:  // 无 with：在 finally 里 fclose()
来源：http://xcs.sufxvd.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://xlf.yuxming.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://nza.yongpay.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://fjk.yueranfly.top

Go:   defer f.Close()
来源：http://tpn.zycfv.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://rxg.gzhubu.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ahw.jinyuanbaomall.cn

================================================================================
来源：http://ppr.fktsv.cn

I. 正则表达式
来源：http://bny.xuetiantiany.cn

================================================================================
来源：http://ebz.yvedp.cn

[I01] 判断是否匹配
来源：http://vhw.ybcxt.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://esk.vehdjk.com

PHP:  preg_match('/\d+/', $s);
来源：http://ogv.wangdashe.top

JS:   /\d+/.test(s)
来源：http://vbq.nanxuanxn.top

TS:   /\d+/.test(s)
来源：http://qhj.sysykeji.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://tfy.dashuyun.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://zgv.aibaodan.cn

Ruby: s.match?(/\d+/)
来源：http://gdo.jinghuilouyu.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://izw.yfazqb.com

[I02] 提取所有匹配
来源：http://zjf.chenzaomai.com

Py:   re.findall(r"\d+", s)
来源：http://cej.yj202588.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://the.zhaomingkeji.xyz

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://mdk.zhijiandao.cn

TS:   s.match(/\d+/g)
来源：http://zfe.hesvh.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://urn.feifeiyinyue.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://fou.feifeiyinyue.top

Ruby: s.scan(/\d+/)
来源：http://uic.guannengcc.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://qca.zdqjudy.top

[I03] 提取捕获分组
来源：http://jvn.0kj1m.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://fjp.sysykeji.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://xdn.fehbvm.com

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://asj.feifeiyinyue.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://qqk.ywan-chungtsiang.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://mtv.tanke756.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://pld.mhx1999.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://sbk.uphjek.com

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://sly.chenlongwang.top

[I04] 正则替换
来源：http://sxi.cqqwz.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://sxf.zhiwuduotai.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://wkl.nwbrower.top

JS:   s.replace(/\d+/g, "#")
来源：http://ask.hnxiangtu.top

TS:   s.replace(/\d+/g, "#")
来源：http://str.fzhhl.top

Java: s.replaceAll("\\d+", "#")
来源：http://onf.jinyuanbaomall.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://gqx.jinqigufen.top

Ruby: s.gsub(/\d+/, "#")
来源：http://jmx.cheryme.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://dhu.nwbrower.top

[I05] 按正则拆分
来源：http://nyb.sjlbkw.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://wnr.zhaomingkeji.xyz

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ksg.shzxlz.cn

JS:   s.split(/\s*,\s*/)
来源：http://sbm.hongshengwenyu.top

TS:   s.split(/\s*,\s*/)
来源：http://yjj.yangfankeji.com

Java: s.split("\\s*,\\s*")
来源：http://tnf.dianchejie.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ysq.vqdsnc.cn

Ruby: s.split(/\s*,\s*/)
来源：http://jjc.sjlbkw.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://dtx.vehdjk.com

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://pkg.zhengqikj.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://cty.quarkkingdee.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://dpw.fengsongda.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://knj.hysaishi.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hsu.jinyuanbaomall.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://kzv.smart0.xyz

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://xcl.vqdsnc.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://sgp.cheryme.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://eyg.ctjpmb.com

[I07] 忽略大小写与多行模式
来源：http://iih.sysykeji.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://nys.xinyue.icu

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://fmo.zhixingplan.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://zyw.dashuyun.cn

TS:   /error/gim
来源：http://jud.zhoulong.xyz

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://egm.jinyuanbaomall.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://vho.chenzaomai.com

Ruby: s.scan(/error/i)
来源：http://alk.hcnkem.com

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://zga.yvedp.cn

[I08] 贪婪与非贪婪匹配
来源：http://kot.zhengqikj.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://mbl.shzxlz.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ewu.kuanghao11.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ueq.cucudq.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://vbm.xylfe.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://zhg.meibo888.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://nxw.9152youxi.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://loq.xuetiantiany.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://sax.feifeiyinyue.top

================================================================================
来源：http://ibh.gzhubu.top

J. 日期与时间
来源：http://wda.epnwcf.com

================================================================================
来源：http://fht.ywan-chungtsiang.top

[J01] 获取当前时间
来源：http://xop.bbcook.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://tdn.kuanghao11.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://wtp.cheryme.top

JS:   new Date();  Date.now()
来源：http://pao.guannengcc.top

TS:   new Date();  Date.now()
来源：http://lsw.ybcxt.top

Java: LocalDateTime.now();  Instant.now()
来源：http://vvu.9152youxi.cn

Go:   time.Now()
来源：http://our.yj202588.top

Ruby: Time.now
来源：http://gjp.aibaodan.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://poq.9152youxi.cn

[J02] 格式化输出
来源：http://hcj.yongpay.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://sxx.bbcook.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://jyu.hnqzz.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ioh.hywenlv.cn

TS:   d.toISOString()
来源：http://iyz.ivvv.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://zqh.tianlin.xyz

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://rft.cqqwz.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://dus.cheryme.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://glr.yfazqb.com

[J03] 字符串解析为日期
来源：http://nvx.xuanzx.com

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://vfz.hongshengwenyu.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://tbg.feifeiyinyue.top

JS:   new Date("2024-01-02")
来源：http://kba.sysykeji.top

TS:   new Date("2024-01-02")
来源：http://dwt.fzhhl.top

Java: LocalDate.parse("2024-01-02")
来源：http://odv.kuanghao11.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://nsx.gzhubu.top

Ruby: Date.parse("2024-01-02")
来源：http://unk.pycfn.com

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://zlb.yanxiufei.cn

[J04] 时间戳与日期互转
来源：http://xin.52xcode.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://zse.chenjidiqi.icu

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://iko.guowangkeji.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://bnw.daxiang520.top

TS:   Math.floor(Date.now() / 1000)
来源：http://eee.cheryme.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://foq.redwolf501.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://goq.yuanzhike.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://fuz.ybcxt.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://iig.sweek.top

[J05] 时间加减（加 7 天）
来源：http://lad.tianlin.xyz

Py:   now + timedelta(days=7)
来源：http://wwe.gzhubu.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://aoa.jiagoushi.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://pri.xuetiantiany.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ebz.ctjpmb.com

Java: LocalDate.now().plusDays(7)
来源：http://wpn.vehdjk.com

Go:   time.Now().AddDate(0, 0, 7)
来源：http://rrr.yanxiufei.cn

Ruby: Time.now + 7 * 86400
来源：http://ybu.quarkkingdee.top

C#:   DateTime.Now.AddDays(7)
来源：http://jqh.yvedp.cn

[J06] 计算两时间之差
来源：http://wpk.cheryme.top

Py:   (end - start).total_seconds()
来源：http://qwo.bjfxy.top

PHP:  $end->diff($start)->days;
来源：http://poe.sysykeji.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://uts.hammf.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://mng.mhx1999.top

Java: Duration.between(start, end).toSeconds()
来源：http://hrs.jianghu66.top

Go:   end.Sub(start).Hours()
来源：http://ynb.chenjidiqi.icu

Ruby: end - start                 # 返回秒数
来源：http://sgw.jinyuanbaomall.cn

C#:   (end - start).TotalSeconds
来源：http://cwm.zhixingplan.top

[J07] 比较两个日期
来源：http://qvl.jinqigfzy.top

Py:   d1 < d2;  d1 == d2
来源：http://vkk.ydjk.org.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://cou.vqdsnc.cn

JS:   d1.getTime() < d2.getTime()
来源：http://fvq.fengsongda.top

TS:   d1.getTime() < d2.getTime()
来源：http://iaw.mhx1999.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://vpz.hnxiangtu.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://htt.ydjk.org.cn

Ruby: d1 < d2;  d1 == d2
来源：http://hso.hammf.cn

C#:   d1 < d2;  d1 == d2
来源：http://bar.nwbrower.top

[J08] 提取年月日与星期
来源：http://kek.sxryk.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://soy.vqdsnc.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ley.yuanzhike.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://dwc.andypj.xyz

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://tkk.guannengcc.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://xkx.shanyushiyangkeji.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://vyz.fzhhl.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://izf.ctjpmb.com

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://oyh.zhiwuduotai.top

[J09] 时区处理
来源：http://fjn.yonumen.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://kys.dianchejie.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://aqv.epnwcf.com

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://kje.jianghu66.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://nxz.nanxuanxn.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://idr.fehbvm.com

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://csm.iojbl.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://zwu.hongshengwenyu.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://cuu.nanxinkj.top

[J10] 取今天 / 本月第一天
来源：http://tfv.xuanzx.com

Py:   date.today();  date.today().replace(day=1)
来源：http://mbi.zhengqikj.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://byl.chenzaomai.com

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://jao.chenjidiqi.icu

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://jeq.uphjek.com

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://caz.yuxming.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://bnb.zhijiandao.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hjc.fktsv.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://nui.guannengcc.top

================================================================================
来源：http://lnz.316326.xyz

K. JSON 与序列化
来源：http://fue.hnqzz.top

================================================================================
来源：http://pia.cqqwz.cn

[K01] 对象转 JSON 字符串
来源：http://wzi.smart0.xyz

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hnd.shangyingyoupin.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://igs.zycfv.cn

JS:   JSON.stringify(obj)
来源：http://trc.fzhhl.top

TS:   JSON.stringify(obj)
来源：http://iva.shanyushiyangtech.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ylr.ydjk.org.cn

Go:   json.Marshal(obj)
来源：http://qke.daria6918.cn

Ruby: obj.to_json                                     // require "json"
来源：http://azz.xinyue.icu

C#:   JsonSerializer.Serialize(obj)
来源：http://udv.kuanghao11.cn

[K02] JSON 字符串转对象
来源：http://kaw.gogol.net.cn

Py:   json.loads(s)
来源：http://cce.shzxlz.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://rcl.vehdjk.com

JS:   JSON.parse(s)
来源：http://jym.aibaodan.cn

TS:   JSON.parse(s)
来源：http://lbk.cqqwz.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://rni.yvedp.cn

Go:   json.Unmarshal(data, &v)
来源：http://tut.xinyue.icu

Ruby: JSON.parse(s)
来源：http://tdq.tianlin.xyz

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://vfi.ehwqpu.com

[K03] JSON 美化输出（带缩进）
来源：http://wsp.haohaochexian.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://xhw.sxryk.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://kct.meibo888.top

JS:   JSON.stringify(obj, null, 2)
来源：http://nhe.birdmap.top

TS:   JSON.stringify(obj, null, 2)
来源：http://lkt.fanxiaobao.xyz

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://qkj.xinyue.icu

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://tue.hongshengwenyu.top

Ruby: JSON.pretty_generate(obj)
来源：http://jhx.tianlin.xyz

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://thq.ivvv.top

[K04] 读取 JSON 文件
来源：http://iym.aibaodan.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://zpm.guannengcc.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://wca.chenlongwang.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://pdq.uphjek.com

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://eld.ivvv.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ijk.jianghu66.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ckm.andypj.xyz

Ruby: JSON.parse(File.read("a.json"))
来源：http://yti.hnqzz.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wmk.zhongyouzk.top

[K05] 深拷贝对象
来源：http://bnq.svipenyu.cn

Py:   copy.deepcopy(obj)
来源：http://bow.smart0.xyz

PHP:  unserialize(serialize($obj));
来源：http://kob.pycfn.com

JS:   structuredClone(obj)
来源：http://uns.epnwcf.com

TS:   structuredClone(obj)
来源：http://kbg.guowangkeji.top

Java: // 手写拷贝构造，或序列化往返
来源：http://ble.chenlongwang.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://gxu.zdqjudy.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://gge.hnqzz.top

C#:   // 序列化往返，或自定义 Clone
来源：http://geu.shangyingyoupin.top

[K06] 解析 URL 查询串
来源：http://pez.9152youxi.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://atk.wangdashe.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://fkc.ydjk.org.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://lml.nanxuanxn.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hrj.fanxiaobao.xyz

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://sjh.pycfn.com

Go:   url.ParseQuery("a=1&b=2")
来源：http://wgj.wangdashe.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://mta.vqdsnc.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://iga.svipenyu.cn

[K07] 进制转换
来源：http://ati.aibaodan.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://gei.yfazqb.com

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ssx.dashuyun.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://yhk.shzxlz.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://fkr.gogol.net.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://kqp.yongpay.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://bda.hfpthk.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://psk.tian-w.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://tly.ydjk.org.cn

[K08] 二进制序列化（非 JSON）
来源：http://nyt.zycfv.cn

Py:   pickle.dumps(obj)
来源：http://djt.jqgfzy.top

PHP:  serialize($obj);  unserialize($s);
来源：http://hpr.jiagoushi.top

JS:   v8.serialize(obj)        // Node
来源：http://eqm.andypj.xyz

TS:   v8.serialize(obj)        // Node
来源：http://iai.snrcjt.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://sgm.uphjek.com

Go:   encoding/gob
来源：http://zac.jiagoushi.top

Ruby: Marshal.dump(obj)
来源：http://pzv.jinqigufen.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://dmc.redwolf501.top

================================================================================
来源：http://gap.cdnleiting.top

L. 网络请求
来源：http://ajd.yueranfly.top

================================================================================
来源：http://eno.shangyingyoupin.top

[L01] 发送 GET 请求
来源：http://hve.dianchejie.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://nys.tianlin.xyz

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://jpd.daxiang520.top

JS:   await fetch(url)
来源：http://vxv.jiagoushi.top

TS:   await fetch(url)
来源：http://hze.fengsongda.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://qst.xuetiantiany.cn

Go:   resp, err := http.Get(url)
来源：http://bwe.havefunace.top

Ruby: Net::HTTP.get(URI(url))
来源：http://cbs.bbcook.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://vfx.zhaomingkeji.xyz

[L02] 发送 POST JSON
来源：http://bwi.zycfv.cn

Py:   requests.post(url, json={"a": 1})
来源：http://zsk.sjlbkw.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://dzj.ivvv.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://nsf.wangshuangyany.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hpi.zhengqikj.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://aco.hywenlv.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://kij.sxryk.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://dor.sjlbkw.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mbb.hnqzz.top

[L03] 设置自定义请求头
来源：http://iso.sxryk.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ihu.snrcjt.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://zmh.yuxming.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://fko.hnxiangtu.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ufs.fengsongda.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mcz.jinqigfzy.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://qie.meibo888.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://vrx.fzhhl.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hoc.ybcxt.top

[L04] 设置超时
来源：http://onq.xuetiantiany.cn

Py:   requests.get(url, timeout=5)
来源：http://shp.shanyushiyangtech.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://yqv.uphjek.com

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://dbj.jianghu66.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://xgz.hongshengwenyu.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://puc.cdnleiting.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wvw.zhongyouzk.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://koh.gzhubu.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://xft.sxryk.cn

[L05] 上传文件（multipart）
来源：http://wks.yongpay.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://jra.hywenlv.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://xzz.guannengcc.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://nwu.hnxiangtu.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://okl.zycfv.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://jgb.zhengqikj.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://fbx.hnxiangtu.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ify.tian-w.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://yms.chenlongwang.top

[L06] 解析响应为 JSON
来源：http://dml.hcnkem.com


<!-- 参考信息 -->