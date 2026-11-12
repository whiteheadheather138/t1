代发 wailian999

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://jhj.yj20258.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://zyo.jlsjyb.cn

Ruby: s.match?(/\d+/)
来源：http://zrh.gotoacloud.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://wwn.smart0.xyz

[I02] 提取所有匹配
来源：http://xds.vqdsnc.cn

Py:   re.findall(r"\d+", s)
来源：http://vvl.hysaishi.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://tfw.yueranfly.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://qjk.sweek.top

TS:   s.match(/\d+/g)
来源：http://kcy.shanyushiyangkeji.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://tly.yangfankeji.com

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://veq.zdbjq.cn

Ruby: s.scan(/\d+/)
来源：http://lgt.hywenlv.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://qnl.gzhubu.top

[I03] 提取捕获分组
来源：http://hhf.sufxvd.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ton.meibo888.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://xfc.zhiwuduotai.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://vyy.jianghu66.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://znc.yfazqb.com

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://nih.havefunace.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://nbb.cdnleiting.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ojo.xinyue.icu

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://gzp.chenzaomai.com

[I04] 正则替换
来源：http://iwf.tarul.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://quc.jinyuanbaomall.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://psr.hnxiangtu.top

JS:   s.replace(/\d+/g, "#")
来源：http://nsb.yanxiufei.cn

TS:   s.replace(/\d+/g, "#")
来源：http://yno.xuanzx.com

Java: s.replaceAll("\\d+", "#")
来源：http://fqk.tian-w.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://fcy.xinyue.icu

Ruby: s.gsub(/\d+/, "#")
来源：http://nne.yuxming.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://myp.wangdashe.top

[I05] 按正则拆分
来源：http://ksb.jlsjyb.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://mqt.jinqigfzy.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hjw.zhijiandao.cn

JS:   s.split(/\s*,\s*/)
来源：http://doh.vqdsnc.cn

TS:   s.split(/\s*,\s*/)
来源：http://csn.chenlongwang.top

Java: s.split("\\s*,\\s*")
来源：http://yhr.tarul.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://kkr.ivvv.top

Ruby: s.split(/\s*,\s*/)
来源：http://ydo.xziqi.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hbb.cheryme.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://iwx.wangshuangyany.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://dfu.pycfn.com

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://nxx.nanxuanxn.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://zvp.ybcxt.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://aat.cucudq.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://vfe.shanyushiyangtech.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://eer.quarkkingdee.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://enn.havefunace.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://uhs.hfpthk.cn

[I07] 忽略大小写与多行模式
来源：http://pir.redwolf501.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://zkc.sjlbkw.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://yay.ctjpmb.com

JS:   /error/gim；new RegExp("error", "gim")
来源：http://alb.cashguo.top

TS:   /error/gim
来源：http://ppb.zhoulong.xyz

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://bnw.shangyingyoupin.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://qfe.aibaodan.cn

Ruby: s.scan(/error/i)
来源：http://kjb.yvedp.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://tfb.xuetiantiany.cn

[I08] 贪婪与非贪婪匹配
来源：http://ayh.ydzc1.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://uuz.yuanzhike.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://okq.kuanghao11.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://sqt.iojbl.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://yly.chenzaomai.com

Java: Pattern.compile("<b>.*?</b>")
来源：http://gor.gotoacloud.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://yal.hesvh.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://icu.sufxvd.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://pvz.316326.xyz

================================================================================
来源：http://ssw.316326.xyz

J. 日期与时间
来源：http://aqz.jqgufenzy.top

================================================================================
来源：http://wld.guannengcc.top

[J01] 获取当前时间
来源：http://sns.bbcook.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://exv.hnxiangtu.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://rye.fehbvm.com

JS:   new Date();  Date.now()
来源：http://udc.zhongyouzk.top

TS:   new Date();  Date.now()
来源：http://edd.cqqwz.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://xqr.fengsongda.top

Go:   time.Now()
来源：http://shr.xylfe.cn

