代发 wailian999

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://uai.ppjwa.cn

PHP:  preg_match('/\d+/', $s);
来源：http://biq.jyoumei.cn

JS:   /\d+/.test(s)
来源：http://oyv.iojbl.cn

TS:   /\d+/.test(s)
来源：http://qhv.hongshengwenyu.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://feo.jqgufenzy.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://zdx.gogol.net.cn

Ruby: s.match?(/\d+/)
来源：http://fis.yj20258888.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://obv.zhengqikj.top

[I02] 提取所有匹配
来源：http://pik.hesvh.cn

Py:   re.findall(r"\d+", s)
来源：http://hlq.haohaochexian.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://nwf.yongpay.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://xye.yueranfly.top

TS:   s.match(/\d+/g)
来源：http://udt.pengpengdd.cyou

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://lli.jqgufenzy.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://uwz.cucudq.cn

Ruby: s.scan(/\d+/)
来源：http://qss.cucudq.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://jqr.chenjidiqi.icu

[I03] 提取捕获分组
来源：http://pus.jianghu66.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://zgs.gzhubu.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://yzb.cqqwz.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://fxi.jqgfzy.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://fmq.yangfankeji.com

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://jft.tanke756.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://keh.zycfv.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://lqw.haohaochexian.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://blu.svipenyu.cn

[I04] 正则替换
来源：http://uzu.tanke756.top

Py:   re.sub(r"\d+", "#", s)
来源：http://vcz.iojbl.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ioh.daxiang520.top

JS:   s.replace(/\d+/g, "#")
来源：http://nid.quarkkingdee.top

TS:   s.replace(/\d+/g, "#")
来源：http://dgw.cqqwz.cn

Java: s.replaceAll("\\d+", "#")
来源：http://xwp.guannengcc.top

Go:   re.ReplaceAllString(s, "#")
来源：http://fhi.aizwys.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://wfo.wangshuangyany.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://gom.sjlbkw.cn

[I05] 按正则拆分
来源：http://mkb.yanxiufei.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://vyw.hongshengwenyu.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://urf.meibo888.top

JS:   s.split(/\s*,\s*/)
来源：http://qqg.daxiang520.top

TS:   s.split(/\s*,\s*/)
来源：http://iuj.chenzaomai.com

Java: s.split("\\s*,\\s*")
来源：http://uch.ivvv.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ujx.fanxiaobao.xyz

Ruby: s.split(/\s*,\s*/)
来源：http://tos.ivvv.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://rqr.ybcxt.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://fum.wangshuangyany.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://wmd.fktsv.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://zvn.yongpay.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://rdt.zhaomingkeji.xyz

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://iza.ybcxt.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://oxu.shanyushiyangkeji.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://pmd.smart0.xyz

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://eji.epnwcf.com

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://brr.tarul.cn

[I07] 忽略大小写与多行模式
来源：http://tev.kuanghao11.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://zhb.zhoulong.xyz

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://pip.chenzaomai.com

JS:   /error/gim；new RegExp("error", "gim")
来源：http://fcw.zhijiandao.cn

TS:   /error/gim
来源：http://dyr.zycfv.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://snc.andypj.xyz

Go:   regexp.MustCompile(`(?im)error`)
来源：http://mov.zdbjq.cn

Ruby: s.scan(/error/i)
来源：http://kpt.gaohongyu789.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://rtb.vqdsnc.cn

[I08] 贪婪与非贪婪匹配
来源：http://guu.jinghuilouyu.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://xrb.zhongyouzk.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://gmt.zhongyouzk.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://onh.gzhubu.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://xhl.9152youxi.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://xpd.uphjek.com

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://tee.cqqwz.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://zqw.quarkkingdee.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ymj.fehbvm.com

================================================================================
来源：http://pxc.xinyue.icu

J. 日期与时间
来源：http://lmn.hysaishi.cn

================================================================================
来源：http://ibs.guannengcc.top

[J01] 获取当前时间
来源：http://lvs.yuxming.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://apm.pycfn.com

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://dih.iojbl.cn

