代发 wailian999

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://lku.chenjidiqi.icu

Go:   defer f.Close()
来源：http://ckr.cucudq.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ado.shzxlz.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://cmy.fehbvm.com

================================================================================
来源：http://ope.nanxinkj.top

I. 正则表达式
来源：http://emz.sysykeji.top

================================================================================
来源：http://qyn.xuetiantiany.cn

[I01] 判断是否匹配
来源：http://aub.xuetiantiany.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://xep.iojbl.cn

PHP:  preg_match('/\d+/', $s);
来源：http://frr.hammf.cn

JS:   /\d+/.test(s)
来源：http://hkb.tian-w.cn

TS:   /\d+/.test(s)
来源：http://eky.9152youxi.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://tpx.gzhubu.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://gsc.ehwqpu.com

Ruby: s.match?(/\d+/)
来源：http://xfk.jinqigfzy.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://yjf.fanxiaobao.xyz

[I02] 提取所有匹配
来源：http://mqr.epnwcf.com

Py:   re.findall(r"\d+", s)
来源：http://sbm.daria6918.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://chr.xinyue.icu

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://nuq.zhongyouzk.top

TS:   s.match(/\d+/g)
来源：http://yeq.xuetiantiany.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://egm.jinghuilouyu.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://pwc.shuidangran.top

Ruby: s.scan(/\d+/)
来源：http://fkc.dianchejie.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://zzt.hywenlv.cn

[I03] 提取捕获分组
来源：http://xfs.ppjwa.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://inp.hammf.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://rwu.iojbl.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://quw.ydjk.org.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://tws.birdmap.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://wrk.meibo888.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://rru.jlsjyb.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ztr.gogol.net.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://mmy.cqqwz.cn

[I04] 正则替换
来源：http://blx.yanxiufei.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://drm.hcnkem.com

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://pub.hysaishi.cn

JS:   s.replace(/\d+/g, "#")
来源：http://dhb.fktsv.cn

TS:   s.replace(/\d+/g, "#")
来源：http://nyq.guannengcc.top

Java: s.replaceAll("\\d+", "#")
来源：http://vwi.nanxinkj.top

Go:   re.ReplaceAllString(s, "#")
来源：http://vkt.gogol.net.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://bga.xylfe.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ycp.nanxuanxn.top

[I05] 按正则拆分
来源：http://tpo.gotoacloud.top

Py:   re.split(r"\s*,\s*", s)
来源：http://hrp.gzhubu.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://mns.chenlongwang.top

JS:   s.split(/\s*,\s*/)
来源：http://dua.shanyushiyangkeji.top

TS:   s.split(/\s*,\s*/)
来源：http://laj.fktsv.cn

Java: s.split("\\s*,\\s*")
来源：http://ucl.yj20258.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://fjy.smart0.xyz

Ruby: s.split(/\s*,\s*/)
来源：http://jpf.xingfuxueyuan.xyz

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://pvc.shanyushiyangtech.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://onq.chenjidiqi.icu

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://szf.wangdashe.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ecx.ydzc1.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://agq.gogol.net.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://eog.guowangkeji.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://byi.nanxinkj.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://wuk.sysykeji.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ecb.tianlin.xyz

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://qxo.ydjk.org.cn

[I07] 忽略大小写与多行模式
来源：http://egk.fengsongda.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://vpn.ydzc1.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ycc.zdbjq.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://anz.uphjek.com

TS:   /error/gim
来源：http://mce.sufxvd.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://yxq.guannengcc.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://amm.c1oappe.top

Ruby: s.scan(/error/i)
来源：http://vbu.chenlongwang.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ovq.nanxuanxn.top

[I08] 贪婪与非贪婪匹配
来源：http://ejn.shzxlz.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hqq.xuetiantiany.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://bdd.xuetiantiany.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://fcl.jinqigufen.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ivz.svipenyu.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://xig.zhengqikj.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://bcp.hnqzz.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://tgv.fengsongda.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hoy.cheryme.top

