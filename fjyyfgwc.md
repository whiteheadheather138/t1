代发 wailian999

================================================================================
来源：http://qpq.xylfe.cn

I. 正则表达式
来源：http://nal.xziqi.cn

================================================================================
来源：http://mnh.aizwys.cn

[I01] 判断是否匹配
来源：http://xaa.vehdjk.com

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://srr.mhx1999.top

PHP:  preg_match('/\d+/', $s);
来源：http://bkp.sxryk.cn

JS:   /\d+/.test(s)
来源：http://fwq.yj202588.top

TS:   /\d+/.test(s)
来源：http://dro.vehdjk.com

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hha.ywan-chungtsiang.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wva.ydjk.org.cn

Ruby: s.match?(/\d+/)
来源：http://nnc.daria6918.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://mlv.haohaochexian.top

[I02] 提取所有匹配
来源：http://dna.cdnleiting.top

Py:   re.findall(r"\d+", s)
来源：http://ezy.snrcjt.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://odv.chenzaomai.com

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ofv.aizwys.cn

TS:   s.match(/\d+/g)
来源：http://gxi.hcnkem.com

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://xfk.uphjek.com

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ymj.zhaomingkeji.xyz

Ruby: s.scan(/\d+/)
来源：http://kby.yueranfly.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://mst.xylfe.cn

[I03] 提取捕获分组
来源：http://rcs.shangyingyoupin.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://nbx.cucudq.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://mai.vehdjk.com

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://fwe.svipenyu.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://tsw.jqgufenzy.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://cuu.dashuyun.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://tvs.tanke756.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://bgg.sweek.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://toy.zhiwuduotai.top

[I04] 正则替换
来源：http://mez.wangshuangyany.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://kba.yj20258888.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://aca.wangdashe.top

JS:   s.replace(/\d+/g, "#")
来源：http://rha.52xcode.cn

TS:   s.replace(/\d+/g, "#")
来源：http://liu.fengsongda.top

Java: s.replaceAll("\\d+", "#")
来源：http://tya.hcnkem.com

Go:   re.ReplaceAllString(s, "#")
来源：http://hxl.jinqigfzy.top

Ruby: s.gsub(/\d+/, "#")
来源：http://zzh.c1oappe.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://kzz.dashuyun.cn

[I05] 按正则拆分
来源：http://ahq.jyoumei.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://fon.hnxiangtu.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://pbc.wangdashe.top

JS:   s.split(/\s*,\s*/)
来源：http://jsc.hcnkem.com

TS:   s.split(/\s*,\s*/)
来源：http://qlv.xylfe.cn

Java: s.split("\\s*,\\s*")
来源：http://djp.zhixingplan.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://vqv.kuanghao11.cn

Ruby: s.split(/\s*,\s*/)
来源：http://kib.yfazqb.com

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hau.jyoumei.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://mvq.tianlin.xyz

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://rdw.zhongyouzk.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://gya.mhx1999.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hld.zycfv.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://srr.yvedp.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://uag.xuanzx.com

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://xla.xziqi.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hnh.uphjek.com

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://eef.zycfv.cn

[I07] 忽略大小写与多行模式
来源：http://eez.yanxiufei.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://xid.xingfuxueyuan.xyz

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://qhf.0kj1m.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ajr.gaohongyu789.top

TS:   /error/gim
来源：http://kuq.hywenlv.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://yrh.fengsongda.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://jef.xziqi.cn

Ruby: s.scan(/error/i)
来源：http://bce.jiagoushi.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://wmu.mhx1999.top

[I08] 贪婪与非贪婪匹配
来源：http://mso.9152youxi.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://mod.zhixingplan.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://yii.hesvh.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://yln.redwolf501.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://oap.shangyingyoupin.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://wxi.meibo888.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://yel.tianlin.xyz

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://gii.jinyuanbaomall.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hmt.sjlbkw.cn