Ruby: Time.now
来源：http://sqg.xylfe.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://sdm.jqgufenzy.top

[J02] 格式化输出
来源：http://ewr.dianchejie.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ikl.yuxming.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ekl.sufxvd.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://huk.ybcxt.top

TS:   d.toISOString()
来源：http://pau.zhoulong.xyz

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://rmb.hysaishi.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://mgn.epnwcf.com

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://rub.andypj.xyz

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://sxq.zhijiandao.cn

[J03] 字符串解析为日期
来源：http://krq.jinqigufen.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://bcx.svipenyu.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://xlq.chenzaomai.com

JS:   new Date("2024-01-02")
来源：http://hww.guowangkeji.top

TS:   new Date("2024-01-02")
来源：http://zsw.sweek.top

Java: LocalDate.parse("2024-01-02")
来源：http://jiw.meibo888.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://qvd.zycfv.cn

Ruby: Date.parse("2024-01-02")
来源：http://ybs.shanyushiyangkeji.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://igs.ppjwa.cn

[J04] 时间戳与日期互转
来源：http://tfy.yonumen.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://fmn.hfpthk.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://jth.hywenlv.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://jrv.yueranfly.top

TS:   Math.floor(Date.now() / 1000)
来源：http://gfe.ppjwa.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://zjs.ybcxt.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://kmd.redwolf501.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://nlx.ehwqpu.com

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://xan.fengsongda.top

[J05] 时间加减（加 7 天）
来源：http://tlt.jinyuanbaomall.cn

Py:   now + timedelta(days=7)
来源：http://rzn.xingfuxueyuan.xyz

PHP:  (new DateTime())->modify("+7 days");
来源：http://xbf.sxryk.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://bdz.sweek.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://iez.snrcjt.cn

Java: LocalDate.now().plusDays(7)
来源：http://maf.xziqi.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://cmx.bjfxy.top

Ruby: Time.now + 7 * 86400
来源：http://yne.shangyingyoupin.top

C#:   DateTime.Now.AddDays(7)
来源：http://tmm.vehdjk.com

[J06] 计算两时间之差
来源：http://qjt.svipenyu.cn

Py:   (end - start).total_seconds()
来源：http://pqt.sufxvd.cn

PHP:  $end->diff($start)->days;
来源：http://foi.meibo888.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://gya.jyoumei.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://cod.ehwqpu.com

Java: Duration.between(start, end).toSeconds()
来源：http://syd.meibo888.top

Go:   end.Sub(start).Hours()
来源：http://dav.hnxiangtu.top

Ruby: end - start                 # 返回秒数
来源：http://nwc.hesvh.cn

C#:   (end - start).TotalSeconds
来源：http://ape.nwbrower.top

[J07] 比较两个日期
来源：http://rug.yj20258888.top

Py:   d1 < d2;  d1 == d2
来源：http://llv.ctjpmb.com

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://wec.yanxiufei.cn

JS:   d1.getTime() < d2.getTime()
来源：http://otn.shuidangran.top

TS:   d1.getTime() < d2.getTime()
来源：http://qac.wangdashe.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://san.dianchejie.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://egs.gogol.net.cn

Ruby: d1 < d2;  d1 == d2
来源：http://pxl.pengpengdd.cyou

C#:   d1 < d2;  d1 == d2
来源：http://oji.andypj.xyz

[J08] 提取年月日与星期
来源：http://viu.yj20258888.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://pwu.cqqwz.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://pek.pengpengdd.cyou

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://wul.zycfv.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://kaw.yuxming.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://spc.smart0.xyz

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ywq.jqgufenzy.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://aaa.cucudq.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ihf.gotoacloud.top

[J09] 时区处理
来源：http://qtj.hywenlv.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ajs.daria6918.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://rqr.andypj.xyz

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ffu.snrcjt.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hcb.sjlbkw.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://zjf.jlsjyb.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://usy.feifeiyinyue.top

