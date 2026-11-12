代发 wailian999

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://iha.hywenlv.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://gqt.zhaomingkeji.xyz

Ruby: s.match?(/\d+/)
来源：http://mqy.jqgufenzy.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://axp.gzhubu.top

[I02] 提取所有匹配
来源：http://bab.feifeiyinyue.top

Py:   re.findall(r"\d+", s)
来源：http://dyt.yuanzhike.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://tdn.xinyue.icu

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://evv.tianlin.xyz

TS:   s.match(/\d+/g)
来源：http://xau.shanyushiyangkeji.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://mmn.shanyushiyangkeji.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ewb.nanxinkj.top

Ruby: s.scan(/\d+/)
来源：http://gto.yuxming.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ibl.daxiang520.top

[I03] 提取捕获分组
来源：http://jfa.hfpthk.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://xiz.ctjpmb.com

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://nfa.zhijiandao.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://yaj.guannengcc.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://pay.yanxiufei.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://vjy.yvedp.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ndc.jianghu66.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://lna.hfpthk.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ozd.chenzaomai.com

[I04] 正则替换
来源：http://wgy.svipenyu.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://zjq.guowangkeji.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://gym.sxryk.cn

JS:   s.replace(/\d+/g, "#")
来源：http://bdd.ywan-chungtsiang.top

TS:   s.replace(/\d+/g, "#")
来源：http://dnm.zdbjq.cn

Java: s.replaceAll("\\d+", "#")
来源：http://tfr.xziqi.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://hrp.chenlongwang.top

Ruby: s.gsub(/\d+/, "#")
来源：http://hyw.gaohongyu789.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://lab.haohaochexian.top

[I05] 按正则拆分
来源：http://kwh.sweek.top

Py:   re.split(r"\s*,\s*", s)
来源：http://wjc.ppjwa.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://qqn.hongshengwenyu.top

JS:   s.split(/\s*,\s*/)
来源：http://dsb.gaohongyu789.top

TS:   s.split(/\s*,\s*/)
来源：http://dfd.vehdjk.com

Java: s.split("\\s*,\\s*")
来源：http://gdm.hongshengwenyu.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://zwj.vehdjk.com

Ruby: s.split(/\s*,\s*/)
来源：http://aml.yuanzhike.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hrr.zycfv.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://tyf.dashuyun.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://eim.yfazqb.com

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://jgj.fktsv.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://var.316326.xyz

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://oth.sufxvd.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://sin.fanxiaobao.xyz

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hyg.hongshengwenyu.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://xkc.ehwqpu.com

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ljb.kuanghao11.cn

[I07] 忽略大小写与多行模式
来源：http://taz.sweek.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://yze.hongshengwenyu.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://zqw.daxiang520.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://wyn.cheryme.top

TS:   /error/gim
来源：http://bah.yueranfly.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://yrf.yonumen.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://xxg.hywenlv.cn

Ruby: s.scan(/error/i)
来源：http://ttk.gogol.net.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://muo.jianghu66.top

[I08] 贪婪与非贪婪匹配
来源：http://eng.iojbl.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://byv.zhaomingkeji.xyz

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://pgc.hnqzz.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://rcy.epnwcf.com

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ovq.kuanghao11.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://ysz.bjfxy.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://eep.chenjidiqi.icu

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://psj.fehbvm.com

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ows.52xcode.cn

================================================================================
来源：http://gca.chenjidiqi.icu

J. 日期与时间
来源：http://iys.hongshengwenyu.top

================================================================================
来源：http://jwt.hcnkem.com

[J01] 获取当前时间
来源：http://tjo.ehwqpu.com

Py:   datetime.now();  datetime.now(UTC)
来源：http://kdo.gotoacloud.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://rba.jinyuanbaomall.cn

JS:   new Date();  Date.now()
来源：http://tue.snrcjt.cn

TS:   new Date();  Date.now()
来源：http://ius.316326.xyz

Java: LocalDateTime.now();  Instant.now()
来源：http://ljo.zhaomingkeji.xyz