================================================================================
来源：http://kge.zhixingplan.top

J. 日期与时间
来源：http://dyy.fzhhl.top

================================================================================
来源：http://pep.zhongyouzk.top

[J01] 获取当前时间
来源：http://mzh.xuetiantiany.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://vut.uphjek.com

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://pnr.cheryme.top

JS:   new Date();  Date.now()
来源：http://ddc.hongshengwenyu.top

TS:   new Date();  Date.now()
来源：http://pcz.zycfv.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://abq.yuxming.cn

Go:   time.Now()
来源：http://nvl.cheryme.top

Ruby: Time.now
来源：http://loy.fanxiaobao.xyz

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://uqo.yongpay.top

[J02] 格式化输出
来源：http://hzn.sweek.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://sca.havefunace.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://uvl.pengpengdd.cyou

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://rwk.smart0.xyz

TS:   d.toISOString()
来源：http://ylu.meibo888.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://gie.ydjk.org.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://yve.tianlin.xyz

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mol.dianchejie.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://spy.dianchejie.cn

[J03] 字符串解析为日期
来源：http://oua.hesvh.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://eug.xingfuxueyuan.xyz

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://dzn.guannengcc.top

JS:   new Date("2024-01-02")
来源：http://gti.zdqjudy.top

TS:   new Date("2024-01-02")
来源：http://cfg.yongpay.top

Java: LocalDate.parse("2024-01-02")
来源：http://ryu.ivvv.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://fvb.ybcxt.top

Ruby: Date.parse("2024-01-02")
来源：http://kri.mhx1999.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://oyc.yj202588.top

[J04] 时间戳与日期互转
来源：http://zve.yuxming.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://wdp.ctjpmb.com

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ufl.ywan-chungtsiang.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://wet.haohaochexian.top

TS:   Math.floor(Date.now() / 1000)
来源：http://zfe.birdmap.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://lvs.xingfuxueyuan.xyz

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ode.yonumen.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hip.zhengqikj.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://pco.jianghu66.top

[J05] 时间加减（加 7 天）
来源：http://hab.haohaochexian.top

Py:   now + timedelta(days=7)
来源：http://gkp.smart0.xyz

PHP:  (new DateTime())->modify("+7 days");
来源：http://hie.bbcook.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://aoq.nwbrower.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://vom.yvedp.cn

Java: LocalDate.now().plusDays(7)
来源：http://uul.ppjwa.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://txh.epnwcf.com

Ruby: Time.now + 7 * 86400
来源：http://jaf.hcnkem.com

C#:   DateTime.Now.AddDays(7)
来源：http://zax.hesvh.cn

[J06] 计算两时间之差
来源：http://fso.yuanzhike.top

Py:   (end - start).total_seconds()
来源：http://jzj.hnqzz.top

PHP:  $end->diff($start)->days;
来源：http://hwi.316326.xyz

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://lvg.hammf.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://snj.tianlin.xyz

Java: Duration.between(start, end).toSeconds()
来源：http://mik.zhoulong.xyz

Go:   end.Sub(start).Hours()
来源：http://rnv.hnqzz.top

Ruby: end - start                 # 返回秒数
来源：http://zzn.cheryme.top

C#:   (end - start).TotalSeconds
来源：http://hio.ehwqpu.com

[J07] 比较两个日期
来源：http://bpk.jinghuilouyu.cn

Py:   d1 < d2;  d1 == d2
来源：http://eqy.dianchejie.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://xec.yuxming.cn

JS:   d1.getTime() < d2.getTime()
来源：http://wlc.jqgufenzy.top

TS:   d1.getTime() < d2.getTime()
来源：http://biq.tian-w.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ffy.xuanzx.com

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://zpo.yueranfly.top

Ruby: d1 < d2;  d1 == d2
来源：http://tup.bjfxy.top

C#:   d1 < d2;  d1 == d2
来源：http://ukl.xuanzx.com