================================================================================
来源：http://omn.hfpthk.cn

J. 日期与时间
来源：http://hiv.pengpengdd.cyou

================================================================================
来源：http://oun.epnwcf.com

[J01] 获取当前时间
来源：http://lqy.wangshuangyany.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://umv.cheryme.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://mky.zhoulong.xyz

JS:   new Date();  Date.now()
来源：http://nyp.cheryme.top

TS:   new Date();  Date.now()
来源：http://msn.ctjpmb.com

Java: LocalDateTime.now();  Instant.now()
来源：http://ecy.hywenlv.cn

Go:   time.Now()
来源：http://ndg.guannengcc.top

Ruby: Time.now
来源：http://qln.zhixingplan.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ckm.tian-w.cn

[J02] 格式化输出
来源：http://yks.ydzc1.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://xpk.jianghu66.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://wlj.guannengcc.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://oda.shangyingyoupin.top

TS:   d.toISOString()
来源：http://iwb.daria6918.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://kwz.yonumen.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://wmz.zhoulong.xyz

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://tyv.nanxinkj.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://vad.gotoacloud.top

[J03] 字符串解析为日期
来源：http://fwe.dianchejie.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://gmg.fanxiaobao.xyz

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://bfv.zdbjq.cn

JS:   new Date("2024-01-02")
来源：http://cpn.smart0.xyz

TS:   new Date("2024-01-02")
来源：http://ode.gogol.net.cn

Java: LocalDate.parse("2024-01-02")
来源：http://klc.sufxvd.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ebp.shanyushiyangkeji.top

Ruby: Date.parse("2024-01-02")
来源：http://wre.bjfxy.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://xtt.andypj.xyz

[J04] 时间戳与日期互转
来源：http://vys.xingfuxueyuan.xyz

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hwu.feifeiyinyue.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://bhn.ydjk.org.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ulj.9152youxi.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://hta.chenzaomai.com

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://xkg.cucudq.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://djb.aizwys.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://fyu.sxryk.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://rwy.birdmap.top

[J05] 时间加减（加 7 天）
来源：http://bil.xingfuxueyuan.xyz

Py:   now + timedelta(days=7)
来源：http://dwi.ctjpmb.com

PHP:  (new DateTime())->modify("+7 days");
来源：http://oes.xinyue.icu

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://dfo.redwolf501.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://kwi.sysykeji.top

Java: LocalDate.now().plusDays(7)
来源：http://qbo.xziqi.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://uxn.9152youxi.cn

Ruby: Time.now + 7 * 86400
来源：http://xth.sweek.top

C#:   DateTime.Now.AddDays(7)
来源：http://qcn.hysaishi.cn

[J06] 计算两时间之差
来源：http://eqy.yj20258888.top

Py:   (end - start).total_seconds()
来源：http://jvl.cqqwz.cn

PHP:  $end->diff($start)->days;
来源：http://lew.meibo888.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ytd.jianghu66.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://rzg.fehbvm.com

Java: Duration.between(start, end).toSeconds()
来源：http://jug.nwbrower.top

Go:   end.Sub(start).Hours()
来源：http://mob.fzhhl.top

Ruby: end - start                 # 返回秒数
来源：http://rec.aibaodan.cn

C#:   (end - start).TotalSeconds
来源：http://fcv.pycfn.com

[J07] 比较两个日期
来源：http://bel.uphjek.com

Py:   d1 < d2;  d1 == d2
来源：http://jlv.xuanzx.com

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://tmz.nanxinkj.top

JS:   d1.getTime() < d2.getTime()
来源：http://vxl.sysykeji.top

TS:   d1.getTime() < d2.getTime()
来源：http://iia.52xcode.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://coo.xinyue.icu

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://egz.zhixingplan.top

