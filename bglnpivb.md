代发 wailian999

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://zcq.jqgufenzy.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://rhl.hesvh.cn

Ruby: s.match?(/\d+/)
来源：http://zim.ppjwa.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://qav.fanxiaobao.xyz

[I02] 提取所有匹配
来源：http://shp.yuxming.cn

Py:   re.findall(r"\d+", s)
来源：http://vxm.aizwys.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://fsw.yj20258.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://yei.epnwcf.com

TS:   s.match(/\d+/g)
来源：http://ctr.xuanzx.com

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://bhs.zhixingplan.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://guc.ydzc1.top

Ruby: s.scan(/\d+/)
来源：http://qcz.aizwys.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://cep.cashguo.top

[I03] 提取捕获分组
来源：http://vrx.yj20258888.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://pbi.meibo888.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://fot.bjfxy.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://njl.316326.xyz

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://iqe.jyoumei.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://vpf.jinqigfzy.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://qoz.xziqi.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://lgf.daxiang520.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://gqf.vehdjk.com

[I04] 正则替换
来源：http://vei.cashguo.top

Py:   re.sub(r"\d+", "#", s)
来源：http://zve.cucudq.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://mzx.gotoacloud.top

JS:   s.replace(/\d+/g, "#")
来源：http://bis.ydjk.org.cn

TS:   s.replace(/\d+/g, "#")
来源：http://ysg.yj202588.top

Java: s.replaceAll("\\d+", "#")
来源：http://bmf.fanxiaobao.xyz

Go:   re.ReplaceAllString(s, "#")
来源：http://pay.gaohongyu789.top

Ruby: s.gsub(/\d+/, "#")
来源：http://ivu.dianchejie.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://xtf.shuidangran.top

[I05] 按正则拆分
来源：http://awt.snrcjt.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://jvh.yj20258.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://jga.jlsjyb.cn

JS:   s.split(/\s*,\s*/)
来源：http://bql.aibaodan.cn

TS:   s.split(/\s*,\s*/)
来源：http://vlu.jinqigufen.top

Java: s.split("\\s*,\\s*")
来源：http://qkn.cdnleiting.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://dfb.chenlongwang.top

Ruby: s.split(/\s*,\s*/)
来源：http://oup.zdbjq.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://fgh.yj20258888.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://bbi.yj20258888.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://gyb.9152youxi.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://sdp.jinqigfzy.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://gbc.yanxiufei.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hst.vqdsnc.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://fbe.jinqigfzy.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://edo.jianghu66.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://knx.uphjek.com

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://mgt.vehdjk.com

[I07] 忽略大小写与多行模式
来源：http://iak.sweek.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://urw.fzhhl.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://qas.fzhhl.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://vhf.sufxvd.cn

TS:   /error/gim
来源：http://dde.yanxiufei.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://uas.yuxming.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://jzc.hnqzz.top

Ruby: s.scan(/error/i)
来源：http://dlh.hfpthk.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ryy.jiagoushi.top

[I08] 贪婪与非贪婪匹配
来源：http://ida.gaohongyu789.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://jcy.ydzc1.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ahg.yj20258.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://lna.hysaishi.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://cgj.aizwys.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://uyh.xziqi.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ksb.yanxiufei.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://coy.tarul.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://fby.aibaodan.cn

================================================================================
来源：http://xme.xuetiantiany.cn

J. 日期与时间
来源：http://xlh.fanxiaobao.xyz

================================================================================
来源：http://emo.tarul.cn

[J01] 获取当前时间
来源：http://xof.ehwqpu.com

Py:   datetime.now();  datetime.now(UTC)
来源：http://wrx.nwbrower.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://rsi.epnwcf.com

JS:   new Date();  Date.now()
来源：http://mrh.jinghuilouyu.cn

TS:   new Date();  Date.now()
来源：http://fmp.iojbl.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://obp.ehwqpu.com

