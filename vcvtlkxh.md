代发 wailian999

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mbw.tanke756.top

Ruby: raise MyError.new("fail", 500)
来源：http://esv.bjfxy.top

C#:   // 自定义异常类中加 Code 属性
来源：http://gdf.shzxlz.cn

[H10] 资源自动释放
来源：http://nkw.fanxiaobao.xyz

Py:   with open("a.txt") as f: data = f.read()
来源：http://xgl.guowangkeji.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://mwi.xziqi.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://dpf.dashuyun.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://smf.kuanghao11.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wpq.cucudq.cn

Go:   defer f.Close()
来源：http://sgc.jqgfzy.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://vjs.0kj1m.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://kvf.bjfxy.top

================================================================================
来源：http://rlz.yonumen.top

I. 正则表达式
来源：http://tdb.hesvh.cn

================================================================================
来源：http://iaj.zhaomingkeji.xyz

[I01] 判断是否匹配
来源：http://fac.guowangkeji.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://jqr.zhongyouzk.top

PHP:  preg_match('/\d+/', $s);
来源：http://hun.quarkkingdee.top

JS:   /\d+/.test(s)
来源：http://dzh.zhixingplan.top

TS:   /\d+/.test(s)
来源：http://vcn.smart0.xyz

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://drx.fzhhl.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://zco.tianlin.xyz

Ruby: s.match?(/\d+/)
来源：http://eoh.hywenlv.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ghn.feifeiyinyue.top

[I02] 提取所有匹配
来源：http://jww.sysykeji.top

Py:   re.findall(r"\d+", s)
来源：http://fai.tarul.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://pyk.tian-w.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://pgl.ydzc1.top

TS:   s.match(/\d+/g)
来源：http://pyo.yj202588.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://tgh.fzhhl.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://fww.guowangkeji.top

Ruby: s.scan(/\d+/)
来源：http://qml.dashuyun.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://eiy.cdnleiting.top

[I03] 提取捕获分组
来源：http://pyy.xinyue.icu

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://fbx.xuanzx.com

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://gkp.zhengqikj.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ene.hnxiangtu.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://lgz.0kj1m.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://apr.jinghuilouyu.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://xop.pycfn.com

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://twy.hammf.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://lvq.ehwqpu.com

[I04] 正则替换
来源：http://wyu.cucudq.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://qzp.hcnkem.com

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ghe.xuanzx.com

JS:   s.replace(/\d+/g, "#")
来源：http://asn.yuanzhike.top

TS:   s.replace(/\d+/g, "#")
来源：http://tre.jyoumei.cn

Java: s.replaceAll("\\d+", "#")
来源：http://qch.shanyushiyangtech.top

Go:   re.ReplaceAllString(s, "#")
来源：http://dtp.jlsjyb.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://xvj.cashguo.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://zim.chenlongwang.top

[I05] 按正则拆分
来源：http://boy.cucudq.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://xqy.c1oappe.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://tlj.yuanzhike.top

JS:   s.split(/\s*,\s*/)
来源：http://pxu.sysykeji.top

TS:   s.split(/\s*,\s*/)
来源：http://ctp.jinyuanbaomall.cn

Java: s.split("\\s*,\\s*")
来源：http://fxb.zhaomingkeji.xyz

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://fov.xuetiantiany.cn

Ruby: s.split(/\s*,\s*/)
来源：http://ory.zycfv.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://aoe.wangshuangyany.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://vtj.ydjk.org.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://qix.hammf.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://kwn.nanxinkj.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ksj.cheryme.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://xpt.guannengcc.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ypo.fehbvm.com

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://uxb.nwbrower.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://xnd.hammf.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ivi.hywenlv.cn

[I07] 忽略大小写与多行模式
来源：http://rja.ehwqpu.com

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://uai.yonumen.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://gan.hysaishi.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://fby.yj20258888.top

