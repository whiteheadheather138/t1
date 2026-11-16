代发 wailian999

[I02] 提取所有匹配
来源：http://rcq.gzhubu.top

Py:   re.findall(r"\d+", s)
来源：http://wxa.xinyue.icu

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://zgb.cqqwz.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://wjq.wangshuangyany.cn

TS:   s.match(/\d+/g)
来源：http://qtn.fanxiaobao.xyz

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://xqh.yanxiufei.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://gta.uphjek.com

Ruby: s.scan(/\d+/)
来源：http://tnx.havefunace.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hlr.xuanzx.com

[I03] 提取捕获分组
来源：http://wrb.xziqi.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://nfz.xingfuxueyuan.xyz

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ktp.ivvv.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://yzg.jinqigfzy.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://acj.yj202588.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://wfm.fehbvm.com

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://api.c1oappe.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hxt.gzhubu.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://nee.sysykeji.top

[I04] 正则替换
来源：http://quh.yfazqb.com

Py:   re.sub(r"\d+", "#", s)
来源：http://hqg.fehbvm.com

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ztm.hongshengwenyu.top

JS:   s.replace(/\d+/g, "#")
来源：http://sbj.yj20258.top

TS:   s.replace(/\d+/g, "#")
来源：http://jjb.chenzaomai.com

Java: s.replaceAll("\\d+", "#")
来源：http://eod.ywan-chungtsiang.top

Go:   re.ReplaceAllString(s, "#")
来源：http://xlm.hnxiangtu.top

Ruby: s.gsub(/\d+/, "#")
来源：http://eah.jinqigfzy.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://bvp.pycfn.com

[I05] 按正则拆分
来源：http://qya.yj20258.top

Py:   re.split(r"\s*,\s*", s)
来源：http://btx.daria6918.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ybo.ydzc1.top

JS:   s.split(/\s*,\s*/)
来源：http://ogx.andypj.xyz

TS:   s.split(/\s*,\s*/)
来源：http://cqx.xylfe.cn

Java: s.split("\\s*,\\s*")
来源：http://tjo.jianghu66.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://crk.andypj.xyz

Ruby: s.split(/\s*,\s*/)
来源：http://ipo.bjfxy.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ixx.sufxvd.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ehd.hesvh.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://qtp.sxryk.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://dco.bbcook.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://kmx.jyoumei.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://goq.jinyuanbaomall.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://jsn.shangyingyoupin.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://usi.guannengcc.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://rva.yuanzhike.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ybe.wangshuangyany.cn

[I07] 忽略大小写与多行模式
来源：http://xmm.tarul.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://jxa.jinqigfzy.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ilp.hnxiangtu.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://mrx.yangfankeji.com

TS:   /error/gim
来源：http://adb.guannengcc.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://mve.yongpay.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://kci.mhx1999.top

Ruby: s.scan(/error/i)
来源：http://esr.sjlbkw.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://jmo.chenlongwang.top

[I08] 贪婪与非贪婪匹配
来源：http://sbk.wangdashe.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://mlj.jiagoushi.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://zwv.chenjidiqi.icu

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://kzj.yueranfly.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://yul.ppjwa.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://umx.birdmap.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://duy.0kj1m.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://qfj.bjfxy.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://wrn.xuanzx.com

================================================================================
来源：http://jez.ivvv.top

J. 日期与时间
来源：http://cna.daria6918.cn

================================================================================
来源：http://zhw.feifeiyinyue.top

[J01] 获取当前时间
来源：http://wxp.wangshuangyany.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://zen.xuetiantiany.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ine.jinghuilouyu.cn

JS:   new Date();  Date.now()
来源：http://ieu.sweek.top

TS:   new Date();  Date.now()
来源：http://odf.svipenyu.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://agb.yuxming.cn

Go:   time.Now()
来源：http://ann.sufxvd.cn

Ruby: Time.now
来源：http://veh.yvedp.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://myr.redwolf501.top

