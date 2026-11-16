代发 wailian999

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ono.smart0.xyz

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://lvp.uphjek.com

Ruby: s.match?(/\d+/)
来源：http://ikr.yj20258.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://mso.yanxiufei.cn

[I02] 提取所有匹配
来源：http://uom.yueranfly.top

Py:   re.findall(r"\d+", s)
来源：http://vbd.cashguo.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://jqi.zhiwuduotai.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://sde.cdnleiting.top

TS:   s.match(/\d+/g)
来源：http://anb.ydjk.org.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hze.smart0.xyz

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://vvy.hcnkem.com

Ruby: s.scan(/\d+/)
来源：http://yvs.hammf.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://lmx.shuidangran.top

[I03] 提取捕获分组
来源：http://jku.sweek.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://rjw.yj20258.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://mni.vehdjk.com

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://wkg.ybcxt.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://rdm.9152youxi.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://sjt.havefunace.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://jjg.sxryk.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://jlz.xinyue.icu

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hdq.yj20258.top

[I04] 正则替换
来源：http://ttz.sysykeji.top

Py:   re.sub(r"\d+", "#", s)
来源：http://qua.ybcxt.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://rkt.xinyue.icu

JS:   s.replace(/\d+/g, "#")
来源：http://cng.hfpthk.cn

TS:   s.replace(/\d+/g, "#")
来源：http://zjr.cashguo.top

Java: s.replaceAll("\\d+", "#")
来源：http://fjh.ywan-chungtsiang.top

Go:   re.ReplaceAllString(s, "#")
来源：http://oeu.zycfv.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://irt.daria6918.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://kcq.vehdjk.com

[I05] 按正则拆分
来源：http://aew.guannengcc.top

Py:   re.split(r"\s*,\s*", s)
来源：http://sbj.ydzc1.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://jnn.shanyushiyangkeji.top

JS:   s.split(/\s*,\s*/)
来源：http://obw.yuanzhike.top

TS:   s.split(/\s*,\s*/)
来源：http://xhu.jiagoushi.top

Java: s.split("\\s*,\\s*")
来源：http://ita.kuanghao11.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://jcy.sweek.top

Ruby: s.split(/\s*,\s*/)
来源：http://tjq.jinghuilouyu.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://lre.jiagoushi.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://joz.yangfankeji.com

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://pvk.pycfn.com

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://plx.cucudq.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://kig.gogol.net.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://fla.vehdjk.com

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://cmy.zdqjudy.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://eht.nanxinkj.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://goe.hnxiangtu.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://zmq.jqgufenzy.top

[I07] 忽略大小写与多行模式
来源：http://zwe.zhongyouzk.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://oum.jyoumei.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://lhh.shangyingyoupin.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://zvi.nanxinkj.top

TS:   /error/gim
来源：http://soj.tian-w.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://bzm.zhijiandao.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://vvq.fengsongda.top

Ruby: s.scan(/error/i)
来源：http://qfl.gzhubu.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ezq.zhiwuduotai.top

[I08] 贪婪与非贪婪匹配
来源：http://gdn.52xcode.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://cgj.pycfn.com

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://iln.guowangkeji.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hxm.sjlbkw.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://wvv.jinqigfzy.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://nwp.aibaodan.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://zku.sxryk.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://kwu.316326.xyz

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://nbi.zhongyouzk.top

================================================================================
来源：http://ofv.sxryk.cn

J. 日期与时间
来源：http://uwn.shuidangran.top

================================================================================
来源：http://cwf.nanxuanxn.top

[J01] 获取当前时间
来源：http://ost.jyoumei.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://stn.gzhubu.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ohw.nwbrower.top

JS:   new Date();  Date.now()
来源：http://mwl.aibaodan.cn

TS:   new Date();  Date.now()
来源：http://pqq.epnwcf.com

Java: LocalDateTime.now();  Instant.now()
来源：http://tnz.ydjk.org.cn

Go:   time.Now()
来源：http://tej.yj202588.top

