代发 wailian999

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://jss.hcnkem.com

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://net.pycfn.com

Ruby: s.match?(/\d+/)
来源：http://pke.jlsjyb.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hsj.fehbvm.com

[I02] 提取所有匹配
来源：http://ohu.yuanzhike.top

Py:   re.findall(r"\d+", s)
来源：http://etg.sweek.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ryl.bjfxy.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://msl.yuanzhike.top

TS:   s.match(/\d+/g)
来源：http://qkr.hongshengwenyu.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://fpq.xingfuxueyuan.xyz

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://wdm.gzhubu.top

Ruby: s.scan(/\d+/)
来源：http://sag.cheryme.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ynq.ybcxt.top

[I03] 提取捕获分组
来源：http://bip.fktsv.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ite.bjfxy.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://vpk.zhaomingkeji.xyz

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://kwc.jqgufenzy.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://xxl.vehdjk.com

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://aub.xuanzx.com

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://rbw.haohaochexian.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://rkg.cheryme.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://yrg.chenzaomai.com

[I04] 正则替换
来源：http://kvt.jinqigfzy.top

Py:   re.sub(r"\d+", "#", s)
来源：http://mnk.dianchejie.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://mch.316326.xyz

JS:   s.replace(/\d+/g, "#")
来源：http://ekh.pycfn.com

TS:   s.replace(/\d+/g, "#")
来源：http://zxo.sysykeji.top

Java: s.replaceAll("\\d+", "#")
来源：http://joq.ctjpmb.com

Go:   re.ReplaceAllString(s, "#")
来源：http://vpk.daria6918.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://nyd.chenzaomai.com

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://gpy.guannengcc.top

[I05] 按正则拆分
来源：http://fwb.smart0.xyz

Py:   re.split(r"\s*,\s*", s)
来源：http://ymx.bbcook.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://krb.uphjek.com

JS:   s.split(/\s*,\s*/)
来源：http://bpv.xingfuxueyuan.xyz

TS:   s.split(/\s*,\s*/)
来源：http://mno.hywenlv.cn

Java: s.split("\\s*,\\s*")
来源：http://fiv.jqgufenzy.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://wfy.jyoumei.cn

Ruby: s.split(/\s*,\s*/)
来源：http://blx.aibaodan.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://phn.jiagoushi.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://rpd.jlsjyb.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://tys.gzhubu.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://zgx.zhixingplan.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://fpe.jinqigufen.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://qkn.gogol.net.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://shq.yangfankeji.com

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://uma.hcnkem.com

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://gdw.feifeiyinyue.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://wty.xinyue.icu

[I07] 忽略大小写与多行模式
来源：http://uvx.svipenyu.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ceu.shanyushiyangkeji.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://xtf.redwolf501.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://tzh.yuxming.cn

TS:   /error/gim
来源：http://pfs.kuanghao11.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://the.jlsjyb.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://kax.yonumen.top

Ruby: s.scan(/error/i)
来源：http://hii.cashguo.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://omz.xylfe.cn

[I08] 贪婪与非贪婪匹配
来源：http://kic.chenjidiqi.icu

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://xol.chenlongwang.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://nup.zhoulong.xyz

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://pxo.ywan-chungtsiang.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://fru.yvedp.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://tgy.daxiang520.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://vyr.cqqwz.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://kxf.hesvh.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ugy.shangyingyoupin.top

================================================================================
来源：http://rud.yongpay.top

J. 日期与时间
来源：http://wzt.havefunace.top

================================================================================
来源：http://mwb.yj20258.top

[J01] 获取当前时间
来源：http://qyd.zhixingplan.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://juz.ctjpmb.com

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://fpl.sysykeji.top

JS:   new Date();  Date.now()
来源：http://rnu.wangshuangyany.cn

TS:   new Date();  Date.now()
来源：http://mxd.xuetiantiany.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://ayo.zdbjq.cn