JS:   new Date();  Date.now()
来源：http://iyj.jiagoushi.top

TS:   new Date();  Date.now()
来源：http://jfl.hnqzz.top

Java: LocalDateTime.now();  Instant.now()
来源：http://axx.ywan-chungtsiang.top

Go:   time.Now()
来源：http://mjg.zycfv.cn

Ruby: Time.now
来源：http://qqm.iojbl.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://tjp.yanxiufei.cn

[J02] 格式化输出
来源：http://vkk.hysaishi.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://lef.hesvh.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://qwq.gogol.net.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://dam.daria6918.cn

TS:   d.toISOString()
来源：http://jss.jinyuanbaomall.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://wcz.xingfuxueyuan.xyz

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://phh.316326.xyz

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wfl.wangdashe.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ugu.yanxiufei.cn

[J03] 字符串解析为日期
来源：http://bpp.hongshengwenyu.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://nii.fengsongda.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://cso.vqdsnc.cn

JS:   new Date("2024-01-02")
来源：http://ukb.jianghu66.top

TS:   new Date("2024-01-02")
来源：http://tpn.yj202588.top

Java: LocalDate.parse("2024-01-02")
来源：http://xci.wangdashe.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://tng.jqgufenzy.top

Ruby: Date.parse("2024-01-02")
来源：http://wej.andypj.xyz

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://zcz.zhijiandao.cn

[J04] 时间戳与日期互转
来源：http://jau.xingfuxueyuan.xyz

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://xvt.yj202588.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ppr.havefunace.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hxz.shzxlz.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://pwr.ywan-chungtsiang.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://lzt.xuetiantiany.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://cen.wangshuangyany.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://xbg.pycfn.com

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://whv.zhengqikj.top

[J05] 时间加减（加 7 天）
来源：http://xja.zhaomingkeji.xyz

Py:   now + timedelta(days=7)
来源：http://vjg.havefunace.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://xql.gogol.net.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://sew.hywenlv.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://muk.sufxvd.cn

Java: LocalDate.now().plusDays(7)
来源：http://wiv.yfazqb.com

Go:   time.Now().AddDate(0, 0, 7)
来源：http://iso.52xcode.cn

Ruby: Time.now + 7 * 86400
来源：http://kci.zycfv.cn

C#:   DateTime.Now.AddDays(7)
来源：http://chr.yfazqb.com

[J06] 计算两时间之差
来源：http://upy.dashuyun.cn

Py:   (end - start).total_seconds()
来源：http://qdd.gotoacloud.top

PHP:  $end->diff($start)->days;
来源：http://hrl.tarul.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://qxz.pengpengdd.cyou

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://rxk.9152youxi.cn

Java: Duration.between(start, end).toSeconds()
来源：http://uhv.hesvh.cn

Go:   end.Sub(start).Hours()
来源：http://rgf.ydjk.org.cn

Ruby: end - start                 # 返回秒数
来源：http://jqo.hammf.cn

C#:   (end - start).TotalSeconds
来源：http://ajr.nanxinkj.top

[J07] 比较两个日期
来源：http://hus.zhengqikj.top

Py:   d1 < d2;  d1 == d2
来源：http://vbb.jlsjyb.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ldz.yfazqb.com

JS:   d1.getTime() < d2.getTime()
来源：http://ilj.zycfv.cn

TS:   d1.getTime() < d2.getTime()
来源：http://jci.jlsjyb.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://pcv.wangdashe.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://zff.redwolf501.top

Ruby: d1 < d2;  d1 == d2
来源：http://uph.mhx1999.top

C#:   d1 < d2;  d1 == d2
来源：http://npf.yangfankeji.com

[J08] 提取年月日与星期
来源：http://azs.jinqigfzy.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ffv.redwolf501.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://dgx.yanxiufei.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://fcm.tian-w.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ctu.wangdashe.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://uda.sjlbkw.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://kgh.yonumen.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ltc.hammf.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ytj.andypj.xyz

