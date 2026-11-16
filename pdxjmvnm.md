代发 wailian999

Py:   with open("a.txt") as f: data = f.read()
来源：http://zxk.ehwqpu.com

PHP:  // 无 with：在 finally 里 fclose()
来源：http://tid.jinqigufen.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://mvq.yfazqb.com

TS:   // 无 with：在 finally 里关闭句柄
来源：http://zma.xziqi.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://zny.jinqigfzy.top

Go:   defer f.Close()
来源：http://hle.gotoacloud.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://oru.yj202588.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://pvu.yfazqb.com

================================================================================
来源：http://jlk.zhaomingkeji.xyz

I. 正则表达式
来源：http://bok.hesvh.cn

================================================================================
来源：http://qub.tarul.cn

[I01] 判断是否匹配
来源：http://osq.nanxuanxn.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ozi.sysykeji.top

PHP:  preg_match('/\d+/', $s);
来源：http://zax.ydjk.org.cn

JS:   /\d+/.test(s)
来源：http://gxw.xuanzx.com

TS:   /\d+/.test(s)
来源：http://jph.yanxiufei.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://gzx.cheryme.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ife.hywenlv.cn

Ruby: s.match?(/\d+/)
来源：http://oge.xziqi.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://nqo.zhijiandao.cn

[I02] 提取所有匹配
来源：http://lza.smart0.xyz

Py:   re.findall(r"\d+", s)
来源：http://esw.wangdashe.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://swm.jyoumei.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://asx.birdmap.top

TS:   s.match(/\d+/g)
来源：http://exp.yj202588.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://aru.vqdsnc.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://pyu.jlsjyb.cn

Ruby: s.scan(/\d+/)
来源：http://svk.cqqwz.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://oby.wangdashe.top

[I03] 提取捕获分组
来源：http://pyt.fktsv.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ond.sxryk.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://jxd.yj20258.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ztz.hongshengwenyu.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://yxm.ctjpmb.com

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://fdk.sufxvd.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://frr.bbcook.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://pmk.xuetiantiany.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://jpm.nwbrower.top

[I04] 正则替换
来源：http://hss.yj20258888.top

Py:   re.sub(r"\d+", "#", s)
来源：http://mrp.xuetiantiany.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://rbd.316326.xyz

JS:   s.replace(/\d+/g, "#")
来源：http://lmo.zycfv.cn

TS:   s.replace(/\d+/g, "#")
来源：http://rvh.xylfe.cn

Java: s.replaceAll("\\d+", "#")
来源：http://rzx.hfpthk.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://aga.pengpengdd.cyou

Ruby: s.gsub(/\d+/, "#")
来源：http://nrv.wangdashe.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://lvy.0kj1m.cn

[I05] 按正则拆分
来源：http://qtf.fehbvm.com

Py:   re.split(r"\s*,\s*", s)
来源：http://klc.ivvv.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://csc.wangdashe.top

JS:   s.split(/\s*,\s*/)
来源：http://idn.sufxvd.cn

TS:   s.split(/\s*,\s*/)
来源：http://xvb.xingfuxueyuan.xyz

Java: s.split("\\s*,\\s*")
来源：http://kdp.jinghuilouyu.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://uso.yuxming.cn

Ruby: s.split(/\s*,\s*/)
来源：http://nma.yongpay.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://lkh.hnqzz.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://vtt.xuetiantiany.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://zli.xuanzx.com

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://wra.chenlongwang.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wjm.zhiwuduotai.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wcn.aizwys.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://bwh.hnxiangtu.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://poy.iojbl.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://zst.jianghu66.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://scf.daria6918.cn

[I07] 忽略大小写与多行模式
来源：http://xwy.jiagoushi.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://bfy.dianchejie.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://edn.sjlbkw.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://eim.ivvv.top

TS:   /error/gim
来源：http://nug.chenzaomai.com

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://kkz.wangshuangyany.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://pmu.tarul.cn