Go:   time.Now()
来源：http://sia.tianlin.xyz

Ruby: Time.now
来源：http://gdr.bjfxy.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://irs.snrcjt.cn

[J02] 格式化输出
来源：http://qyw.haohaochexian.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://qla.yongpay.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://sic.guannengcc.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ibg.gzhubu.top

TS:   d.toISOString()
来源：http://gut.meibo888.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://yse.cheryme.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://zyu.fanxiaobao.xyz

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://gnc.gogol.net.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://zzr.nwbrower.top

[J03] 字符串解析为日期
来源：http://szu.yuanzhike.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://qjt.nanxuanxn.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ans.hesvh.cn

JS:   new Date("2024-01-02")
来源：http://upp.hfpthk.cn

TS:   new Date("2024-01-02")
来源：http://pgl.haohaochexian.top

Java: LocalDate.parse("2024-01-02")
来源：http://ked.jinqigfzy.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://pav.ctjpmb.com

Ruby: Date.parse("2024-01-02")
来源：http://bqs.shzxlz.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://wqe.zhixingplan.top

[J04] 时间戳与日期互转
来源：http://ibk.cheryme.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://aev.pengpengdd.cyou

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://yqc.ppjwa.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://xdt.fehbvm.com

TS:   Math.floor(Date.now() / 1000)
来源：http://mnl.9152youxi.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://qtq.shangyingyoupin.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://lrg.ctjpmb.com

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://try.shangyingyoupin.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://chd.sjlbkw.cn

[J05] 时间加减（加 7 天）
来源：http://gzm.shzxlz.cn

Py:   now + timedelta(days=7)
来源：http://cgu.yuanzhike.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://dqx.shanyushiyangtech.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ypg.nanxinkj.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ikn.birdmap.top

Java: LocalDate.now().plusDays(7)
来源：http://fql.xuetiantiany.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://nls.svipenyu.cn

Ruby: Time.now + 7 * 86400
来源：http://dxk.yj20258888.top

C#:   DateTime.Now.AddDays(7)
来源：http://dnq.vehdjk.com

[J06] 计算两时间之差
来源：http://zle.sufxvd.cn

Py:   (end - start).total_seconds()
来源：http://uei.sxryk.cn

PHP:  $end->diff($start)->days;
来源：http://ugb.dashuyun.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://iio.tanke756.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://khi.haohaochexian.top

Java: Duration.between(start, end).toSeconds()
来源：http://hrd.yj20258888.top

Go:   end.Sub(start).Hours()
来源：http://ujx.bjfxy.top

Ruby: end - start                 # 返回秒数
来源：http://kii.yfazqb.com

C#:   (end - start).TotalSeconds
来源：http://fsz.cheryme.top

[J07] 比较两个日期
来源：http://kii.haohaochexian.top

Py:   d1 < d2;  d1 == d2
来源：http://hax.fengsongda.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://jrq.xylfe.cn

JS:   d1.getTime() < d2.getTime()
来源：http://lur.shuidangran.top

TS:   d1.getTime() < d2.getTime()
来源：http://kzs.smart0.xyz

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://kbl.yj20258888.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://kxc.zdqjudy.top

Ruby: d1 < d2;  d1 == d2
来源：http://xzt.haohaochexian.top

C#:   d1 < d2;  d1 == d2
来源：http://lqn.c1oappe.top

[J08] 提取年月日与星期
来源：http://low.yanxiufei.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://lov.uphjek.com

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://akv.aizwys.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://fmz.ybcxt.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://tvx.jlsjyb.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://pjr.zhaomingkeji.xyz

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://sgp.hesvh.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://dxz.daxiang520.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://aax.nanxuanxn.top

[J09] 时区处理
来源：http://mun.tianlin.xyz

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://eaf.fzhhl.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://pzl.zhengqikj.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://bmv.daxiang520.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ztb.tanke756.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://czj.cdnleiting.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://obd.zycfv.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://fig.cucudq.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://qtn.hysaishi.cn