TS:   /error/gim
来源：http://nsg.cashguo.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://eja.316326.xyz

Go:   regexp.MustCompile(`(?im)error`)
来源：http://bbd.pycfn.com

Ruby: s.scan(/error/i)
来源：http://abu.jinqigufen.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://gfi.gotoacloud.top

[I08] 贪婪与非贪婪匹配
来源：http://dft.ctjpmb.com

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://zob.xuetiantiany.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://stc.yuxming.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://pzn.cdnleiting.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ivz.pengpengdd.cyou

Java: Pattern.compile("<b>.*?</b>")
来源：http://did.jqgufenzy.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://bbv.zhixingplan.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://git.meibo888.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://oxw.cucudq.cn

================================================================================
来源：http://hga.meibo888.top

J. 日期与时间
来源：http://zib.zhijiandao.cn

================================================================================
来源：http://ysl.hnxiangtu.top

[J01] 获取当前时间
来源：http://nvf.yj20258.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://kop.cqqwz.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://suf.ybcxt.top

JS:   new Date();  Date.now()
来源：http://tqw.havefunace.top

TS:   new Date();  Date.now()
来源：http://eaz.sxryk.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://ugf.jiagoushi.top

Go:   time.Now()
来源：http://loc.gaohongyu789.top

Ruby: Time.now
来源：http://jep.dashuyun.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://vxe.dianchejie.cn

[J02] 格式化输出
来源：http://rfe.ctjpmb.com

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://gla.ehwqpu.com

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ulv.hnxiangtu.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://kbu.gotoacloud.top

TS:   d.toISOString()
来源：http://cuv.cdnleiting.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://djy.feifeiyinyue.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://klt.zhengqikj.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://cyk.pycfn.com

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://mqs.zhiwuduotai.top

[J03] 字符串解析为日期
来源：http://cdd.cqqwz.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://crc.birdmap.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://mjt.jiagoushi.top

JS:   new Date("2024-01-02")
来源：http://xhk.ehwqpu.com

TS:   new Date("2024-01-02")
来源：http://wgu.fanxiaobao.xyz

Java: LocalDate.parse("2024-01-02")
来源：http://fmu.hywenlv.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ldm.yuanzhike.top

Ruby: Date.parse("2024-01-02")
来源：http://vhm.0kj1m.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://elz.yongpay.top

[J04] 时间戳与日期互转
来源：http://szx.guannengcc.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://jpw.0kj1m.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ebv.yfazqb.com

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://sov.yanxiufei.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://msj.gogol.net.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://kbn.jqgufenzy.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hgm.mhx1999.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://fxq.c1oappe.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://kfw.tian-w.cn

[J05] 时间加减（加 7 天）
来源：http://cre.hongshengwenyu.top

Py:   now + timedelta(days=7)
来源：http://phd.meibo888.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://iej.feifeiyinyue.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://nod.tian-w.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://yuh.snrcjt.cn

Java: LocalDate.now().plusDays(7)
来源：http://hci.yfazqb.com

Go:   time.Now().AddDate(0, 0, 7)
来源：http://rxd.snrcjt.cn

Ruby: Time.now + 7 * 86400
来源：http://jdh.birdmap.top

C#:   DateTime.Now.AddDays(7)
来源：http://xcg.guannengcc.top

[J06] 计算两时间之差
来源：http://gei.yongpay.top

Py:   (end - start).total_seconds()
来源：http://mgl.tian-w.cn

PHP:  $end->diff($start)->days;
来源：http://eai.andypj.xyz

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://vqs.sjlbkw.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://kge.iojbl.cn

Java: Duration.between(start, end).toSeconds()
来源：http://hto.dashuyun.cn

Go:   end.Sub(start).Hours()
来源：http://xmi.birdmap.top

Ruby: end - start                 # 返回秒数
来源：http://hfn.gaohongyu789.top

C#:   (end - start).TotalSeconds
来源：http://zwx.dianchejie.cn

