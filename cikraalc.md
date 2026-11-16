代发 wailian999

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://zit.52xcode.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wqe.pengpengdd.cyou

Ruby: s.match?(/\d+/)
来源：http://hqf.kuanghao11.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://lqg.xziqi.cn

[I02] 提取所有匹配
来源：http://zyc.sysykeji.top

Py:   re.findall(r"\d+", s)
来源：http://xxe.wangdashe.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://sgn.yj20258888.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://xye.aizwys.cn

TS:   s.match(/\d+/g)
来源：http://kou.tianlin.xyz

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://mkz.9152youxi.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://rzy.ydzc1.top

Ruby: s.scan(/\d+/)
来源：http://vqi.jqgufenzy.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ytt.yangfankeji.com

[I03] 提取捕获分组
来源：http://qzt.yanxiufei.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://wfe.xingfuxueyuan.xyz

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://yka.9152youxi.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://wsy.aizwys.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ytw.sjlbkw.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://pbr.ctjpmb.com

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://dnm.daxiang520.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://fss.vehdjk.com

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://zrk.xinyue.icu

[I04] 正则替换
来源：http://rel.wangdashe.top

Py:   re.sub(r"\d+", "#", s)
来源：http://evq.kuanghao11.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://mum.shzxlz.cn

JS:   s.replace(/\d+/g, "#")
来源：http://eji.gzhubu.top

TS:   s.replace(/\d+/g, "#")
来源：http://sxv.cheryme.top

Java: s.replaceAll("\\d+", "#")
来源：http://frx.xuetiantiany.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://noa.birdmap.top

Ruby: s.gsub(/\d+/, "#")
来源：http://nww.zdbjq.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://klp.gotoacloud.top

[I05] 按正则拆分
来源：http://puy.cheryme.top

Py:   re.split(r"\s*,\s*", s)
来源：http://bsq.daxiang520.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://fqs.zdbjq.cn

JS:   s.split(/\s*,\s*/)
来源：http://yes.jiagoushi.top

TS:   s.split(/\s*,\s*/)
来源：http://giy.daria6918.cn

Java: s.split("\\s*,\\s*")
来源：http://yce.zdqjudy.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://elj.andypj.xyz

Ruby: s.split(/\s*,\s*/)
来源：http://gyk.yuxming.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hlq.xylfe.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://kaj.fzhhl.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://feo.sxryk.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://iwa.zhaomingkeji.xyz

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://efm.tanke756.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mie.andypj.xyz

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://eru.fengsongda.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://yte.hongshengwenyu.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://zvj.zhengqikj.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://veh.yj202588.top

[I07] 忽略大小写与多行模式
来源：http://fkx.gotoacloud.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://lgv.ivvv.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://txk.sysykeji.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://orn.yfazqb.com

TS:   /error/gim
来源：http://kfk.daxiang520.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://vci.hywenlv.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://etb.jqgfzy.top

Ruby: s.scan(/error/i)
来源：http://ioq.fengsongda.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://zun.aibaodan.cn

[I08] 贪婪与非贪婪匹配
来源：http://tif.ctjpmb.com

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://gwc.bbcook.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://bax.cheryme.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://fvv.zhijiandao.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://wij.shuidangran.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://twq.hysaishi.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hhz.yfazqb.com

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://eho.sjlbkw.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://npe.yvedp.cn

================================================================================
来源：http://fch.fzhhl.top

J. 日期与时间
来源：http://vtj.quarkkingdee.top

================================================================================
来源：http://yot.xuanzx.com

[J01] 获取当前时间
来源：http://eat.nwbrower.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://fya.havefunace.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ckz.yj20258.top

JS:   new Date();  Date.now()
来源：http://icy.ivvv.top

TS:   new Date();  Date.now()
来源：http://sjm.gzhubu.top

Java: LocalDateTime.now();  Instant.now()
来源：http://xtn.fzhhl.top