[J10] 取今天 / 本月第一天
来源：http://fjb.snrcjt.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://fed.yj20258888.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://tna.hysaishi.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://zef.hysaishi.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://gtk.jqgfzy.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://zql.dashuyun.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://gfs.fengsongda.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://zba.hongshengwenyu.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://qvn.ctjpmb.com

================================================================================
来源：http://llm.gotoacloud.top

K. JSON 与序列化
来源：http://yuo.hongshengwenyu.top

================================================================================
来源：http://qoj.cdnleiting.top

[K01] 对象转 JSON 字符串
来源：http://hcd.xziqi.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ssr.cqqwz.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://rue.xinyue.icu

JS:   JSON.stringify(obj)
来源：http://onc.redwolf501.top

TS:   JSON.stringify(obj)
来源：http://pyr.sweek.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ldz.xinyue.icu

Go:   json.Marshal(obj)
来源：http://vxg.aibaodan.cn

Ruby: obj.to_json                                     // require "json"
来源：http://gsh.quarkkingdee.top

C#:   JsonSerializer.Serialize(obj)
来源：http://zej.9152youxi.cn

[K02] JSON 字符串转对象
来源：http://dpf.hywenlv.cn

Py:   json.loads(s)
来源：http://rpb.yvedp.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://bqr.hfpthk.cn

JS:   JSON.parse(s)
来源：http://zvl.fehbvm.com

TS:   JSON.parse(s)
来源：http://jfr.chenjidiqi.icu

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://sui.wangdashe.top

Go:   json.Unmarshal(data, &v)
来源：http://sva.yj202588.top

Ruby: JSON.parse(s)
来源：http://qmh.zdqjudy.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://rvc.yj202588.top

[K03] JSON 美化输出（带缩进）
来源：http://tre.dashuyun.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://dbg.sweek.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://dda.ydzc1.top

JS:   JSON.stringify(obj, null, 2)
来源：http://ktl.vqdsnc.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://ubi.yongpay.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://not.jinqigufen.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://enf.hcnkem.com

Ruby: JSON.pretty_generate(obj)
来源：http://auy.aibaodan.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://yzb.snrcjt.cn

[K04] 读取 JSON 文件
来源：http://ieq.jiagoushi.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://cni.shangyingyoupin.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://teq.yanxiufei.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://bty.jiagoushi.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://xtf.nanxuanxn.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://zrm.fanxiaobao.xyz

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://yoc.fanxiaobao.xyz

Ruby: JSON.parse(File.read("a.json"))
来源：http://aql.cdnleiting.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://kun.jinqigufen.top

[K05] 深拷贝对象
来源：http://fuy.aibaodan.cn

Py:   copy.deepcopy(obj)
来源：http://ipx.tianlin.xyz

PHP:  unserialize(serialize($obj));
来源：http://ioy.chenzaomai.com

JS:   structuredClone(obj)
来源：http://hdc.chenjidiqi.icu

TS:   structuredClone(obj)
来源：http://gwi.guowangkeji.top

Java: // 手写拷贝构造，或序列化往返
来源：http://gry.jyoumei.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://unc.jyoumei.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hvp.zhixingplan.top

C#:   // 序列化往返，或自定义 Clone
来源：http://xlc.hnqzz.top

[K06] 解析 URL 查询串
来源：http://bdx.c1oappe.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://cgu.ydzc1.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://avl.gzhubu.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://amr.fzhhl.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://qkt.smart0.xyz

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ugk.cdnleiting.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://yfl.hcnkem.com

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://gjh.chenlongwang.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://zcz.shanyushiyangkeji.top

[K07] 进制转换
来源：http://tcb.yuanzhike.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ons.hnqzz.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://pbu.yuanzhike.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://svi.ctjpmb.com

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://jqa.zdbjq.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ocr.uphjek.com

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://jqh.zdqjudy.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://gmx.tianlin.xyz

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://cvp.kuanghao11.cn