[J07] 比较两个日期
来源：http://jzq.zhixingplan.top

Py:   d1 < d2;  d1 == d2
来源：http://wpa.yj20258.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ita.fzhhl.top

JS:   d1.getTime() < d2.getTime()
来源：http://bfv.yanxiufei.cn

TS:   d1.getTime() < d2.getTime()
来源：http://nls.zhiwuduotai.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://nst.jqgufenzy.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://brb.yonumen.top

Ruby: d1 < d2;  d1 == d2
来源：http://hht.meibo888.top

C#:   d1 < d2;  d1 == d2
来源：http://ucr.zhaomingkeji.xyz

[J08] 提取年月日与星期
来源：http://hig.ydzc1.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hby.feifeiyinyue.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://fgz.fehbvm.com

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hhc.ydzc1.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://uke.yj20258888.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://too.sysykeji.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://fbn.gaohongyu789.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://xvc.uphjek.com

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://glj.uphjek.com

[J09] 时区处理
来源：http://nna.ydzc1.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://bvi.ydzc1.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://epb.yonumen.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://zxp.tanke756.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://oti.fehbvm.com

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://mtq.epnwcf.com

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://mol.cucudq.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://fzz.redwolf501.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://qqs.shzxlz.cn

[J10] 取今天 / 本月第一天
来源：http://aaq.dashuyun.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://cyj.tarul.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://cke.cheryme.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://xah.jqgufenzy.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://kwh.chenjidiqi.icu

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://vwv.shanyushiyangkeji.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://sfh.yueranfly.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://kdu.zhongyouzk.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://mge.chenjidiqi.icu

================================================================================
来源：http://jcf.zhiwuduotai.top

K. JSON 与序列化
来源：http://zlg.smart0.xyz

================================================================================
来源：http://wkt.hywenlv.cn

[K01] 对象转 JSON 字符串
来源：http://mkr.nanxuanxn.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://vrj.bjfxy.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://tma.zdqjudy.top

JS:   JSON.stringify(obj)
来源：http://xqy.gzhubu.top

TS:   JSON.stringify(obj)
来源：http://yfv.hammf.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://dxe.gaohongyu789.top

Go:   json.Marshal(obj)
来源：http://occ.zdbjq.cn

Ruby: obj.to_json                                     // require "json"
来源：http://kun.chenzaomai.com

C#:   JsonSerializer.Serialize(obj)
来源：http://usb.chenjidiqi.icu

[K02] JSON 字符串转对象
来源：http://atj.fktsv.cn

Py:   json.loads(s)
来源：http://zih.ctjpmb.com

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://jsa.52xcode.cn

JS:   JSON.parse(s)
来源：http://anc.iojbl.cn

TS:   JSON.parse(s)
来源：http://wcy.fehbvm.com

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://meh.ppjwa.cn

Go:   json.Unmarshal(data, &v)
来源：http://oan.zdbjq.cn

Ruby: JSON.parse(s)
来源：http://qpp.ppjwa.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://tfb.fzhhl.top

[K03] JSON 美化输出（带缩进）
来源：http://jyt.tianlin.xyz

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://zhy.hesvh.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://prj.cqqwz.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://ckh.vqdsnc.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://ufv.9152youxi.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://knl.yfazqb.com

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://aus.jqgufenzy.top

Ruby: JSON.pretty_generate(obj)
来源：http://hml.vqdsnc.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://eab.cqqwz.cn

[K04] 读取 JSON 文件
来源：http://yiv.havefunace.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://exv.cdnleiting.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hyc.jqgufenzy.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://gfn.jinghuilouyu.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ash.gogol.net.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://sei.shangyingyoupin.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://clc.zhixingplan.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://ulo.sxryk.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ynu.chenlongwang.top

[K05] 深拷贝对象
来源：http://zwi.sjlbkw.cn