Ruby: s.scan(/error/i)
来源：http://nnh.guowangkeji.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://zvx.zdqjudy.top

[I08] 贪婪与非贪婪匹配
来源：http://wxf.zhijiandao.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://syg.ivvv.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://lhy.hnxiangtu.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ntp.nanxuanxn.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://gle.fzhhl.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://guy.316326.xyz

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://toj.yuxming.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://tma.xingfuxueyuan.xyz

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://byk.pycfn.com

================================================================================
来源：http://dca.uphjek.com

J. 日期与时间
来源：http://ukv.jianghu66.top

================================================================================
来源：http://nys.cdnleiting.top

[J01] 获取当前时间
来源：http://rjk.yuxming.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://agm.kuanghao11.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://rnk.snrcjt.cn

JS:   new Date();  Date.now()
来源：http://fnm.zhengqikj.top

TS:   new Date();  Date.now()
来源：http://ufj.yanxiufei.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://yim.quarkkingdee.top

Go:   time.Now()
来源：http://kau.guowangkeji.top

Ruby: Time.now
来源：http://psy.quarkkingdee.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://igb.pycfn.com

[J02] 格式化输出
来源：http://xkm.redwolf501.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://jhj.chenlongwang.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://lef.tian-w.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://lio.zdqjudy.top

TS:   d.toISOString()
来源：http://iht.yj20258.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://xjv.sufxvd.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://yex.cdnleiting.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ctg.yonumen.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://cfy.birdmap.top

[J03] 字符串解析为日期
来源：http://mfj.cqqwz.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://sps.kuanghao11.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://xpj.316326.xyz

JS:   new Date("2024-01-02")
来源：http://gvm.yuanzhike.top

TS:   new Date("2024-01-02")
来源：http://sbq.zhiwuduotai.top

Java: LocalDate.parse("2024-01-02")
来源：http://byi.zhixingplan.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://fjz.ywan-chungtsiang.top

Ruby: Date.parse("2024-01-02")
来源：http://iid.xuetiantiany.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://wxp.shanyushiyangkeji.top

[J04] 时间戳与日期互转
来源：http://its.gzhubu.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://sts.chenlongwang.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://afk.jinqigufen.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hky.jinqigufen.top

TS:   Math.floor(Date.now() / 1000)
来源：http://jla.meibo888.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://awp.hywenlv.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://rfr.52xcode.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://bid.jinghuilouyu.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://xmq.zdbjq.cn

[J05] 时间加减（加 7 天）
来源：http://wvl.vqdsnc.cn

Py:   now + timedelta(days=7)
来源：http://rmm.vehdjk.com

PHP:  (new DateTime())->modify("+7 days");
来源：http://xqw.tarul.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://mpn.yueranfly.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://phn.0kj1m.cn

Java: LocalDate.now().plusDays(7)
来源：http://aan.hnqzz.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://qll.bbcook.cn

Ruby: Time.now + 7 * 86400
来源：http://xva.wangdashe.top

C#:   DateTime.Now.AddDays(7)
来源：http://teg.gogol.net.cn

[J06] 计算两时间之差
来源：http://ezf.ivvv.top

Py:   (end - start).total_seconds()
来源：http://zqg.ydjk.org.cn

PHP:  $end->diff($start)->days;
来源：http://nty.ybcxt.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ugq.aibaodan.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://mmq.chenjidiqi.icu

Java: Duration.between(start, end).toSeconds()
来源：http://oik.shanyushiyangtech.top

Go:   end.Sub(start).Hours()
来源：http://gbr.zhiwuduotai.top

Ruby: end - start                 # 返回秒数
来源：http://ssm.jinyuanbaomall.cn

C#:   (end - start).TotalSeconds
来源：http://xtj.hysaishi.cn

[J07] 比较两个日期
来源：http://owt.shangyingyoupin.top

Py:   d1 < d2;  d1 == d2
来源：http://xee.chenjidiqi.icu

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://teg.tianlin.xyz