[J08] 提取年月日与星期
来源：http://yzb.haohaochexian.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://guk.9152youxi.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://fwy.jqgfzy.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://vri.chenlongwang.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://gha.hammf.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://oyg.cqqwz.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ppw.smart0.xyz

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://mgl.jianghu66.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://mnv.dashuyun.cn

[J09] 时区处理
来源：http://sae.jyoumei.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://clr.yangfankeji.com

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://kee.316326.xyz

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://uio.chenzaomai.com

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://pvi.chenzaomai.com

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://khp.hesvh.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hnz.vqdsnc.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://xmy.ctjpmb.com

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://xxt.ywan-chungtsiang.top

[J10] 取今天 / 本月第一天
来源：http://eje.shzxlz.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://zvo.jinqigufen.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://rli.zhaomingkeji.xyz

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://fcv.shuidangran.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://yoj.fzhhl.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ufk.feifeiyinyue.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://dlq.hywenlv.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://tas.fanxiaobao.xyz

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://cfm.xylfe.cn

================================================================================
来源：http://uxa.havefunace.top

K. JSON 与序列化
来源：http://umr.gaohongyu789.top

================================================================================
来源：http://xxn.jyoumei.cn

[K01] 对象转 JSON 字符串
来源：http://wfr.havefunace.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://uod.wangdashe.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://xxt.fengsongda.top

JS:   JSON.stringify(obj)
来源：http://obw.dianchejie.cn

TS:   JSON.stringify(obj)
来源：http://reo.fktsv.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://fnw.cdnleiting.top

Go:   json.Marshal(obj)
来源：http://gbw.cqqwz.cn

Ruby: obj.to_json                                     // require "json"
来源：http://grd.zdqjudy.top

C#:   JsonSerializer.Serialize(obj)
来源：http://ink.zhijiandao.cn

[K02] JSON 字符串转对象
来源：http://awh.gzhubu.top

Py:   json.loads(s)
来源：http://axc.shanyushiyangkeji.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://wsq.316326.xyz

JS:   JSON.parse(s)
来源：http://btl.pengpengdd.cyou

TS:   JSON.parse(s)
来源：http://ntt.jqgfzy.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://xbb.hfpthk.cn

Go:   json.Unmarshal(data, &v)
来源：http://euk.ydjk.org.cn

Ruby: JSON.parse(s)
来源：http://gaj.fengsongda.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://lvo.guowangkeji.top

[K03] JSON 美化输出（带缩进）
来源：http://pva.jiagoushi.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hhx.snrcjt.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ror.hammf.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://dja.gaohongyu789.top

TS:   JSON.stringify(obj, null, 2)
来源：http://yfb.hongshengwenyu.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ten.meibo888.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://yck.zhongyouzk.top

Ruby: JSON.pretty_generate(obj)
来源：http://fgd.uphjek.com

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ish.sysykeji.top

[K04] 读取 JSON 文件
来源：http://uug.yueranfly.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://tij.aibaodan.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://gli.yanxiufei.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://qkd.haohaochexian.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://lgm.fzhhl.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://nsq.0kj1m.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://rja.yj20258.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://wez.yvedp.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hin.pengpengdd.cyou

[K05] 深拷贝对象
来源：http://vvj.cheryme.top

Py:   copy.deepcopy(obj)
来源：http://gqr.jinqigufen.top

PHP:  unserialize(serialize($obj));
来源：http://kyl.sxryk.cn

JS:   structuredClone(obj)
来源：http://gfa.nanxuanxn.top

TS:   structuredClone(obj)
来源：http://mrx.zhixingplan.top

Java: // 手写拷贝构造，或序列化往返
来源：http://poo.meibo888.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://xex.ybcxt.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://gau.0kj1m.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://pos.yj20258.top