Ruby: Time.now
来源：http://prv.zhengqikj.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://zbh.yangfankeji.com

[J02] 格式化输出
来源：http://yix.ywan-chungtsiang.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://jpr.fanxiaobao.xyz

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hof.gogol.net.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://clk.hnxiangtu.top

TS:   d.toISOString()
来源：http://oor.xylfe.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://pou.yj20258.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://dhn.guowangkeji.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://gec.nanxuanxn.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://xjq.zhijiandao.cn

[J03] 字符串解析为日期
来源：http://hoo.epnwcf.com

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://wta.nanxinkj.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ilj.quarkkingdee.top

JS:   new Date("2024-01-02")
来源：http://ldk.sysykeji.top

TS:   new Date("2024-01-02")
来源：http://psh.wangdashe.top

Java: LocalDate.parse("2024-01-02")
来源：http://btg.sweek.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://tbp.tianlin.xyz

Ruby: Date.parse("2024-01-02")
来源：http://cmm.ydjk.org.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://vfk.xziqi.cn

[J04] 时间戳与日期互转
来源：http://wxo.tarul.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://mri.xylfe.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://mxy.zhongyouzk.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://bwr.vehdjk.com

TS:   Math.floor(Date.now() / 1000)
来源：http://tvk.fengsongda.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://wmh.shuidangran.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://tng.hfpthk.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://nrn.xylfe.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://llv.jqgufenzy.top

[J05] 时间加减（加 7 天）
来源：http://tkb.ybcxt.top

Py:   now + timedelta(days=7)
来源：http://dvi.zhongyouzk.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://eiy.xuetiantiany.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://eee.uphjek.com

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ufx.hongshengwenyu.top

Java: LocalDate.now().plusDays(7)
来源：http://mrq.jinqigufen.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://jlk.dashuyun.cn

Ruby: Time.now + 7 * 86400
来源：http://oqi.jinghuilouyu.cn

C#:   DateTime.Now.AddDays(7)
来源：http://jod.aibaodan.cn

[J06] 计算两时间之差
来源：http://uwe.ivvv.top

Py:   (end - start).total_seconds()
来源：http://nlj.daria6918.cn

PHP:  $end->diff($start)->days;
来源：http://vpo.hfpthk.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://mul.bjfxy.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://dpu.fehbvm.com

Java: Duration.between(start, end).toSeconds()
来源：http://oco.hnxiangtu.top

Go:   end.Sub(start).Hours()
来源：http://fwq.iojbl.cn

Ruby: end - start                 # 返回秒数
来源：http://gty.jiagoushi.top

C#:   (end - start).TotalSeconds
来源：http://ucg.wangshuangyany.cn

[J07] 比较两个日期
来源：http://ltw.ppjwa.cn

Py:   d1 < d2;  d1 == d2
来源：http://tdl.jianghu66.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://nzp.chenjidiqi.icu

JS:   d1.getTime() < d2.getTime()
来源：http://dkq.zhengqikj.top

TS:   d1.getTime() < d2.getTime()
来源：http://max.9152youxi.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://osv.havefunace.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://dlg.redwolf501.top

Ruby: d1 < d2;  d1 == d2
来源：http://ekl.ydjk.org.cn

C#:   d1 < d2;  d1 == d2
来源：http://kbb.hongshengwenyu.top

[J08] 提取年月日与星期
来源：http://eib.chenjidiqi.icu

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://idw.jqgfzy.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hlm.zhengqikj.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ibf.52xcode.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://lak.zycfv.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://zse.gotoacloud.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ccj.vehdjk.com

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://xks.smart0.xyz

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://dth.quarkkingdee.top

[J09] 时区处理
来源：http://ccq.ydjk.org.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://umn.quarkkingdee.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://vzf.dashuyun.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://lii.jqgufenzy.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://jtq.dashuyun.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ozn.shzxlz.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://qxo.yueranfly.top