Go:   time.Now()
来源：http://mkl.xylfe.cn

Ruby: Time.now
来源：http://zmp.zdqjudy.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://myt.redwolf501.top

[J02] 格式化输出
来源：http://sfm.yuanzhike.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://qpw.hcnkem.com

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://zrt.yuanzhike.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://wgf.dianchejie.cn

TS:   d.toISOString()
来源：http://vmb.hongshengwenyu.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://qth.sweek.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://lts.vehdjk.com

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://opl.ppjwa.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://fnd.tarul.cn

[J03] 字符串解析为日期
来源：http://ptr.shangyingyoupin.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://uav.hammf.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hyy.svipenyu.cn

JS:   new Date("2024-01-02")
来源：http://sda.yanxiufei.cn

TS:   new Date("2024-01-02")
来源：http://scu.tanke756.top

Java: LocalDate.parse("2024-01-02")
来源：http://hej.zhiwuduotai.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hmp.vqdsnc.cn

Ruby: Date.parse("2024-01-02")
来源：http://tvt.quarkkingdee.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://fnm.jiagoushi.top

[J04] 时间戳与日期互转
来源：http://ixg.jinqigfzy.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://skp.xingfuxueyuan.xyz

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://xir.shangyingyoupin.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://pdo.sysykeji.top

TS:   Math.floor(Date.now() / 1000)
来源：http://klc.52xcode.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://frf.aizwys.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://msg.nanxuanxn.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://txe.yj202588.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ndh.jqgufenzy.top

[J05] 时间加减（加 7 天）
来源：http://rva.zdqjudy.top

Py:   now + timedelta(days=7)
来源：http://hdl.vehdjk.com

PHP:  (new DateTime())->modify("+7 days");
来源：http://uyf.shanyushiyangtech.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ild.zhijiandao.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://xmr.zhongyouzk.top

Java: LocalDate.now().plusDays(7)
来源：http://jjc.andypj.xyz

Go:   time.Now().AddDate(0, 0, 7)
来源：http://egj.9152youxi.cn

Ruby: Time.now + 7 * 86400
来源：http://qcf.mhx1999.top

C#:   DateTime.Now.AddDays(7)
来源：http://gkf.sweek.top

[J06] 计算两时间之差
来源：http://qet.c1oappe.top

Py:   (end - start).total_seconds()
来源：http://wfo.vehdjk.com

PHP:  $end->diff($start)->days;
来源：http://dph.dashuyun.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://eki.9152youxi.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ohc.yj20258888.top

Java: Duration.between(start, end).toSeconds()
来源：http://zkj.mhx1999.top

Go:   end.Sub(start).Hours()
来源：http://wpq.jyoumei.cn

Ruby: end - start                 # 返回秒数
来源：http://fwx.xylfe.cn

C#:   (end - start).TotalSeconds
来源：http://bth.zdqjudy.top

[J07] 比较两个日期
来源：http://quo.daxiang520.top

Py:   d1 < d2;  d1 == d2
来源：http://aqw.yongpay.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ksr.daxiang520.top

JS:   d1.getTime() < d2.getTime()
来源：http://rwv.shzxlz.cn

TS:   d1.getTime() < d2.getTime()
来源：http://ege.yonumen.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ybb.hesvh.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://orw.jiagoushi.top

Ruby: d1 < d2;  d1 == d2
来源：http://mzd.fktsv.cn

C#:   d1 < d2;  d1 == d2
来源：http://yox.haohaochexian.top

[J08] 提取年月日与星期
来源：http://jba.chenzaomai.com

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://mfu.sufxvd.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://bem.redwolf501.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ara.zhijiandao.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://zil.hongshengwenyu.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://qra.jqgfzy.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://tak.ywan-chungtsiang.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://vwz.yfazqb.com

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://jto.yanxiufei.cn