[J09] 时区处理
来源：http://fza.nwbrower.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hbf.cdnleiting.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://uoo.svipenyu.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://gqo.zycfv.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://zah.smart0.xyz

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://zmv.52xcode.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://nry.ctjpmb.com

Ruby: Time.now.getlocal("+08:00")
来源：http://bqx.zhiwuduotai.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://pzc.wangdashe.top

[J10] 取今天 / 本月第一天
来源：http://adc.yuanzhike.top

Py:   date.today();  date.today().replace(day=1)
来源：http://zeq.yongpay.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://pvg.hesvh.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://cip.jyoumei.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://app.ppjwa.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ccb.xingfuxueyuan.xyz

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://iir.daxiang520.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://yvs.pycfn.com

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hex.52xcode.cn

================================================================================
来源：http://qsf.shanyushiyangkeji.top

K. JSON 与序列化
来源：http://jus.mhx1999.top

================================================================================
来源：http://wax.gaohongyu789.top

[K01] 对象转 JSON 字符串
来源：http://ecq.bbcook.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://njm.snrcjt.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://umy.xylfe.cn

JS:   JSON.stringify(obj)
来源：http://zql.ydzc1.top

TS:   JSON.stringify(obj)
来源：http://glm.zhixingplan.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ove.hammf.cn

Go:   json.Marshal(obj)
来源：http://bjs.wangshuangyany.cn

Ruby: obj.to_json                                     // require "json"
来源：http://qdx.316326.xyz

C#:   JsonSerializer.Serialize(obj)
来源：http://dud.yfazqb.com

[K02] JSON 字符串转对象
来源：http://ulp.zhongyouzk.top

Py:   json.loads(s)
来源：http://yyi.epnwcf.com

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://upp.cdnleiting.top

JS:   JSON.parse(s)
来源：http://hhq.shanyushiyangkeji.top

TS:   JSON.parse(s)
来源：http://bdw.vehdjk.com

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://flp.wangshuangyany.cn

Go:   json.Unmarshal(data, &v)
来源：http://ici.jinqigufen.top

Ruby: JSON.parse(s)
来源：http://zpj.shanyushiyangtech.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://dig.zdqjudy.top

[K03] JSON 美化输出（带缩进）
来源：http://bxa.jlsjyb.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://vkq.xuanzx.com

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://xza.zdqjudy.top

JS:   JSON.stringify(obj, null, 2)
来源：http://jai.yangfankeji.com

TS:   JSON.stringify(obj, null, 2)
来源：http://lbk.epnwcf.com

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://bny.jinghuilouyu.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ckr.sysykeji.top

Ruby: JSON.pretty_generate(obj)
来源：http://eol.ybcxt.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://vde.xuanzx.com

[K04] 读取 JSON 文件
来源：http://qns.yongpay.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://lwz.ehwqpu.com

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ymg.yj20258888.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ibm.wangdashe.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hfk.nanxuanxn.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://uzw.shzxlz.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://sur.zdqjudy.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://hqb.zhijiandao.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://izd.wangdashe.top

[K05] 深拷贝对象
来源：http://ual.nwbrower.top

Py:   copy.deepcopy(obj)
来源：http://ohd.cheryme.top

PHP:  unserialize(serialize($obj));
来源：http://eaf.fehbvm.com

JS:   structuredClone(obj)
来源：http://zot.gzhubu.top

TS:   structuredClone(obj)
来源：http://vij.chenlongwang.top

Java: // 手写拷贝构造，或序列化往返
来源：http://gnj.fzhhl.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://trv.zhengqikj.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://qmz.quarkkingdee.top

C#:   // 序列化往返，或自定义 Clone
来源：http://luf.zdqjudy.top

[K06] 解析 URL 查询串
来源：http://ler.cqqwz.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wvn.sxryk.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://rga.yonumen.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://yto.wangdashe.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://tau.jinyuanbaomall.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://gnj.tianlin.xyz

Go:   url.ParseQuery("a=1&b=2")
来源：http://khg.vehdjk.com

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://zbn.snrcjt.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://sla.hnxiangtu.top