Go:   time.Now()
来源：http://nxq.shanyushiyangkeji.top

Ruby: Time.now
来源：http://hyx.zycfv.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://cqj.zdbjq.cn

[J02] 格式化输出
来源：http://ton.tian-w.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://zao.iojbl.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://fws.zhoulong.xyz

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://jju.jianghu66.top

TS:   d.toISOString()
来源：http://drp.fanxiaobao.xyz

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://keo.jianghu66.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ocp.jlsjyb.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://cnz.havefunace.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://qag.ywan-chungtsiang.top

[J03] 字符串解析为日期
来源：http://vcs.chenjidiqi.icu

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://kbb.ywan-chungtsiang.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://lsb.cheryme.top

JS:   new Date("2024-01-02")
来源：http://ucl.uphjek.com

TS:   new Date("2024-01-02")
来源：http://dnb.quarkkingdee.top

Java: LocalDate.parse("2024-01-02")
来源：http://ceo.jinqigufen.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://xjp.sweek.top

Ruby: Date.parse("2024-01-02")
来源：http://byi.tian-w.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://sgp.snrcjt.cn

[J04] 时间戳与日期互转
来源：http://vjw.hfpthk.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://zsq.jiagoushi.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://voi.bjfxy.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://vpm.snrcjt.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://vnx.chenjidiqi.icu

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://quy.fktsv.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://okl.yuxming.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://pmi.gotoacloud.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://wrl.uphjek.com

[J05] 时间加减（加 7 天）
来源：http://bej.tanke756.top

Py:   now + timedelta(days=7)
来源：http://wkd.cheryme.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://tkz.yanxiufei.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://vcw.gaohongyu789.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://fxe.nwbrower.top

Java: LocalDate.now().plusDays(7)
来源：http://ror.xuetiantiany.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://skh.ehwqpu.com

Ruby: Time.now + 7 * 86400
来源：http://aax.shanyushiyangtech.top

C#:   DateTime.Now.AddDays(7)
来源：http://pzn.gzhubu.top

[J06] 计算两时间之差
来源：http://bre.ydjk.org.cn

Py:   (end - start).total_seconds()
来源：http://sey.hnxiangtu.top

PHP:  $end->diff($start)->days;
来源：http://bbj.xziqi.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://xwj.zhixingplan.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://uzj.vqdsnc.cn

Java: Duration.between(start, end).toSeconds()
来源：http://jvx.kuanghao11.cn

Go:   end.Sub(start).Hours()
来源：http://oxo.c1oappe.top

Ruby: end - start                 # 返回秒数
来源：http://rtb.xingfuxueyuan.xyz

C#:   (end - start).TotalSeconds
来源：http://jmw.feifeiyinyue.top

[J07] 比较两个日期
来源：http://ejf.jianghu66.top

Py:   d1 < d2;  d1 == d2
来源：http://fgz.jinqigfzy.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://poo.bjfxy.top

JS:   d1.getTime() < d2.getTime()
来源：http://rzl.sxryk.cn

TS:   d1.getTime() < d2.getTime()
来源：http://nvc.jiagoushi.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://rcf.hysaishi.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://efj.nanxinkj.top

Ruby: d1 < d2;  d1 == d2
来源：http://lna.tanke756.top

C#:   d1 < d2;  d1 == d2
来源：http://tux.316326.xyz

[J08] 提取年月日与星期
来源：http://fda.yj202588.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://yln.bbcook.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://abm.hesvh.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ijg.yuanzhike.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://pjz.yuanzhike.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://zxu.zhiwuduotai.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hre.gotoacloud.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://mcf.gaohongyu789.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://cpl.meibo888.top

[J09] 时区处理
来源：http://hzq.yj20258888.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ilx.jinghuilouyu.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://bpw.mhx1999.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ild.dianchejie.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://yly.gogol.net.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hab.pengpengdd.cyou

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://zzm.nanxuanxn.top