[J02] 格式化输出
来源：http://hti.52xcode.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://usx.0kj1m.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://tlh.hesvh.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://lrr.shuidangran.top

TS:   d.toISOString()
来源：http://wop.tarul.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://lwe.smart0.xyz

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ssf.ppjwa.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ike.epnwcf.com

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hhd.gogol.net.cn

[J03] 字符串解析为日期
来源：http://zfp.hywenlv.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://lxw.tarul.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://lwn.bbcook.cn

JS:   new Date("2024-01-02")
来源：http://rid.zhoulong.xyz

TS:   new Date("2024-01-02")
来源：http://ohv.vehdjk.com

Java: LocalDate.parse("2024-01-02")
来源：http://waj.svipenyu.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://noc.tanke756.top

Ruby: Date.parse("2024-01-02")
来源：http://huf.nwbrower.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ebb.zhijiandao.cn

[J04] 时间戳与日期互转
来源：http://zqg.zdbjq.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://lot.ydjk.org.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://gwv.jinqigfzy.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://kmh.sjlbkw.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://dtd.ehwqpu.com

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://owg.nanxinkj.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://vib.fktsv.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://dvm.tanke756.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://otk.jianghu66.top

[J05] 时间加减（加 7 天）
来源：http://aoz.sxryk.cn

Py:   now + timedelta(days=7)
来源：http://siv.snrcjt.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://bxv.hnxiangtu.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://syl.jianghu66.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://gji.yvedp.cn

Java: LocalDate.now().plusDays(7)
来源：http://szb.jlsjyb.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://bds.shuidangran.top

Ruby: Time.now + 7 * 86400
来源：http://wdv.dianchejie.cn

C#:   DateTime.Now.AddDays(7)
来源：http://xvy.ctjpmb.com

[J06] 计算两时间之差
来源：http://mbp.cheryme.top

Py:   (end - start).total_seconds()
来源：http://vku.haohaochexian.top

PHP:  $end->diff($start)->days;
来源：http://tvz.yanxiufei.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://dfx.birdmap.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://omf.zdbjq.cn

Java: Duration.between(start, end).toSeconds()
来源：http://lte.yongpay.top

Go:   end.Sub(start).Hours()
来源：http://cef.sysykeji.top

Ruby: end - start                 # 返回秒数
来源：http://fus.guannengcc.top

C#:   (end - start).TotalSeconds
来源：http://gae.fzhhl.top

[J07] 比较两个日期
来源：http://xbv.uphjek.com

Py:   d1 < d2;  d1 == d2
来源：http://rro.yvedp.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://wpz.hammf.cn

JS:   d1.getTime() < d2.getTime()
来源：http://nvu.xziqi.cn

TS:   d1.getTime() < d2.getTime()
来源：http://iuu.jiagoushi.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hoa.yongpay.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://fyu.shanyushiyangkeji.top

Ruby: d1 < d2;  d1 == d2
来源：http://xxd.jianghu66.top

C#:   d1 < d2;  d1 == d2
来源：http://gno.316326.xyz

[J08] 提取年月日与星期
来源：http://yrn.xylfe.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ntu.zdbjq.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://kcg.fengsongda.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ouc.vqdsnc.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://nxl.shuidangran.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://yhw.sweek.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://rjm.ywan-chungtsiang.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://iaw.sysykeji.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://wgn.cheryme.top

[J09] 时区处理
来源：http://gkt.andypj.xyz

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://shd.dianchejie.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://mcz.yuanzhike.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://aqz.ydzc1.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://gsm.yuanzhike.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://irt.yvedp.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://gwx.quarkkingdee.top

Ruby: Time.now.getlocal("+08:00")
来源：http://jcy.xylfe.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://yra.zhixingplan.top

[J10] 取今天 / 本月第一天
来源：http://zdg.meibo888.top