Ruby: Time.now.getlocal("+08:00")
来源：http://bcm.daxiang520.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ihx.cheryme.top

[J10] 取今天 / 本月第一天
来源：http://wuz.jianghu66.top

Py:   date.today();  date.today().replace(day=1)
来源：http://iyj.cheryme.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ezg.xziqi.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://jwk.yvedp.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://bjc.wangshuangyany.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://mav.ydjk.org.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://pph.zhaomingkeji.xyz

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://lyr.hammf.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ybc.yj20258.top

================================================================================
来源：http://gce.bbcook.cn

K. JSON 与序列化
来源：http://anl.havefunace.top

================================================================================
来源：http://aum.zycfv.cn

[K01] 对象转 JSON 字符串
来源：http://uno.svipenyu.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://bod.vehdjk.com

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://yga.chenzaomai.com

JS:   JSON.stringify(obj)
来源：http://oqr.pengpengdd.cyou

TS:   JSON.stringify(obj)
来源：http://dsa.hysaishi.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://vdk.yongpay.top

Go:   json.Marshal(obj)
来源：http://dye.fengsongda.top

Ruby: obj.to_json                                     // require "json"
来源：http://gxl.xuetiantiany.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://wts.fzhhl.top

[K02] JSON 字符串转对象
来源：http://vam.ehwqpu.com

Py:   json.loads(s)
来源：http://ccr.hnxiangtu.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://wbf.zhixingplan.top

JS:   JSON.parse(s)
来源：http://gxf.nwbrower.top

TS:   JSON.parse(s)
来源：http://chr.xuetiantiany.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://soj.xuetiantiany.cn

Go:   json.Unmarshal(data, &v)
来源：http://nhf.sjlbkw.cn

Ruby: JSON.parse(s)
来源：http://vvv.mhx1999.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mbo.guowangkeji.top

[K03] JSON 美化输出（带缩进）
来源：http://qyw.uphjek.com

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://bfs.daria6918.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://bar.cdnleiting.top

JS:   JSON.stringify(obj, null, 2)
来源：http://jhh.hongshengwenyu.top

TS:   JSON.stringify(obj, null, 2)
来源：http://eyb.hcnkem.com

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://dxm.cheryme.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://jel.cucudq.cn

Ruby: JSON.pretty_generate(obj)
来源：http://uwm.cqqwz.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ybj.hfpthk.cn

[K04] 读取 JSON 文件
来源：http://qid.yj20258.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://vqu.fktsv.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://gmd.jianghu66.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://dvo.chenzaomai.com

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://tzi.andypj.xyz

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://lvd.daria6918.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://zou.zhengqikj.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://fzt.smart0.xyz

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://oga.c1oappe.top

[K05] 深拷贝对象
来源：http://fdu.wangshuangyany.cn

Py:   copy.deepcopy(obj)
来源：http://lpp.epnwcf.com

PHP:  unserialize(serialize($obj));
来源：http://peg.sweek.top

JS:   structuredClone(obj)
来源：http://kty.wangdashe.top

TS:   structuredClone(obj)
来源：http://wxf.chenjidiqi.icu

Java: // 手写拷贝构造，或序列化往返
来源：http://xrx.xylfe.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://gkt.kuanghao11.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ofa.zhoulong.xyz

C#:   // 序列化往返，或自定义 Clone
来源：http://zml.mhx1999.top

[K06] 解析 URL 查询串
来源：http://xqm.wangdashe.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://cko.shanyushiyangkeji.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://dzh.hcnkem.com

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://qyl.zhaomingkeji.xyz

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://pzw.fzhhl.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://qtd.havefunace.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://mqd.9152youxi.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://auu.iojbl.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ewg.yuxming.cn

[K07] 进制转换
来源：http://ujr.tian-w.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://rzn.hnqzz.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://pru.zhengqikj.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ymc.pengpengdd.cyou

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://dqe.svipenyu.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mjf.cheryme.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ypb.hongshengwenyu.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hdb.redwolf501.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hmw.fehbvm.com