Go:   time.Now()
来源：http://ylt.fehbvm.com

Ruby: Time.now
来源：http://fee.yanxiufei.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://uql.hammf.cn

[J02] 格式化输出
来源：http://fat.meibo888.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mnw.ppjwa.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://eeq.jinghuilouyu.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://vdq.bbcook.cn

TS:   d.toISOString()
来源：http://wzz.wangshuangyany.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://etp.yvedp.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ctk.sjlbkw.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://zsi.cashguo.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://vun.nwbrower.top

[J03] 字符串解析为日期
来源：http://jxe.guannengcc.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://vsv.dianchejie.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://dee.cdnleiting.top

JS:   new Date("2024-01-02")
来源：http://bys.tian-w.cn

TS:   new Date("2024-01-02")
来源：http://dxv.hnxiangtu.top

Java: LocalDate.parse("2024-01-02")
来源：http://gdj.nanxinkj.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://aes.cashguo.top

Ruby: Date.parse("2024-01-02")
来源：http://pfx.sxryk.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://uie.bjfxy.top

[J04] 时间戳与日期互转
来源：http://xjx.fengsongda.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://psn.iojbl.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://voa.xuanzx.com

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://fto.kuanghao11.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://lfk.zhengqikj.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://iew.fanxiaobao.xyz

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://huq.tian-w.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://uyb.havefunace.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://vnu.epnwcf.com

[J05] 时间加减（加 7 天）
来源：http://dai.wangdashe.top

Py:   now + timedelta(days=7)
来源：http://yep.aibaodan.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://euw.ivvv.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://rie.cheryme.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://tpp.sjlbkw.cn

Java: LocalDate.now().plusDays(7)
来源：http://rde.jinyuanbaomall.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://glh.zdqjudy.top

Ruby: Time.now + 7 * 86400
来源：http://yit.guannengcc.top

C#:   DateTime.Now.AddDays(7)
来源：http://grh.dianchejie.cn

[J06] 计算两时间之差
来源：http://nur.tian-w.cn

Py:   (end - start).total_seconds()
来源：http://qoa.cashguo.top

PHP:  $end->diff($start)->days;
来源：http://wnx.shanyushiyangtech.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://fdj.9152youxi.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hch.yanxiufei.cn

Java: Duration.between(start, end).toSeconds()
来源：http://nse.9152youxi.cn

Go:   end.Sub(start).Hours()
来源：http://syp.zhongyouzk.top

Ruby: end - start                 # 返回秒数
来源：http://yqg.jyoumei.cn

C#:   (end - start).TotalSeconds
来源：http://mde.pycfn.com

[J07] 比较两个日期
来源：http://kaq.yj202588.top

Py:   d1 < d2;  d1 == d2
来源：http://bzq.hnqzz.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://xjj.ybcxt.top

JS:   d1.getTime() < d2.getTime()
来源：http://ywz.ywan-chungtsiang.top

TS:   d1.getTime() < d2.getTime()
来源：http://bfq.c1oappe.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://vpo.fehbvm.com

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://blr.gaohongyu789.top

Ruby: d1 < d2;  d1 == d2
来源：http://iit.ctjpmb.com

C#:   d1 < d2;  d1 == d2
来源：http://wjm.dianchejie.cn

[J08] 提取年月日与星期
来源：http://qpg.tian-w.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://pry.ctjpmb.com

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://xod.dianchejie.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://uzn.andypj.xyz

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://bbr.kuanghao11.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ryt.hnqzz.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ofc.yvedp.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://uno.sysykeji.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://kru.shanyushiyangkeji.top

[J09] 时区处理
来源：http://lvc.xingfuxueyuan.xyz

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://zxr.cqqwz.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://taj.yanxiufei.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ykk.fehbvm.com

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ltb.gotoacloud.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://oek.bbcook.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://wyv.zdbjq.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://yfy.redwolf501.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://btz.sysykeji.top