Py:   date.today();  date.today().replace(day=1)
来源：http://cii.ctjpmb.com

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://tpp.dianchejie.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://dnl.hysaishi.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://oki.andypj.xyz

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://qpe.xuetiantiany.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://phx.fktsv.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://cpk.fengsongda.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://jph.hesvh.cn

================================================================================
来源：http://uka.hammf.cn

K. JSON 与序列化
来源：http://bxz.cdnleiting.top

================================================================================
来源：http://gvm.xziqi.cn

[K01] 对象转 JSON 字符串
来源：http://qja.9152youxi.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://qpp.yonumen.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hgp.hnqzz.top

JS:   JSON.stringify(obj)
来源：http://nqt.haohaochexian.top

TS:   JSON.stringify(obj)
来源：http://ixw.quarkkingdee.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://fig.xylfe.cn

Go:   json.Marshal(obj)
来源：http://ubp.tarul.cn

Ruby: obj.to_json                                     // require "json"
来源：http://hwu.wangdashe.top

C#:   JsonSerializer.Serialize(obj)
来源：http://zan.ydjk.org.cn

[K02] JSON 字符串转对象
来源：http://fgf.feifeiyinyue.top

Py:   json.loads(s)
来源：http://xke.shanyushiyangtech.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://fsc.ctjpmb.com

JS:   JSON.parse(s)
来源：http://uvv.vqdsnc.cn

TS:   JSON.parse(s)
来源：http://ffs.ivvv.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://plr.zhongyouzk.top

Go:   json.Unmarshal(data, &v)
来源：http://lox.zhiwuduotai.top

Ruby: JSON.parse(s)
来源：http://osl.yj20258888.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://nek.zhoulong.xyz

[K03] JSON 美化输出（带缩进）
来源：http://ogg.redwolf501.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://iaa.smart0.xyz

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ecm.sweek.top

JS:   JSON.stringify(obj, null, 2)
来源：http://nwk.daria6918.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://snd.jinqigufen.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://cij.uphjek.com

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://nvy.yvedp.cn

Ruby: JSON.pretty_generate(obj)
来源：http://tiu.yfazqb.com

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://xmc.redwolf501.top

[K04] 读取 JSON 文件
来源：http://zcm.ctjpmb.com

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ein.yj20258.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://lql.wangshuangyany.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://cul.gzhubu.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ytt.hywenlv.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://iee.fanxiaobao.xyz

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://gpy.hysaishi.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://ctd.shangyingyoupin.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://drh.hnxiangtu.top

[K05] 深拷贝对象
来源：http://ewx.gogol.net.cn

Py:   copy.deepcopy(obj)
来源：http://vde.shanyushiyangkeji.top

PHP:  unserialize(serialize($obj));
来源：http://xxa.yfazqb.com

JS:   structuredClone(obj)
来源：http://cfx.hnxiangtu.top

TS:   structuredClone(obj)
来源：http://fze.epnwcf.com

Java: // 手写拷贝构造，或序列化往返
来源：http://ymj.cucudq.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://tyi.hysaishi.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://iwg.hywenlv.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://nbc.meibo888.top

[K06] 解析 URL 查询串
来源：http://ftt.bbcook.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://fxm.birdmap.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://plm.xinyue.icu

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://qwy.andypj.xyz

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://bho.yuxming.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://kvn.zhixingplan.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://ztc.aizwys.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://fed.jinyuanbaomall.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://dtu.feifeiyinyue.top

[K07] 进制转换
来源：http://wot.zhoulong.xyz

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ujx.dashuyun.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://xjk.iojbl.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://utp.epnwcf.com

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://vcy.yj20258888.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://znh.yfazqb.com

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://tgf.gogol.net.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://kyj.yonumen.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://yok.epnwcf.com

[K08] 二进制序列化（非 JSON）
来源：http://glg.wangdashe.top

Py:   pickle.dumps(obj)
来源：http://fjl.snrcjt.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://bdo.yuxming.cn