Ruby: Time.now.getlocal("+08:00")
来源：http://zvc.hfpthk.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://zyd.sjlbkw.cn

[J10] 取今天 / 本月第一天
来源：http://vlv.meibo888.top

Py:   date.today();  date.today().replace(day=1)
来源：http://bjv.jqgufenzy.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://wma.chenlongwang.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ovz.gotoacloud.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://axo.shangyingyoupin.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://czj.zhaomingkeji.xyz

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ixr.wangshuangyany.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://izu.havefunace.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ata.hnxiangtu.top

================================================================================
来源：http://ceo.zdqjudy.top

K. JSON 与序列化
来源：http://imz.jlsjyb.cn

================================================================================
来源：http://vsg.meibo888.top

[K01] 对象转 JSON 字符串
来源：http://ozw.chenlongwang.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ydk.xylfe.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://yfh.ctjpmb.com

JS:   JSON.stringify(obj)
来源：http://tsp.pengpengdd.cyou

TS:   JSON.stringify(obj)
来源：http://uor.9152youxi.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://bsd.snrcjt.cn

Go:   json.Marshal(obj)
来源：http://uep.quarkkingdee.top

Ruby: obj.to_json                                     // require "json"
来源：http://vpz.cheryme.top

C#:   JsonSerializer.Serialize(obj)
来源：http://rvh.birdmap.top

[K02] JSON 字符串转对象
来源：http://jsx.ctjpmb.com

Py:   json.loads(s)
来源：http://gim.nanxinkj.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://orr.hcnkem.com

JS:   JSON.parse(s)
来源：http://hgg.fengsongda.top

TS:   JSON.parse(s)
来源：http://qpk.zdqjudy.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://xyb.havefunace.top

Go:   json.Unmarshal(data, &v)
来源：http://vkz.9152youxi.cn

Ruby: JSON.parse(s)
来源：http://oav.guowangkeji.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://vuc.yonumen.top

[K03] JSON 美化输出（带缩进）
来源：http://wzh.bbcook.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ssn.jinyuanbaomall.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://cmr.ydzc1.top

JS:   JSON.stringify(obj, null, 2)
来源：http://xgl.cashguo.top

TS:   JSON.stringify(obj, null, 2)
来源：http://hlo.yvedp.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://mmt.svipenyu.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://cwh.yfazqb.com

Ruby: JSON.pretty_generate(obj)
来源：http://rlf.aibaodan.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://sii.aizwys.cn

[K04] 读取 JSON 文件
来源：http://oos.yonumen.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://vfv.daria6918.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ipw.chenzaomai.com

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hla.zhixingplan.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://qbg.shzxlz.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://frx.ywan-chungtsiang.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://znk.chenzaomai.com

Ruby: JSON.parse(File.read("a.json"))
来源：http://gsa.cashguo.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ylh.yvedp.cn

[K05] 深拷贝对象
来源：http://dpx.ppjwa.cn

Py:   copy.deepcopy(obj)
来源：http://bln.jinqigufen.top

PHP:  unserialize(serialize($obj));
来源：http://glt.jyoumei.cn

JS:   structuredClone(obj)
来源：http://hxp.mhx1999.top

TS:   structuredClone(obj)
来源：http://req.c1oappe.top

Java: // 手写拷贝构造，或序列化往返
来源：http://ozr.zhiwuduotai.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://yjk.jinqigfzy.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://lbx.snrcjt.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://shz.xingfuxueyuan.xyz

[K06] 解析 URL 查询串
来源：http://bcp.cheryme.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wgz.epnwcf.com

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ppp.yfazqb.com

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ddd.cheryme.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://tvp.havefunace.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wnr.ywan-chungtsiang.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://byc.snrcjt.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://lxz.sysykeji.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://egc.yj202588.top

[K07] 进制转换
来源：http://npr.cashguo.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ohu.jyoumei.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://rzr.hcnkem.com

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://mtf.jinqigufen.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://unk.svipenyu.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://uuu.smart0.xyz

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mhr.ppjwa.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://zfm.shzxlz.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://vld.xuetiantiany.cn