[K06] 解析 URL 查询串
来源：http://ppj.zycfv.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hiq.shangyingyoupin.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://tpx.nanxuanxn.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://cir.yuxming.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://kxd.xylfe.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://taa.yvedp.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://bcx.ydjk.org.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://kbw.hnxiangtu.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://dss.hywenlv.cn

[K07] 进制转换
来源：http://bxw.xingfuxueyuan.xyz

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://gyt.quarkkingdee.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hki.xingfuxueyuan.xyz

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ecn.gogol.net.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://nbo.zhaomingkeji.xyz

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://axo.redwolf501.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://pwy.xinyue.icu

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://wsz.fengsongda.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://jns.haohaochexian.top

[K08] 二进制序列化（非 JSON）
来源：http://ctt.haohaochexian.top

Py:   pickle.dumps(obj)
来源：http://ooe.daria6918.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://akm.gaohongyu789.top

JS:   v8.serialize(obj)        // Node
来源：http://aha.dashuyun.cn

TS:   v8.serialize(obj)        // Node
来源：http://msw.quarkkingdee.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://oec.hnxiangtu.top

Go:   encoding/gob
来源：http://vcu.shanyushiyangkeji.top

Ruby: Marshal.dump(obj)
来源：http://qrw.yj20258888.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://vvu.wangdashe.top

================================================================================
来源：http://woq.xuanzx.com

L. 网络请求
来源：http://aob.ivvv.top

================================================================================
来源：http://qng.yfazqb.com

[L01] 发送 GET 请求
来源：http://rrc.sxryk.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hrj.dianchejie.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://csg.zhiwuduotai.top

JS:   await fetch(url)
来源：http://qhb.cqqwz.cn

TS:   await fetch(url)
来源：http://vmk.hywenlv.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hjp.uphjek.com

Go:   resp, err := http.Get(url)
来源：http://sto.ybcxt.top

Ruby: Net::HTTP.get(URI(url))
来源：http://jdz.c1oappe.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://nsa.jianghu66.top

[L02] 发送 POST JSON
来源：http://iph.feifeiyinyue.top

Py:   requests.post(url, json={"a": 1})
来源：http://gab.9152youxi.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://yrt.yangfankeji.com

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ckh.bjfxy.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://zba.gaohongyu789.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://vqa.aizwys.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://oot.ivvv.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://rwd.chenzaomai.com

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://pko.hnqzz.top

[L03] 设置自定义请求头
来源：http://oeq.aizwys.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ibe.sysykeji.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://myg.ywan-chungtsiang.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://awp.zhiwuduotai.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://zuy.9152youxi.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://pfu.zdbjq.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://pgn.smart0.xyz

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://nvf.snrcjt.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://klz.chenlongwang.top

[L04] 设置超时
来源：http://zqg.pycfn.com

Py:   requests.get(url, timeout=5)
来源：http://ibh.tian-w.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://lgq.cheryme.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mwk.nanxuanxn.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://qqt.mhx1999.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mun.zdqjudy.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://usl.sufxvd.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://gxy.hammf.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://fhc.shuidangran.top

[L05] 上传文件（multipart）
来源：http://vkj.zhaomingkeji.xyz

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://aht.zhengqikj.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://awb.ppjwa.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://osi.birdmap.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://pnh.ydjk.org.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mrr.shanyushiyangtech.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://gaf.gotoacloud.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://zdg.hcnkem.com

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://xwk.nwbrower.top

[L06] 解析响应为 JSON
来源：http://brn.cdnleiting.top

Py:   resp.json()
来源：http://bne.hesvh.cn

PHP:  json_decode($body, true);
来源：http://olb.jinqigfzy.top

JS:   await resp.json()
来源：http://oim.zhixingplan.top

TS:   await resp.json()
来源：http://ilr.fzhhl.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://cyc.zhaomingkeji.xyz

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://dqa.gzhubu.top

Ruby: JSON.parse(resp.body)
来源：http://fxf.dashuyun.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://bgf.cheryme.top


<!-- 参考信息 -->