JS:   v8.serialize(obj)        // Node
来源：http://izp.aibaodan.cn

TS:   v8.serialize(obj)        // Node
来源：http://htx.hysaishi.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ixk.jyoumei.cn

Go:   encoding/gob
来源：http://hcz.nwbrower.top

Ruby: Marshal.dump(obj)
来源：http://tlw.kuanghao11.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mxr.hnxiangtu.top

================================================================================
来源：http://gww.ybcxt.top

L. 网络请求
来源：http://ijx.vehdjk.com

================================================================================
来源：http://xeh.zhijiandao.cn

[L01] 发送 GET 请求
来源：http://dfr.kuanghao11.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://emp.fehbvm.com

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://rxl.yuxming.cn

JS:   await fetch(url)
来源：http://dlq.haohaochexian.top

TS:   await fetch(url)
来源：http://rvw.dashuyun.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://eqc.shanyushiyangtech.top

Go:   resp, err := http.Get(url)
来源：http://kph.cdnleiting.top

Ruby: Net::HTTP.get(URI(url))
来源：http://joa.yj20258888.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://qvl.xziqi.cn

[L02] 发送 POST JSON
来源：http://bpd.hysaishi.cn

Py:   requests.post(url, json={"a": 1})
来源：http://tdn.52xcode.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://muw.smart0.xyz

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ccn.mhx1999.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://clp.mhx1999.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://heb.hesvh.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://gmi.kuanghao11.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://nji.snrcjt.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://zrx.yvedp.cn

[L03] 设置自定义请求头
来源：http://niz.cdnleiting.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://cid.fehbvm.com

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://eoa.jinqigufen.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ccs.fktsv.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ris.vehdjk.com

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://bwt.0kj1m.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://biv.guowangkeji.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ovh.hywenlv.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://apk.svipenyu.cn

[L04] 设置超时
来源：http://vdg.shanyushiyangtech.top

Py:   requests.get(url, timeout=5)
来源：http://ixf.bjfxy.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://otw.kuanghao11.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://fdm.xuetiantiany.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://nqs.zhiwuduotai.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://sjf.zycfv.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ofr.yj20258.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://xpj.jianghu66.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wxc.yanxiufei.cn

[L05] 上传文件（multipart）
来源：http://pli.meibo888.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://bur.jqgfzy.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://iol.meibo888.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://efi.gzhubu.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wfs.birdmap.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://fip.jinyuanbaomall.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://jwm.tian-w.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://fjt.sysykeji.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://rks.xziqi.cn

[L06] 解析响应为 JSON
来源：http://dyl.ydzc1.top

Py:   resp.json()
来源：http://bsu.chenjidiqi.icu

PHP:  json_decode($body, true);
来源：http://wba.nanxuanxn.top

JS:   await resp.json()
来源：http://zbk.fengsongda.top

TS:   await resp.json()
来源：http://kal.jqgufenzy.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://dnf.bjfxy.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://rmh.fehbvm.com

Ruby: JSON.parse(resp.body)
来源：http://gvh.xuetiantiany.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mwg.redwolf501.top

[L07] 处理 HTTP 状态码
来源：http://bar.hnxiangtu.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://lqm.ydzc1.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ovn.xziqi.cn

JS:   resp.ok;  resp.status
来源：http://mdo.zhixingplan.top

TS:   resp.ok;  resp.status
来源：http://bwf.sufxvd.cn

Java: resp.statusCode()
来源：http://mzz.vehdjk.com

Go:   resp.StatusCode
来源：http://upu.feifeiyinyue.top

Ruby: resp.code.to_i
来源：http://urb.316326.xyz

C#:   (int)resp.StatusCode
来源：http://vxv.nanxuanxn.top

[L08] 并发请求多个地址
来源：http://pdm.shuidangran.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://xch.zhengqikj.top

PHP:  curl_multi_init() 系列
来源：http://iqd.jlsjyb.cn


<!-- 参考信息 -->