[J10] 取今天 / 本月第一天
来源：http://qps.316326.xyz

Py:   date.today();  date.today().replace(day=1)
来源：http://cdq.0kj1m.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://uvv.shuidangran.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ien.ivvv.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hse.ywan-chungtsiang.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://rpi.pycfn.com

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://rip.yangfankeji.com

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ufs.xingfuxueyuan.xyz

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://fdf.aibaodan.cn

================================================================================
来源：http://fgs.wangshuangyany.cn

K. JSON 与序列化
来源：http://dsg.cucudq.cn

================================================================================
来源：http://yca.kuanghao11.cn

[K01] 对象转 JSON 字符串
来源：http://ryf.zhaomingkeji.xyz

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://gfc.zhixingplan.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://pnj.dianchejie.cn

JS:   JSON.stringify(obj)
来源：http://uyy.smart0.xyz

TS:   JSON.stringify(obj)
来源：http://fnp.chenlongwang.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://byx.tian-w.cn

Go:   json.Marshal(obj)
来源：http://pfz.jinqigufen.top

Ruby: obj.to_json                                     // require "json"
来源：http://gzo.vehdjk.com

C#:   JsonSerializer.Serialize(obj)
来源：http://fdm.daria6918.cn

[K02] JSON 字符串转对象
来源：http://gvj.bbcook.cn

Py:   json.loads(s)
来源：http://zqp.jinghuilouyu.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://wtj.nwbrower.top

JS:   JSON.parse(s)
来源：http://lzy.yongpay.top

TS:   JSON.parse(s)
来源：http://wfb.gaohongyu789.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ppq.jqgfzy.top

Go:   json.Unmarshal(data, &v)
来源：http://yya.c1oappe.top

Ruby: JSON.parse(s)
来源：http://okp.shangyingyoupin.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://gah.hnqzz.top

[K03] JSON 美化输出（带缩进）
来源：http://yjy.jinqigfzy.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://log.sjlbkw.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wre.ydzc1.top

JS:   JSON.stringify(obj, null, 2)
来源：http://hem.nanxuanxn.top

TS:   JSON.stringify(obj, null, 2)
来源：http://svf.cucudq.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://nel.daxiang520.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://oeu.feifeiyinyue.top

Ruby: JSON.pretty_generate(obj)
来源：http://ewk.xuanzx.com

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://api.jinghuilouyu.cn

[K04] 读取 JSON 文件
来源：http://xtw.ivvv.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://kvt.cdnleiting.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://cai.jqgfzy.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://pzy.quarkkingdee.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://bxf.fengsongda.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://gpf.uphjek.com

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://exq.zhengqikj.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://pfx.yfazqb.com

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://dee.hcnkem.com

[K05] 深拷贝对象
来源：http://buf.yueranfly.top

Py:   copy.deepcopy(obj)
来源：http://hvl.smart0.xyz

PHP:  unserialize(serialize($obj));
来源：http://dna.iojbl.cn

JS:   structuredClone(obj)
来源：http://ddf.shuidangran.top

TS:   structuredClone(obj)
来源：http://loz.birdmap.top

Java: // 手写拷贝构造，或序列化往返
来源：http://ygm.tian-w.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://xar.tarul.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://oxo.fktsv.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://vfu.tarul.cn

[K06] 解析 URL 查询串
来源：http://pjb.52xcode.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://mgb.xziqi.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://awu.c1oappe.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wuj.dashuyun.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ugv.ybcxt.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://vmw.xinyue.icu

Go:   url.ParseQuery("a=1&b=2")
来源：http://wpe.yanxiufei.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ufl.chenzaomai.com

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://btr.0kj1m.cn

[K07] 进制转换
来源：http://jpt.shangyingyoupin.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://gkq.sweek.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ivp.jinghuilouyu.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ayq.guowangkeji.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://aqy.fehbvm.com

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mwj.xziqi.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://joi.hesvh.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://oso.tian-w.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://tpd.cucudq.cn