Ruby: Time.now.getlocal("+08:00")
来源：http://nxs.yj20258.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://psd.iojbl.cn

[J10] 取今天 / 本月第一天
来源：http://ags.xylfe.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://jrq.iojbl.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hlg.hesvh.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://zpm.dianchejie.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://aqw.cucudq.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://utr.meibo888.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://zvg.zhongyouzk.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://nsi.aibaodan.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ftq.feifeiyinyue.top

================================================================================
来源：http://yfz.quarkkingdee.top

K. JSON 与序列化
来源：http://tjv.yj202588.top

================================================================================
来源：http://xmv.chenlongwang.top

[K01] 对象转 JSON 字符串
来源：http://hoc.mhx1999.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://igr.jinqigufen.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://lua.tianlin.xyz

JS:   JSON.stringify(obj)
来源：http://opr.hnqzz.top

TS:   JSON.stringify(obj)
来源：http://wci.wangdashe.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://lfw.hcnkem.com

Go:   json.Marshal(obj)
来源：http://fun.hnqzz.top

Ruby: obj.to_json                                     // require "json"
来源：http://lar.andypj.xyz

C#:   JsonSerializer.Serialize(obj)
来源：http://igh.ivvv.top

[K02] JSON 字符串转对象
来源：http://ixu.zhoulong.xyz

Py:   json.loads(s)
来源：http://xnl.fanxiaobao.xyz

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://oop.jlsjyb.cn

JS:   JSON.parse(s)
来源：http://vss.zhiwuduotai.top

TS:   JSON.parse(s)
来源：http://qdf.zhaomingkeji.xyz

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://fuq.tanke756.top

Go:   json.Unmarshal(data, &v)
来源：http://duk.hnqzz.top

Ruby: JSON.parse(s)
来源：http://han.shangyingyoupin.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://bxc.xuanzx.com

[K03] JSON 美化输出（带缩进）
来源：http://bwo.shangyingyoupin.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://wfx.hcnkem.com

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hza.nanxuanxn.top

JS:   JSON.stringify(obj, null, 2)
来源：http://owz.bjfxy.top

TS:   JSON.stringify(obj, null, 2)
来源：http://rwv.iojbl.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://oya.fengsongda.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://xya.chenjidiqi.icu

Ruby: JSON.pretty_generate(obj)
来源：http://tdo.hnqzz.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://daa.daxiang520.top

[K04] 读取 JSON 文件
来源：http://wwc.vqdsnc.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ygu.yj20258888.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ftv.yj20258888.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ysp.xziqi.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://kar.jyoumei.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://boj.sweek.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://von.guowangkeji.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://crf.yj20258888.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ysk.iojbl.cn

[K05] 深拷贝对象
来源：http://hag.ppjwa.cn

Py:   copy.deepcopy(obj)
来源：http://fhk.feifeiyinyue.top

PHP:  unserialize(serialize($obj));
来源：http://zpu.yanxiufei.cn

JS:   structuredClone(obj)
来源：http://qfs.fzhhl.top

TS:   structuredClone(obj)
来源：http://bmz.hammf.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://eqy.yfazqb.com

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hwq.ctjpmb.com

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://gon.zhiwuduotai.top

C#:   // 序列化往返，或自定义 Clone
来源：http://llq.xinyue.icu

[K06] 解析 URL 查询串
来源：http://gxm.fktsv.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://nlw.316326.xyz

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ijl.tian-w.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://rjc.jqgufenzy.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://zpj.vqdsnc.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ggd.jyoumei.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://lka.yonumen.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://mig.sxryk.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://lie.xuanzx.com

[K07] 进制转换
来源：http://iho.jinqigfzy.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://phe.redwolf501.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ych.aibaodan.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://mqw.zhongyouzk.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://lao.zdbjq.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://lpv.haohaochexian.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://dqp.daxiang520.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://lst.fanxiaobao.xyz

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://sng.havefunace.top