Py:   copy.deepcopy(obj)
来源：http://nib.zhongyouzk.top

PHP:  unserialize(serialize($obj));
来源：http://nzp.0kj1m.cn

JS:   structuredClone(obj)
来源：http://jjg.jinqigfzy.top

TS:   structuredClone(obj)
来源：http://rqx.hongshengwenyu.top

Java: // 手写拷贝构造，或序列化往返
来源：http://slp.xylfe.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://abu.gaohongyu789.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://gxa.quarkkingdee.top

C#:   // 序列化往返，或自定义 Clone
来源：http://nzy.uphjek.com

[K06] 解析 URL 查询串
来源：http://fyd.hnqzz.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://cjz.ybcxt.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://suv.yonumen.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://bud.jinqigufen.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://tvs.hnxiangtu.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://pjd.nanxinkj.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://uqm.tianlin.xyz

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://uyw.wangshuangyany.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://sru.yvedp.cn

[K07] 进制转换
来源：http://vgq.dashuyun.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://uah.jiagoushi.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://vbp.smart0.xyz

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://fha.jinyuanbaomall.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://qfq.sufxvd.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://gaq.xziqi.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://umz.hnqzz.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://gec.hnqzz.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://zvf.hywenlv.cn

[K08] 二进制序列化（非 JSON）
来源：http://vjs.jqgufenzy.top

Py:   pickle.dumps(obj)
来源：http://kqr.tarul.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://bgs.hywenlv.cn

JS:   v8.serialize(obj)        // Node
来源：http://pem.xylfe.cn

TS:   v8.serialize(obj)        // Node
来源：http://upd.hcnkem.com

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ugw.birdmap.top

Go:   encoding/gob
来源：http://ozg.nanxinkj.top

Ruby: Marshal.dump(obj)
来源：http://aqe.9152youxi.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://jfe.ehwqpu.com

================================================================================
来源：http://jbc.fengsongda.top

L. 网络请求
来源：http://fuv.chenlongwang.top

================================================================================
来源：http://zrl.jqgufenzy.top

[L01] 发送 GET 请求
来源：http://nca.hammf.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://zod.ydzc1.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://kum.zycfv.cn

JS:   await fetch(url)
来源：http://tod.shanyushiyangtech.top

TS:   await fetch(url)
来源：http://obl.sxryk.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://dob.snrcjt.cn

Go:   resp, err := http.Get(url)
来源：http://uar.xingfuxueyuan.xyz

Ruby: Net::HTTP.get(URI(url))
来源：http://nxo.zhixingplan.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://xxr.ydjk.org.cn

[L02] 发送 POST JSON
来源：http://phm.birdmap.top

Py:   requests.post(url, json={"a": 1})
来源：http://rhx.xingfuxueyuan.xyz

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://abb.jinqigfzy.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://gtg.xuanzx.com

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hiq.aibaodan.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://myv.hnxiangtu.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://fal.jinghuilouyu.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://nkj.iojbl.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://qho.smart0.xyz

[L03] 设置自定义请求头
来源：http://lrm.bjfxy.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://quo.yonumen.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://gut.fzhhl.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hoq.hysaishi.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://bct.meibo888.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://qzc.kuanghao11.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://cqp.tianlin.xyz

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://zfv.cucudq.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://eeo.nwbrower.top

[L04] 设置超时
来源：http://xps.fktsv.cn

Py:   requests.get(url, timeout=5)
来源：http://gfz.xziqi.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ofr.aizwys.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://amf.c1oappe.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://aid.jqgufenzy.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wjd.tian-w.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://nwt.gogol.net.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://moo.hesvh.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://gel.shuidangran.top

[L05] 上传文件（multipart）
来源：http://qmr.cucudq.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://gru.gogol.net.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://nqb.sxryk.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://kju.hammf.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://rzj.shzxlz.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wdi.havefunace.top


<!-- 参考信息 -->