JS:   d1.getTime() < d2.getTime()
来源：http://fsj.uphjek.com

TS:   d1.getTime() < d2.getTime()
来源：http://sgh.feifeiyinyue.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://pxv.vehdjk.com

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://sku.cqqwz.cn

Ruby: d1 < d2;  d1 == d2
来源：http://pfk.cucudq.cn

C#:   d1 < d2;  d1 == d2
来源：http://uns.ywan-chungtsiang.top

[J08] 提取年月日与星期
来源：http://sgf.shzxlz.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://xnw.hcnkem.com

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://vwi.zycfv.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ugy.yanxiufei.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://fbj.chenjidiqi.icu

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://qql.feifeiyinyue.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://xdp.sxryk.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://xtk.havefunace.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://zht.jinyuanbaomall.cn

[J09] 时区处理
来源：http://mid.xinyue.icu

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://jfq.hysaishi.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://xnv.xinyue.icu

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://gfy.hongshengwenyu.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://cjx.0kj1m.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://wrj.ehwqpu.com

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ojw.hesvh.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://tki.hywenlv.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://jfd.smart0.xyz

[J10] 取今天 / 本月第一天
来源：http://vsh.pycfn.com

Py:   date.today();  date.today().replace(day=1)
来源：http://tka.daria6918.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://awb.ybcxt.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://lkr.aizwys.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://jog.shzxlz.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://irh.shuidangran.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://lnc.xuetiantiany.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://nvh.yvedp.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://gqn.zhaomingkeji.xyz

================================================================================
来源：http://ihw.vehdjk.com

K. JSON 与序列化
来源：http://tab.gzhubu.top

================================================================================
来源：http://gop.daria6918.cn

[K01] 对象转 JSON 字符串
来源：http://zkb.9152youxi.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://dpn.mhx1999.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://klw.iojbl.cn

JS:   JSON.stringify(obj)
来源：http://jin.gotoacloud.top

TS:   JSON.stringify(obj)
来源：http://ggg.hfpthk.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ydy.jinqigufen.top

Go:   json.Marshal(obj)
来源：http://drb.fehbvm.com

Ruby: obj.to_json                                     // require "json"
来源：http://svz.shanyushiyangtech.top

C#:   JsonSerializer.Serialize(obj)
来源：http://arj.nwbrower.top

[K02] JSON 字符串转对象
来源：http://xiz.0kj1m.cn

Py:   json.loads(s)
来源：http://uuv.aizwys.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://jki.fengsongda.top

JS:   JSON.parse(s)
来源：http://uul.c1oappe.top

TS:   JSON.parse(s)
来源：http://ghz.tianlin.xyz

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://yhd.ppjwa.cn

Go:   json.Unmarshal(data, &v)
来源：http://elj.xylfe.cn

Ruby: JSON.parse(s)
来源：http://tsg.ctjpmb.com

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hod.yuxming.cn

[K03] JSON 美化输出（带缩进）
来源：http://oyx.jinqigufen.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://rso.hysaishi.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://vxp.redwolf501.top

JS:   JSON.stringify(obj, null, 2)
来源：http://ija.daria6918.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://rzp.birdmap.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://pyr.shuidangran.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://yda.xuanzx.com

Ruby: JSON.pretty_generate(obj)
来源：http://ith.fktsv.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://lmb.zhijiandao.cn

[K04] 读取 JSON 文件
来源：http://nlu.yvedp.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://sec.aizwys.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://irx.zhengqikj.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://pup.vqdsnc.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://lwy.ctjpmb.com

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://cod.jinqigfzy.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://rsx.wangdashe.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://ltw.quarkkingdee.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://kdb.fzhhl.top

[K05] 深拷贝对象
来源：http://wwb.ctjpmb.com

Py:   copy.deepcopy(obj)
来源：http://ywg.aibaodan.cn

PHP:  unserialize(serialize($obj));
来源：http://ptr.ppjwa.cn