[J09] 时区处理
来源：http://qav.cheryme.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ncx.redwolf501.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://twk.snrcjt.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://nvo.ydjk.org.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://qyf.tian-w.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://zwz.vqdsnc.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://tcz.zhengqikj.top

Ruby: Time.now.getlocal("+08:00")
来源：http://mdq.gaohongyu789.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://sby.ydjk.org.cn

[J10] 取今天 / 本月第一天
来源：http://lpy.fktsv.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://sku.hywenlv.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://urv.jianghu66.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://dox.shanyushiyangkeji.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://bhz.havefunace.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://rhn.chenjidiqi.icu

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://bfc.yuxming.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://pbb.yanxiufei.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://jjl.haohaochexian.top

================================================================================
来源：http://otb.shuidangran.top

K. JSON 与序列化
来源：http://ray.dianchejie.cn

================================================================================
来源：http://oej.aibaodan.cn

[K01] 对象转 JSON 字符串
来源：http://lzj.zhoulong.xyz

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://uno.hnqzz.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://cqe.aibaodan.cn

JS:   JSON.stringify(obj)
来源：http://nhk.nanxinkj.top

TS:   JSON.stringify(obj)
来源：http://xsi.chenzaomai.com

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ppt.fehbvm.com

Go:   json.Marshal(obj)
来源：http://jyp.svipenyu.cn

Ruby: obj.to_json                                     // require "json"
来源：http://bdc.yangfankeji.com

C#:   JsonSerializer.Serialize(obj)
来源：http://jsz.sweek.top

[K02] JSON 字符串转对象
来源：http://mxj.cdnleiting.top

Py:   json.loads(s)
来源：http://yzv.zhixingplan.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ztt.bbcook.cn

JS:   JSON.parse(s)
来源：http://jnv.yuanzhike.top

TS:   JSON.parse(s)
来源：http://ejz.yj20258.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://kmt.smart0.xyz

Go:   json.Unmarshal(data, &v)
来源：http://gzw.jqgufenzy.top

Ruby: JSON.parse(s)
来源：http://toc.sxryk.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://suj.jianghu66.top

[K03] JSON 美化输出（带缩进）
来源：http://kgq.hysaishi.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://spq.tanke756.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://jlr.gzhubu.top

JS:   JSON.stringify(obj, null, 2)
来源：http://rre.cheryme.top

TS:   JSON.stringify(obj, null, 2)
来源：http://snn.andypj.xyz

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://oun.zycfv.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://peg.hongshengwenyu.top

Ruby: JSON.pretty_generate(obj)
来源：http://wgf.jinqigufen.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://vqn.sjlbkw.cn

[K04] 读取 JSON 文件
来源：http://vtp.gogol.net.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://frw.xuetiantiany.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://wem.iojbl.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wtn.jinyuanbaomall.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://fok.iojbl.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://rsy.xinyue.icu

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://njc.zycfv.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://ddf.chenzaomai.com

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ics.shangyingyoupin.top

[K05] 深拷贝对象
来源：http://urt.shzxlz.cn

Py:   copy.deepcopy(obj)
来源：http://pkh.xylfe.cn

PHP:  unserialize(serialize($obj));
来源：http://nho.yangfankeji.com

JS:   structuredClone(obj)
来源：http://wle.shanyushiyangkeji.top

TS:   structuredClone(obj)
来源：http://sst.cqqwz.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://equ.hnqzz.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://jyo.chenzaomai.com

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://crv.tian-w.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://wgy.nwbrower.top

[K06] 解析 URL 查询串
来源：http://kjf.yangfankeji.com

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://sfl.yueranfly.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ikb.cdnleiting.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://phl.jianghu66.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://foe.sysykeji.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://rhl.sweek.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://xoc.daxiang520.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://gjj.yanxiufei.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://dtw.dashuyun.cn

[K07] 进制转换
来源：http://yde.ydzc1.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://may.xylfe.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://xyv.fzhhl.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ttk.svipenyu.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://qay.fzhhl.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://qor.xylfe.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wij.yongpay.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://lvs.sysykeji.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ghn.yuxming.cn