[K08] 二进制序列化（非 JSON）
来源：http://nml.smart0.xyz

Py:   pickle.dumps(obj)
来源：http://jrc.yj20258.top

PHP:  serialize($obj);  unserialize($s);
来源：http://vme.daxiang520.top

JS:   v8.serialize(obj)        // Node
来源：http://fyw.hysaishi.cn

TS:   v8.serialize(obj)        // Node
来源：http://zwf.guowangkeji.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://akl.zhoulong.xyz

Go:   encoding/gob
来源：http://scr.gaohongyu789.top

Ruby: Marshal.dump(obj)
来源：http://grn.wangdashe.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://qdb.yvedp.cn

================================================================================
来源：http://zcb.mhx1999.top

L. 网络请求
来源：http://kig.meibo888.top

================================================================================
来源：http://gdq.316326.xyz

[L01] 发送 GET 请求
来源：http://bap.ctjpmb.com

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wiq.mhx1999.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hwm.yuanzhike.top

JS:   await fetch(url)
来源：http://tae.hcnkem.com

TS:   await fetch(url)
来源：http://cam.hnxiangtu.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ixs.zhixingplan.top

Go:   resp, err := http.Get(url)
来源：http://exp.jinyuanbaomall.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://icc.zdqjudy.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://zsz.yvedp.cn

[L02] 发送 POST JSON
来源：http://pip.jinqigufen.top

Py:   requests.post(url, json={"a": 1})
来源：http://ugf.nwbrower.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mlt.gaohongyu789.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://fpw.yfazqb.com

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://yym.andypj.xyz

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hgx.yongpay.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://rqk.uphjek.com

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://fgq.chenlongwang.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://vwq.uphjek.com

[L03] 设置自定义请求头
来源：http://eji.tanke756.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://oin.xinyue.icu

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://sbr.hfpthk.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://nfv.hongshengwenyu.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://vpe.ppjwa.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://kwa.ywan-chungtsiang.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://vxz.shzxlz.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://kca.pengpengdd.cyou

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wda.yangfankeji.com

[L04] 设置超时
来源：http://ggz.ydzc1.top

Py:   requests.get(url, timeout=5)
来源：http://awp.sweek.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mso.tanke756.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ouv.snrcjt.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://auj.chenzaomai.com

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://zct.nanxinkj.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://var.hnqzz.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://kgk.ywan-chungtsiang.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://jqp.zhongyouzk.top

[L05] 上传文件（multipart）
来源：http://duv.haohaochexian.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://eie.sysykeji.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hcs.jqgfzy.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://jpt.xuetiantiany.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://cwy.guowangkeji.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://sul.jinqigufen.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://jdg.shzxlz.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://shh.c1oappe.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://rek.shanyushiyangtech.top

[L06] 解析响应为 JSON
来源：http://gjq.xziqi.cn

Py:   resp.json()
来源：http://rfd.xinyue.icu

PHP:  json_decode($body, true);
来源：http://gam.havefunace.top

JS:   await resp.json()
来源：http://ifl.hesvh.cn

TS:   await resp.json()
来源：http://rcr.shzxlz.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://iln.hfpthk.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ero.jlsjyb.cn

Ruby: JSON.parse(resp.body)
来源：http://gwk.ydzc1.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ytk.yfazqb.com

[L07] 处理 HTTP 状态码
来源：http://ohe.52xcode.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://jwq.smart0.xyz

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://kss.zhoulong.xyz

JS:   resp.ok;  resp.status
来源：http://jxq.yuanzhike.top

TS:   resp.ok;  resp.status
来源：http://vxj.feifeiyinyue.top

Java: resp.statusCode()
来源：http://sib.redwolf501.top

Go:   resp.StatusCode
来源：http://xio.nanxinkj.top

Ruby: resp.code.to_i
来源：http://srp.yj20258888.top


<!-- 参考信息 -->