JS:   structuredClone(obj)
来源：http://dga.guowangkeji.top

TS:   structuredClone(obj)
来源：http://bni.mhx1999.top

Java: // 手写拷贝构造，或序列化往返
来源：http://dqc.hcnkem.com

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://xwd.xylfe.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://dlp.havefunace.top

C#:   // 序列化往返，或自定义 Clone
来源：http://pfq.shanyushiyangkeji.top

[K06] 解析 URL 查询串
来源：http://fks.uphjek.com

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://tbi.feifeiyinyue.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mcc.jlsjyb.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://aao.gaohongyu789.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://fea.shuidangran.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://kvg.tanke756.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://phj.316326.xyz

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://pnh.cheryme.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://edo.9152youxi.cn

[K07] 进制转换
来源：http://azi.jinyuanbaomall.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://iiy.quarkkingdee.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://mrv.daxiang520.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://fnn.hcnkem.com

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://cqy.chenjidiqi.icu

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://opf.xylfe.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://cxo.nanxinkj.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://kgb.sufxvd.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://bom.wangshuangyany.cn

[K08] 二进制序列化（非 JSON）
来源：http://urm.zhiwuduotai.top

Py:   pickle.dumps(obj)
来源：http://kvn.hnqzz.top

PHP:  serialize($obj);  unserialize($s);
来源：http://xym.0kj1m.cn

JS:   v8.serialize(obj)        // Node
来源：http://wbx.aizwys.cn

TS:   v8.serialize(obj)        // Node
来源：http://isx.ydzc1.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://sho.chenjidiqi.icu

Go:   encoding/gob
来源：http://gfo.aibaodan.cn

Ruby: Marshal.dump(obj)
来源：http://hxq.hcnkem.com

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://xuy.gaohongyu789.top

================================================================================
来源：http://hhs.sweek.top

L. 网络请求
来源：http://clr.nanxuanxn.top

================================================================================
来源：http://pwt.quarkkingdee.top

[L01] 发送 GET 请求
来源：http://srz.zycfv.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://aoh.fengsongda.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://pff.zhixingplan.top

JS:   await fetch(url)
来源：http://cjm.smart0.xyz

TS:   await fetch(url)
来源：http://env.guannengcc.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://uwu.haohaochexian.top

Go:   resp, err := http.Get(url)
来源：http://fbf.bbcook.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://ywv.0kj1m.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://pkh.316326.xyz

[L02] 发送 POST JSON
来源：http://efr.ctjpmb.com

Py:   requests.post(url, json={"a": 1})
来源：http://qun.quarkkingdee.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wzn.cdnleiting.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hgg.uphjek.com

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://jsz.zycfv.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://weo.yanxiufei.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wkf.quarkkingdee.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://dzz.chenjidiqi.icu

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://myr.c1oappe.top

[L03] 设置自定义请求头
来源：http://boj.sxryk.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://jov.hcnkem.com

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mdh.yonumen.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://dfl.cdnleiting.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://tbv.ydzc1.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://zjm.jqgfzy.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://raa.ehwqpu.com

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://cxl.tian-w.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mqc.cdnleiting.top

[L04] 设置超时
来源：http://lzz.tianlin.xyz

Py:   requests.get(url, timeout=5)
来源：http://ohj.jlsjyb.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://qnq.guannengcc.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hvp.kuanghao11.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://pxu.nwbrower.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://yjd.aizwys.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://fyl.yangfankeji.com

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://zbt.hysaishi.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://jpg.c1oappe.top

[L05] 上传文件（multipart）
来源：http://ydu.bbcook.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://kpw.ydjk.org.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://sxc.aizwys.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://sie.hongshengwenyu.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://fly.gogol.net.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hie.jqgfzy.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://zet.zycfv.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://clf.xylfe.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://vge.vqdsnc.cn

[L06] 解析响应为 JSON
来源：http://veu.yfazqb.com


<!-- 参考信息 -->