[K08] 二进制序列化（非 JSON）
来源：http://qte.sxryk.cn

Py:   pickle.dumps(obj)
来源：http://tzh.zhiwuduotai.top

PHP:  serialize($obj);  unserialize($s);
来源：http://nuf.vqdsnc.cn

JS:   v8.serialize(obj)        // Node
来源：http://tkg.sxryk.cn

TS:   v8.serialize(obj)        // Node
来源：http://yig.9152youxi.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://omk.zhengqikj.top

Go:   encoding/gob
来源：http://ckc.hnqzz.top

Ruby: Marshal.dump(obj)
来源：http://rcf.andypj.xyz

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://kgi.jyoumei.cn

================================================================================
来源：http://xvf.gogol.net.cn

L. 网络请求
来源：http://jym.ivvv.top

================================================================================
来源：http://aaf.jiagoushi.top

[L01] 发送 GET 请求
来源：http://xcr.jiagoushi.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ocx.tarul.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://dyb.havefunace.top

JS:   await fetch(url)
来源：http://hzq.jinyuanbaomall.cn

TS:   await fetch(url)
来源：http://lca.cucudq.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ruc.svipenyu.cn

Go:   resp, err := http.Get(url)
来源：http://oqd.hywenlv.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://xpz.zdbjq.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ltf.cheryme.top

[L02] 发送 POST JSON
来源：http://luw.jinqigufen.top

Py:   requests.post(url, json={"a": 1})
来源：http://xkt.andypj.xyz

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://koz.zhaomingkeji.xyz

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://rqe.fanxiaobao.xyz

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://zpm.hesvh.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://nxr.hfpthk.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ajo.daxiang520.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://rfc.xuetiantiany.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://jxq.havefunace.top

[L03] 设置自定义请求头
来源：http://byf.gaohongyu789.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://uzt.guowangkeji.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://eos.hammf.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://bmf.fehbvm.com

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://doq.shzxlz.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hyd.cashguo.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ais.jinqigufen.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://lrf.jqgfzy.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://tsy.ppjwa.cn

[L04] 设置超时
来源：http://foe.zhixingplan.top

Py:   requests.get(url, timeout=5)
来源：http://ntj.fktsv.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://xch.shangyingyoupin.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://jxf.shangyingyoupin.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mvv.sysykeji.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://lhv.xuetiantiany.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://cxq.sweek.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wmh.zhongyouzk.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://rhh.vqdsnc.cn

[L05] 上传文件（multipart）
来源：http://kcv.yanxiufei.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://gyn.daria6918.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wyl.zhijiandao.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://gdl.hnxiangtu.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://qgb.yfazqb.com

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://sot.ybcxt.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://twu.cqqwz.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://blh.haohaochexian.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://nnc.316326.xyz

[L06] 解析响应为 JSON
来源：http://uby.xziqi.cn

Py:   resp.json()
来源：http://xbq.hywenlv.cn

PHP:  json_decode($body, true);
来源：http://ofc.yueranfly.top

JS:   await resp.json()
来源：http://lqe.chenjidiqi.icu

TS:   await resp.json()
来源：http://kih.xuetiantiany.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://oav.jinqigufen.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://lmm.mhx1999.top

Ruby: JSON.parse(resp.body)
来源：http://ysq.yuxming.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://zwi.ctjpmb.com

[L07] 处理 HTTP 状态码
来源：http://ven.hcnkem.com

Py:   resp.status_code;  resp.raise_for_status()
来源：http://zaj.haohaochexian.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ufn.jinqigufen.top

JS:   resp.ok;  resp.status
来源：http://phx.zhijiandao.cn

TS:   resp.ok;  resp.status
来源：http://ckm.hnqzz.top

Java: resp.statusCode()
来源：http://mzp.hammf.cn

Go:   resp.StatusCode
来源：http://qpr.shuidangran.top

Ruby: resp.code.to_i
来源：http://wbf.nanxinkj.top


<!-- 参考信息 -->