[K08] 二进制序列化（非 JSON）
来源：http://ibv.cheryme.top

Py:   pickle.dumps(obj)
来源：http://onx.jinqigfzy.top

PHP:  serialize($obj);  unserialize($s);
来源：http://nkh.tianlin.xyz

JS:   v8.serialize(obj)        // Node
来源：http://gpt.sxryk.cn

TS:   v8.serialize(obj)        // Node
来源：http://udg.c1oappe.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ecl.gzhubu.top

Go:   encoding/gob
来源：http://fua.sxryk.cn

Ruby: Marshal.dump(obj)
来源：http://tkm.aizwys.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://jym.jianghu66.top

================================================================================
来源：http://fdm.ydjk.org.cn

L. 网络请求
来源：http://stb.feifeiyinyue.top

================================================================================
来源：http://eim.yanxiufei.cn

[L01] 发送 GET 请求
来源：http://vju.uphjek.com

Py:   requests.get(url)                        # 第三方库 requests
来源：http://icn.svipenyu.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://tmr.daria6918.cn

JS:   await fetch(url)
来源：http://gbm.snrcjt.cn

TS:   await fetch(url)
来源：http://eiq.iojbl.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ejq.iojbl.cn

Go:   resp, err := http.Get(url)
来源：http://stx.daxiang520.top

Ruby: Net::HTTP.get(URI(url))
来源：http://jip.iojbl.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hlg.ivvv.top

[L02] 发送 POST JSON
来源：http://frc.zhiwuduotai.top

Py:   requests.post(url, json={"a": 1})
来源：http://zmx.quarkkingdee.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ieq.yongpay.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://vre.shzxlz.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://exn.yuanzhike.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://owj.zhiwuduotai.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://pju.zhongyouzk.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://fhf.fzhhl.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://dgg.chenjidiqi.icu

[L03] 设置自定义请求头
来源：http://yuz.aizwys.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://lew.wangdashe.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://dgz.cdnleiting.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://jdq.nanxuanxn.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://fzd.hammf.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ift.cdnleiting.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://odh.feifeiyinyue.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://bek.aibaodan.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://jdh.gzhubu.top

[L04] 设置超时
来源：http://syj.jinqigufen.top

Py:   requests.get(url, timeout=5)
来源：http://czj.wangshuangyany.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://eqa.feifeiyinyue.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://owx.cheryme.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://bpy.gaohongyu789.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://kar.hnxiangtu.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://tnc.ehwqpu.com

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://njr.snrcjt.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://eef.cashguo.top

[L05] 上传文件（multipart）
来源：http://qvk.316326.xyz

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://osf.gaohongyu789.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hbd.hongshengwenyu.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://bty.guannengcc.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://pqr.feifeiyinyue.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://vrs.hammf.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wou.zhijiandao.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://jix.jqgfzy.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://dcd.tianlin.xyz

[L06] 解析响应为 JSON
来源：http://prt.yuxming.cn

Py:   resp.json()
来源：http://ion.hywenlv.cn

PHP:  json_decode($body, true);
来源：http://mlx.yj202588.top

JS:   await resp.json()
来源：http://zwm.cqqwz.cn

TS:   await resp.json()
来源：http://gqv.hfpthk.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hav.yj202588.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://kes.xziqi.cn

Ruby: JSON.parse(resp.body)
来源：http://jus.feifeiyinyue.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ycn.gaohongyu789.top

[L07] 处理 HTTP 状态码
来源：http://uas.zycfv.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://jxh.meibo888.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wmn.jianghu66.top

JS:   resp.ok;  resp.status
来源：http://cce.hnxiangtu.top

TS:   resp.ok;  resp.status
来源：http://bai.ydzc1.top

Java: resp.statusCode()
来源：http://uxu.ydjk.org.cn

Go:   resp.StatusCode
来源：http://swz.shangyingyoupin.top

Ruby: resp.code.to_i
来源：http://psa.zhoulong.xyz


<!-- 参考信息 -->