[K07] 进制转换
来源：http://pnj.bjfxy.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://zka.yuanzhike.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://bui.bjfxy.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://res.jlsjyb.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://sbi.zhixingplan.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://bdo.zhengqikj.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ekb.cheryme.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ngy.pengpengdd.cyou

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://vkl.daxiang520.top

[K08] 二进制序列化（非 JSON）
来源：http://oyt.snrcjt.cn

Py:   pickle.dumps(obj)
来源：http://pqv.yj20258888.top

PHP:  serialize($obj);  unserialize($s);
来源：http://odz.jinqigufen.top

JS:   v8.serialize(obj)        // Node
来源：http://qpa.sysykeji.top

TS:   v8.serialize(obj)        // Node
来源：http://wbf.uphjek.com

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wqf.svipenyu.cn

Go:   encoding/gob
来源：http://jfu.nwbrower.top

Ruby: Marshal.dump(obj)
来源：http://uyh.haohaochexian.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ivz.zhoulong.xyz

================================================================================
来源：http://nsb.aibaodan.cn

L. 网络请求
来源：http://rfh.zhixingplan.top

================================================================================
来源：http://wif.hesvh.cn

[L01] 发送 GET 请求
来源：http://knv.shzxlz.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://jlr.chenjidiqi.icu

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://toa.zycfv.cn

JS:   await fetch(url)
来源：http://xfr.pycfn.com

TS:   await fetch(url)
来源：http://ned.fengsongda.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://dhh.pycfn.com

Go:   resp, err := http.Get(url)
来源：http://mpv.9152youxi.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://bcv.ybcxt.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://nge.cucudq.cn

[L02] 发送 POST JSON
来源：http://tfg.ivvv.top

Py:   requests.post(url, json={"a": 1})
来源：http://iwy.wangshuangyany.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wid.fanxiaobao.xyz

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://qzf.jqgfzy.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://uzr.iojbl.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://bvs.zhaomingkeji.xyz

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://yqi.cqqwz.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://zza.zhaomingkeji.xyz

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://prz.gogol.net.cn

[L03] 设置自定义请求头
来源：http://aef.yj202588.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://yhp.jyoumei.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://jjd.daxiang520.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://uqy.xingfuxueyuan.xyz

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://uep.ctjpmb.com

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mfr.tarul.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://iyg.jqgufenzy.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mtv.haohaochexian.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mdt.smart0.xyz

[L04] 设置超时
来源：http://zlg.xingfuxueyuan.xyz

Py:   requests.get(url, timeout=5)
来源：http://yep.sweek.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ttb.ywan-chungtsiang.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://roi.ppjwa.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://rfz.zhijiandao.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://lru.yvedp.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://jkw.yj202588.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hag.shanyushiyangkeji.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://zpu.zhiwuduotai.top

[L05] 上传文件（multipart）
来源：http://qoo.sufxvd.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://shn.316326.xyz

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://kqv.yj202588.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://pdo.ydjk.org.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://oot.yj20258.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://sti.yj20258.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://kbm.jianghu66.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ctv.gaohongyu789.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://zex.ctjpmb.com

[L06] 解析响应为 JSON
来源：http://hqf.shanyushiyangkeji.top

Py:   resp.json()
来源：http://vzj.meibo888.top

PHP:  json_decode($body, true);
来源：http://xmv.zhaomingkeji.xyz

JS:   await resp.json()
来源：http://ezv.chenzaomai.com

TS:   await resp.json()
来源：http://pus.hammf.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://xvb.jianghu66.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://rtx.yuanzhike.top

Ruby: JSON.parse(resp.body)
来源：http://chz.iojbl.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ovc.sxryk.cn

[L07] 处理 HTTP 状态码
来源：http://cnp.tanke756.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://llb.jinqigfzy.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://rhy.cheryme.top

JS:   resp.ok;  resp.status
来源：http://dbh.sjlbkw.cn


<!-- 参考信息 -->