Ruby: d1 < d2;  d1 == d2
来源：http://xbz.sxryk.cn

C#:   d1 < d2;  d1 == d2
来源：http://yvh.guannengcc.top

[J08] 提取年月日与星期
来源：http://dup.9152youxi.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://sno.hongshengwenyu.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://qfm.ivvv.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://kvf.daria6918.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://bny.yongpay.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://cxf.ybcxt.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://wdb.yj202588.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://fce.chenjidiqi.icu

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://vhd.yvedp.cn

[J09] 时区处理
来源：http://eaj.hongshengwenyu.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://axt.guannengcc.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://sdo.smart0.xyz

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://skb.aizwys.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://rtf.jinqigufen.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://fwe.316326.xyz

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://cet.wangshuangyany.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://cuc.yj20258.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://mes.yonumen.top

[J10] 取今天 / 本月第一天
来源：http://gzh.xziqi.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://avx.zdqjudy.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://svl.9152youxi.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://svu.yfazqb.com

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hkm.haohaochexian.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://eax.yangfankeji.com

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ggh.cashguo.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://dex.zhixingplan.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://avo.sysykeji.top

================================================================================
来源：http://dxq.birdmap.top

K. JSON 与序列化
来源：http://wib.sxryk.cn

================================================================================
来源：http://clt.9152youxi.cn

[K01] 对象转 JSON 字符串
来源：http://knl.sxryk.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://cvs.yuanzhike.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://wxz.jyoumei.cn

JS:   JSON.stringify(obj)
来源：http://qql.9152youxi.cn

TS:   JSON.stringify(obj)
来源：http://bgj.gogol.net.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://udn.hfpthk.cn

Go:   json.Marshal(obj)
来源：http://chl.dianchejie.cn

Ruby: obj.to_json                                     // require "json"
来源：http://xqe.hywenlv.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://ccw.zhaomingkeji.xyz

[K02] JSON 字符串转对象
来源：http://efw.aibaodan.cn

Py:   json.loads(s)
来源：http://mvp.fzhhl.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://pbz.yj202588.top

JS:   JSON.parse(s)
来源：http://kii.iojbl.cn

TS:   JSON.parse(s)
来源：http://fqx.jlsjyb.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://icw.nanxuanxn.top

Go:   json.Unmarshal(data, &v)
来源：http://civ.dianchejie.cn

Ruby: JSON.parse(s)
来源：http://wsa.fktsv.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://gun.bbcook.cn

[K03] JSON 美化输出（带缩进）
来源：http://tix.svipenyu.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://yqi.uphjek.com

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://gbb.yueranfly.top

JS:   JSON.stringify(obj, null, 2)
来源：http://owq.zdbjq.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://vmf.ybcxt.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://uka.pycfn.com

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://bam.snrcjt.cn

Ruby: JSON.pretty_generate(obj)
来源：http://vbg.yanxiufei.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ekl.haohaochexian.top

[K04] 读取 JSON 文件
来源：http://hkz.zhaomingkeji.xyz

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://pgj.52xcode.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://fxb.hfpthk.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ssy.bjfxy.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://aav.uphjek.com

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hqm.tianlin.xyz

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://res.cheryme.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://drs.yueranfly.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://pqy.zycfv.cn

[K05] 深拷贝对象
来源：http://une.jlsjyb.cn

Py:   copy.deepcopy(obj)
来源：http://glc.havefunace.top

PHP:  unserialize(serialize($obj));
来源：http://tuq.gogol.net.cn

JS:   structuredClone(obj)
来源：http://krw.mhx1999.top

TS:   structuredClone(obj)
来源：http://apr.tanke756.top

Java: // 手写拷贝构造，或序列化往返
来源：http://cal.bbcook.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://svw.bbcook.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://omb.hywenlv.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://kjx.ppjwa.cn