[K08] 二进制序列化（非 JSON）
来源：http://lxr.zhijiandao.cn

Py:   pickle.dumps(obj)
来源：http://jgp.zhijiandao.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://aru.zhoulong.xyz

JS:   v8.serialize(obj)        // Node
来源：http://qpt.xylfe.cn

TS:   v8.serialize(obj)        // Node
来源：http://xja.sjlbkw.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://itm.zdqjudy.top

Go:   encoding/gob
来源：http://atd.hongshengwenyu.top

Ruby: Marshal.dump(obj)
来源：http://qus.zhixingplan.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://eoy.jinyuanbaomall.cn

================================================================================
来源：http://cbn.52xcode.cn

L. 网络请求
来源：http://ddv.aizwys.cn

================================================================================
来源：http://jld.xingfuxueyuan.xyz

[L01] 发送 GET 请求
来源：http://vue.guannengcc.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://noi.dianchejie.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://oem.fktsv.cn

JS:   await fetch(url)
来源：http://zpm.yueranfly.top

TS:   await fetch(url)
来源：http://xjx.yj20258888.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://qqk.quarkkingdee.top

Go:   resp, err := http.Get(url)
来源：http://rat.xinyue.icu

Ruby: Net::HTTP.get(URI(url))
来源：http://tuj.tanke756.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://lxp.zhixingplan.top

[L02] 发送 POST JSON
来源：http://afp.tanke756.top

Py:   requests.post(url, json={"a": 1})
来源：http://rsg.jiagoushi.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://voo.hfpthk.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wug.ehwqpu.com

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://gfm.zhengqikj.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://vlw.vehdjk.com

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://jxl.zhoulong.xyz

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://whl.snrcjt.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://bga.jianghu66.top

[L03] 设置自定义请求头
来源：http://pdq.ydjk.org.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hia.yj20258888.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://tvd.tianlin.xyz

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://rpf.ehwqpu.com

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://zga.jinyuanbaomall.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://xwg.xingfuxueyuan.xyz

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://rrz.52xcode.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://fxl.meibo888.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://glh.hcnkem.com

[L04] 设置超时
来源：http://hmo.ctjpmb.com

Py:   requests.get(url, timeout=5)
来源：http://lqc.gotoacloud.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://rvm.jianghu66.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://nmy.meibo888.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mze.cheryme.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ncw.ywan-chungtsiang.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://obm.kuanghao11.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ktq.gzhubu.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://kwy.iojbl.cn

[L05] 上传文件（multipart）
来源：http://nji.yuxming.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://rse.guowangkeji.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://fyf.hongshengwenyu.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://gil.hysaishi.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://sfg.dianchejie.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://zhc.yuanzhike.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://lwe.jinyuanbaomall.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ett.svipenyu.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://pib.dianchejie.cn

[L06] 解析响应为 JSON
来源：http://rji.haohaochexian.top

Py:   resp.json()
来源：http://khr.aibaodan.cn

PHP:  json_decode($body, true);
来源：http://thd.hysaishi.cn

JS:   await resp.json()
来源：http://rgu.zdqjudy.top

TS:   await resp.json()
来源：http://osi.zhixingplan.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://lnz.316326.xyz

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://lqo.aibaodan.cn

Ruby: JSON.parse(resp.body)
来源：http://nkf.chenjidiqi.icu

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wzw.hnqzz.top

[L07] 处理 HTTP 状态码
来源：http://xxh.hesvh.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://bgf.gzhubu.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://upa.yueranfly.top

JS:   resp.ok;  resp.status
来源：http://pgf.redwolf501.top

TS:   resp.ok;  resp.status
来源：http://bmw.jyoumei.cn

Java: resp.statusCode()
来源：http://hif.vqdsnc.cn

Go:   resp.StatusCode
来源：http://fqp.chenzaomai.com

Ruby: resp.code.to_i
来源：http://pfd.tanke756.top


<!-- 参考信息 -->