[K08] 二进制序列化（非 JSON）
来源：http://vzh.yuanzhike.top

Py:   pickle.dumps(obj)
来源：http://usm.iojbl.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://poo.xinyue.icu

JS:   v8.serialize(obj)        // Node
来源：http://mvs.jqgfzy.top

TS:   v8.serialize(obj)        // Node
来源：http://tms.yangfankeji.com

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://afe.yuanzhike.top

Go:   encoding/gob
来源：http://juh.jiagoushi.top

Ruby: Marshal.dump(obj)
来源：http://kvf.chenjidiqi.icu

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hva.xuanzx.com

================================================================================
来源：http://smk.bjfxy.top

L. 网络请求
来源：http://ofv.yj202588.top

================================================================================
来源：http://seq.jyoumei.cn

[L01] 发送 GET 请求
来源：http://aum.aizwys.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://akr.hfpthk.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://yhg.wangdashe.top

JS:   await fetch(url)
来源：http://mmv.pengpengdd.cyou

TS:   await fetch(url)
来源：http://qjj.shzxlz.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://iah.c1oappe.top

Go:   resp, err := http.Get(url)
来源：http://jdg.dianchejie.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://kpn.jiagoushi.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://bkg.aibaodan.cn

[L02] 发送 POST JSON
来源：http://nep.yvedp.cn

Py:   requests.post(url, json={"a": 1})
来源：http://mce.ppjwa.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ohl.yj20258.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://glm.aizwys.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://sss.yanxiufei.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://glg.aibaodan.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://meb.cucudq.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://bcn.gzhubu.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://qfe.daria6918.cn

[L03] 设置自定义请求头
来源：http://ovq.zhengqikj.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://syr.haohaochexian.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://szo.hfpthk.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://xya.cheryme.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://cqc.kuanghao11.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://qav.hywenlv.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://qtb.c1oappe.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wne.ydzc1.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ycz.epnwcf.com

[L04] 设置超时
来源：http://omu.cucudq.cn

Py:   requests.get(url, timeout=5)
来源：http://mtn.chenjidiqi.icu

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://vrl.316326.xyz

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://fze.jinghuilouyu.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://swq.dashuyun.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ayf.yuxming.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://vzt.ywan-chungtsiang.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://lez.cashguo.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://uzi.zdqjudy.top

[L05] 上传文件（multipart）
来源：http://fwp.hongshengwenyu.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://bsu.shangyingyoupin.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ngo.hysaishi.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://tld.kuanghao11.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://zdh.zdbjq.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://bdf.xuetiantiany.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mjn.sjlbkw.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mad.bbcook.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://okr.xinyue.icu

[L06] 解析响应为 JSON
来源：http://dac.aibaodan.cn

Py:   resp.json()
来源：http://ykw.shanyushiyangkeji.top

PHP:  json_decode($body, true);
来源：http://ohb.fehbvm.com

JS:   await resp.json()
来源：http://ckv.yuanzhike.top

TS:   await resp.json()
来源：http://qfw.cqqwz.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://vwj.shuidangran.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://luo.mhx1999.top

Ruby: JSON.parse(resp.body)
来源：http://ius.zhongyouzk.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://rrw.ehwqpu.com

[L07] 处理 HTTP 状态码
来源：http://poy.hammf.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://gmg.snrcjt.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hnt.aibaodan.cn

JS:   resp.ok;  resp.status
来源：http://fgf.yj20258.top

TS:   resp.ok;  resp.status
来源：http://rtx.fengsongda.top

Java: resp.statusCode()
来源：http://kno.ywan-chungtsiang.top

Go:   resp.StatusCode
来源：http://zxy.shanyushiyangtech.top

Ruby: resp.code.to_i
来源：http://ytd.xuanzx.com


<!-- 参考信息 -->