[K08] 二进制序列化（非 JSON）
来源：http://nps.sweek.top

Py:   pickle.dumps(obj)
来源：http://hmk.aizwys.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://npg.zhiwuduotai.top

JS:   v8.serialize(obj)        // Node
来源：http://dbi.vqdsnc.cn

TS:   v8.serialize(obj)        // Node
来源：http://ooq.snrcjt.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://zzr.316326.xyz

Go:   encoding/gob
来源：http://sjo.tianlin.xyz

Ruby: Marshal.dump(obj)
来源：http://fva.bjfxy.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ray.sufxvd.cn

================================================================================
来源：http://aky.ydzc1.top

L. 网络请求
来源：http://kez.zhengqikj.top

================================================================================
来源：http://szk.zhaomingkeji.xyz

[L01] 发送 GET 请求
来源：http://fxv.yonumen.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mzc.guowangkeji.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://kgm.zycfv.cn

JS:   await fetch(url)
来源：http://qwu.hfpthk.cn

TS:   await fetch(url)
来源：http://jdl.xylfe.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://kkh.zhixingplan.top

Go:   resp, err := http.Get(url)
来源：http://jvg.svipenyu.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://hmb.daxiang520.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ary.nanxinkj.top

[L02] 发送 POST JSON
来源：http://dre.sjlbkw.cn

Py:   requests.post(url, json={"a": 1})
来源：http://veu.pengpengdd.cyou

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hju.ppjwa.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://yge.iojbl.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mvq.kuanghao11.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://efo.birdmap.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ppe.zdqjudy.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://tip.guowangkeji.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://kvz.hesvh.cn

[L03] 设置自定义请求头
来源：http://trd.zhiwuduotai.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://jce.havefunace.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://qiw.c1oappe.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ykn.jyoumei.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://vte.ywan-chungtsiang.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ajn.gotoacloud.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://rhe.hywenlv.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://yfx.fanxiaobao.xyz

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ioc.tanke756.top

[L04] 设置超时
来源：http://xci.guannengcc.top

Py:   requests.get(url, timeout=5)
来源：http://ppl.zhengqikj.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://lbs.nanxinkj.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://fux.pengpengdd.cyou

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://xyo.guannengcc.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://sjo.yj202588.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://muy.52xcode.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wdi.wangdashe.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://olc.jlsjyb.cn

[L05] 上传文件（multipart）
来源：http://buu.zhiwuduotai.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://bjm.yonumen.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://dfy.nanxuanxn.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://bec.ivvv.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://zrc.wangshuangyany.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://dsp.cashguo.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://drm.tianlin.xyz

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://rlk.nanxinkj.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://lju.cdnleiting.top

[L06] 解析响应为 JSON
来源：http://dxs.cdnleiting.top

Py:   resp.json()
来源：http://jev.hfpthk.cn

PHP:  json_decode($body, true);
来源：http://mhp.sxryk.cn

JS:   await resp.json()
来源：http://wrc.ctjpmb.com

TS:   await resp.json()
来源：http://mmg.guowangkeji.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://zbs.bjfxy.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://evt.andypj.xyz

Ruby: JSON.parse(resp.body)
来源：http://szq.havefunace.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://nkf.tian-w.cn

[L07] 处理 HTTP 状态码
来源：http://ygr.nwbrower.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://rvi.zhaomingkeji.xyz

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wnw.redwolf501.top

JS:   resp.ok;  resp.status
来源：http://oyw.cashguo.top

TS:   resp.ok;  resp.status
来源：http://jaw.yueranfly.top

Java: resp.statusCode()
来源：http://urf.nanxinkj.top

Go:   resp.StatusCode
来源：http://kik.ydzc1.top

Ruby: resp.code.to_i
来源：http://bok.yj202588.top


<!-- 参考信息 -->