[K06] 解析 URL 查询串
来源：http://fmz.zycfv.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ipj.chenzaomai.com

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://rbk.jiagoushi.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hjs.smart0.xyz

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://vsr.gotoacloud.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wiy.c1oappe.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://vrg.shanyushiyangkeji.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://lmg.dashuyun.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://eeh.shanyushiyangtech.top

[K07] 进制转换
来源：http://vxv.hnqzz.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://cmz.zhijiandao.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hud.tarul.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://upt.fzhhl.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://jgz.hnqzz.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://izj.0kj1m.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://poz.redwolf501.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://jtp.bjfxy.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wad.jyoumei.cn

[K08] 二进制序列化（非 JSON）
来源：http://fls.chenlongwang.top

Py:   pickle.dumps(obj)
来源：http://xyv.daxiang520.top

PHP:  serialize($obj);  unserialize($s);
来源：http://qud.xinyue.icu

JS:   v8.serialize(obj)        // Node
来源：http://ihu.guannengcc.top

TS:   v8.serialize(obj)        // Node
来源：http://rnz.cashguo.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://zjg.jinyuanbaomall.cn

Go:   encoding/gob
来源：http://djh.nanxuanxn.top

Ruby: Marshal.dump(obj)
来源：http://mnr.yueranfly.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://sod.pengpengdd.cyou

================================================================================
来源：http://rdp.uphjek.com

L. 网络请求
来源：http://jqe.guowangkeji.top

================================================================================
来源：http://xqk.daxiang520.top

[L01] 发送 GET 请求
来源：http://tqe.316326.xyz

Py:   requests.get(url)                        # 第三方库 requests
来源：http://bwk.cqqwz.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://acl.hcnkem.com

JS:   await fetch(url)
来源：http://pbw.xziqi.cn

TS:   await fetch(url)
来源：http://kcl.redwolf501.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://axt.ywan-chungtsiang.top

Go:   resp, err := http.Get(url)
来源：http://pli.andypj.xyz

Ruby: Net::HTTP.get(URI(url))
来源：http://ybt.jinqigufen.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://uba.hfpthk.cn

[L02] 发送 POST JSON
来源：http://pzj.shanyushiyangkeji.top

Py:   requests.post(url, json={"a": 1})
来源：http://jqh.andypj.xyz

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://fnr.sufxvd.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://zgp.hcnkem.com

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://jqc.hnxiangtu.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://yrs.havefunace.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://miy.feifeiyinyue.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://vlt.havefunace.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://cau.tian-w.cn

[L03] 设置自定义请求头
来源：http://ate.fanxiaobao.xyz

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://onl.zhiwuduotai.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ydr.shangyingyoupin.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://pkv.hnxiangtu.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://pml.quarkkingdee.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://pqm.yj202588.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://out.zhoulong.xyz

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://gnl.havefunace.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://kpm.dashuyun.cn

[L04] 设置超时
来源：http://hxq.uphjek.com

Py:   requests.get(url, timeout=5)
来源：http://fmq.ppjwa.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ftm.jqgufenzy.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mmz.xingfuxueyuan.xyz

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://jnk.shuidangran.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://pgc.sweek.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://llm.wangdashe.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://lrn.aizwys.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://akc.zhengqikj.top

[L05] 上传文件（multipart）
来源：http://nix.zycfv.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ivn.chenlongwang.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://djo.hcnkem.com

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://gsk.nanxuanxn.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://fdl.yj20258888.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://gbe.chenzaomai.com

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://vmy.fktsv.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://opu.hywenlv.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://zxh.zhongyouzk.top

[L06] 解析响应为 JSON
来源：http://woo.hfpthk.cn

Py:   resp.json()
来源：http://nuq.smart0.xyz

PHP:  json_decode($body, true);
来源：http://ipn.zdbjq.cn

JS:   await resp.json()
来源：http://dnl.dianchejie.cn

TS:   await resp.json()
来源：http://itd.zhoulong.xyz


<!-- 参考信息 -->